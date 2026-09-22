# Chapitre 14 — Les données : la matière première

## En mots simples

L'IA ne pense pas toute seule. Elle travaille sur des données, comme une cuisine travaille sur des ingrédients. La qualité du plat dépend de la qualité de ce que vous mettez dedans. Aucun chef, aussi habile soit-il, ne peut faire un bon plat avec des légumes pourris. L'IA est pareille : de bonnes données entrent, des résultats utiles sortent ; de mauvaises données entrent, des résultats inutiles ou nuisibles sortent.

C'est la vérité la plus importante sur l'IA que les patrons d'entreprise ratent. Ils se concentrent sur le modèle — à quel point il est intelligent, quelle marque acheter — et ignorent les données sur lesquelles il tourne. Mais le modèle n'est que le chef. Les données sont la nourriture. La plupart des projets d'IA échouent non pas parce que le modèle était faible, mais parce que les données étaient désordonnées, incomplètes ou fausses.

Les données, en mots simples, sont des informations enregistrées. Noms de clients, historiques de commandes, factures, emails, tableurs, dossiers d'employés, clics sur le site web, relevés de machines — tout cela est des données. Une partie est bien rangée, dans des tables nettes. La plupart sont désordonnées, éparpillées dans des fichiers, des boîtes de réception et du papier. Votre travail est de savoir ce que vous avez, où c'est, et si c'est assez bon pour construire dessus.

Ce chapitre porte sur la façon de traiter vos données comme la matière précieuse qu'elles sont. Il couvre quelles données vous avez et où elles vivent, comment dire si elles sont propres et à jour, les règles de base pour les données personnelles, comment les garder en sécurité, et comment les organiser sans retourner toute votre entreprise. Le traitement juridique approfondi de la vie privée est au [Chapitre 10](ch10-privacy-and-gdpr.md) ; ce chapitre vous donne les bases de travail pour préparer vos données à l'IA.

Une image simple à garder : avant de cuisiner, vous vérifiez le garde-manger. Vous trouvez ce que vous avez, jetez ce qui est gâté, et notez ce qui manque. C'est exactement ce que vous faites avec les données avant tout projet d'IA.

## Un peu d'histoire

**Années 1960-1970 : les données vivent dans des bases de données.** Les entreprises stockaient l'information dans des bases de données structurées — des tables nettes de nombres et de courts textes. C'était propre par conception, mais cela ne couvrait qu'une petite tranche de ce que l'entreprise savait. La plupart des connaissances vivaient sur papier ou dans la tête des gens.

**Années 1980-1990 : tableurs et fichiers.** Les ordinateurs personnels ont répandu les données partout. Tableurs, disques partagés, pièces jointes email. Les données sont devenues abondantes mais éparpillées et incohérentes. Le désordre que nous connaissons tous aujourd'hui a commencé ici.

**Années 2000 : le « big data ».** Internet et les systèmes numériques ont produit des données à une échelle que personne n'avait vue. Les entreprises ont commencé à parler du « big data » comme d'un actif. Mais le volume sans qualité a créé un nouveau problème : des océans de données, peu fiables.

**Années 2010 : la qualité des données devient le goulot d'étranglement.** Avec la croissance de l'analytique et de l'apprentissage automatique, une vérité dure est apparue : la plupart des projets passaient 80 % de leur temps à nettoyer les données, pas à les modéliser. « Poubelle dedans, poubelle dehors » est devenue la leçon marquante de l'époque. La préparation des données, pas les algorithmes astucieux, était le vrai travail.

**2018 : le RGPD relance la mise.** La loi européenne sur la vie privée a fait de la manipulation des données un devoir légal, pas seulement une question de qualité. Désormais, des données désordonnées n'étaient pas seulement inutiles ; des données personnelles mal traitées étaient punissables. La gouvernance des données est devenue un sujet de conseil d'administration.

**Années 2020 : l'IA générative rend la portée des données cruciale.** L'IA moderne peut lire du texte et des images désordonnés, donc elle a besoin de données moins bien rangées que les anciens systèmes. Mais elle dépend toujours d'avoir les bonnes données disponibles et fiables. La leçon tient : le modèle n'est bon que ce que vous lui donnez à manger.

L'arc est clair. Nous sommes passés de trop peu de données structurées à trop de données éparpillées. La compétence n'a jamais changé : la trouver, la nettoyer, et savoir à quoi vous fier.

## Curiosité

### 14.6 Le modèle qui écrivait du Python à partir de livres des années 1930

Voici un fait frappant sur la façon dont les données façonnent ce qu'un modèle peut faire : des chercheurs ont entraîné un modèle de langage uniquement sur des livres d'avant 1931 — pas d'ordinateurs, pas d'internet, et pas de code de programmation, car Python n'existait pas encore — et il pouvait quand même écrire un peu de Python, en copiant la structure des exemples placés devant lui.

Cette expérience, et ce qu'elle enseigne sur les données et la structure, est racontée en entier au [Chapitre 3](ch03-the-words-of-ai-without-the-big-words.md), le foyer canonique pour elle. Le point pour ce chapitre tient en une ligne : **ce qu'un modèle peut faire dépend entièrement de ce sur quoi il a été nourri.** Changez les données, et vous changez la capacité. C'est pourquoi vos propres données sont la matière première qui vaut la peine qu'on s'en soucie.

## Un exemple d'entreprise réel

### Le grossiste dont les « données » étaient trois tableurs contradictoires

Un grossiste en matériaux de construction croyait avoir de bonnes données clients. Quand il a essayé d'utiliser l'IA pour prévoir quels produits chaque client commanderait, le projet a calé dès la première semaine. La raison était les données, pas le modèle.

L'information client vivait à trois endroits : un ancien système de comptabilité, un tableur de ventes tenu par un commercial, et une liste de diffusion dans un logiciel d'email. Le même client apparaissait trois fois avec trois orthographes et adresses différentes. Les historiques de commandes ne correspondaient pas entre les systèmes. La moitié des dossiers n'avaient pas de numéro de téléphone. Les données n'étaient pas exactement fausses — elles étaient fragmentées et incohérentes, ce qui est tout aussi mauvais.

La correction n'était pas high-tech. Ils ont choisi un système comme source unique de vérité pour les fiches clients. Ils ont fusionné les doublons à la main. Ils ont fixé une règle simple : chaque nouveau client entre dans le seul système, une fois. Cela a pris quelques semaines d'un travail ingrat. Après cela, le projet de prévision a fonctionné, car pour la première fois il y avait un seul jeu de données fiable sur lequel construire.

La leçon : l'IA était prête. Les données ne l'étaient pas. La plupart des projets d'IA attendent les données, pas les outils.

## Comment faire

### 14.1 Quelles données vous avez et où elles se trouvent

Vous ne pouvez pas utiliser ce que vous ne pouvez pas trouver. La première étape est un inventaire des données : une simple liste de chaque endroit où votre entreprise garde de l'information.

Parcourez votre entreprise et listez chaque source de données. Les typiques :

- **Systèmes métier.** Logiciel de comptabilité, CRM, stocks, plateforme e-commerce, système RH.
- **Fichiers et tableurs.** Disques partagés, ordinateurs portables personnels, Google Drive, fichiers Excel.
- **Email et messages.** Boîtes de réception, outils de chat, fils sauvegardés.
- **Papier.** Dossiers physiques, formulaires signés, notes.
- **Traces web et numériques.** Analytique du site web, journaux d'application, activité du portail client.
- **Données externes.** Flux de fournisseurs, données de marché, registres publics.

Pour chaque source, notez quatre choses : ce qu'elle contient, qui la possède, à peu près combien il y en a, et à quel point elle est à jour. Ne visez pas la perfection ; visez une carte. Vous voulez voir tout le paysage pour savoir où sont les bonnes données et où sont les manques.

Attendez-vous à des surprises. La plupart des patrons découvrent des données qu'ils avaient oublié exister et des manques qu'ils croyaient comblés. L'inventaire lui-même est précieux car il transforme un sentiment vague de « nous avons des données quelque part » en une image claire.

Un bon inventaire est un tableau. Gardez-le simple et mettez-le à jour au fur et à mesure. Il devient la référence pour chaque futur projet d'IA.

### 14.2 Des données propres, complètes et à jour

Une fois que vous savez ce que vous avez, jugez sa qualité. De bonnes données ont trois qualités.

**Propres.** Exemptes d'erreurs, de doublons et d'incohérences. Le même client n'est pas orthographié de trois façons. Les nombres sont réellement des nombres, pas du texte. Les dates sont de vraies dates. Nettoyer signifie corriger ou supprimer les mauvais dossiers.

**Complètes.** Les champs dont vous avez besoin sont remplis. Si vous avez besoin de la région d'un client pour prévoir la demande, mais que la moitié des dossiers n'ont pas de région, les données sont incomplètes. La complétude signifie que les champs importants sont remplis.

**À jour.** Reflète la réalité maintenant, pas il y a trois ans. Une liste de clients où la moitié des entreprises ont déménagé ou fermé est périmée. Des données périmées mènent à de mauvaises conclusions, peu importe à quel point elles semblent propres.

Comment vérifier la qualité sans outils spéciaux :

- **Contrôle par échantillon.** Tirez 20 dossiers au hasard et cherchez erreurs, doublons et blancs. Le taux d'erreur que vous voyez est à peu près le taux d'erreur que vous avez.
- **Comptez les blancs.** Pour les champs dont vous avez besoin, quelle part sont vides ? Beaucoup de blancs signifient une faible complétude.
- **Vérifiez les dates.** Quand chaque source a-t-elle été mise à jour pour la dernière fois ? Vieux signifie périmé.

Vous n'avez pas besoin de données parfaites. Vous avez besoin de données assez bonnes pour la tâche précise. Une prévision approximative tolère plus de bruit qu'une facture client. Ajustez la barre de qualité au travail. Mais sachez où vous en êtes avant de construire.

Nettoyer est un vrai travail et souvent fastidieux. Prévoyez-le. C'est les 80 % du projet que tout le monde oublie de planifier.

### 14.3 Données personnelles et RGPD : règles de base

Une partie de vos données est des données personnelles — toute information sur une personne vivante qui peut être identifiée : noms, emails, numéros de téléphone, adresses, ID clients, même une adresse IP. Les données personnelles portent des devoirs légaux, et le traitement complet est au [Chapitre 10](ch10-privacy-and-gdpr.md). Voici les bases de travail dont vous avez besoin avant de les utiliser avec l'IA.

**Sachez ce qui est personnel.** Marquez, dans votre inventaire, chaque source qui détient des données personnelles. Vous ne pouvez pas protéger ce que vous n'avez pas identifié.

**Ayez une raison licite.** Sous le RGPD, vous ne pouvez traiter des données personnelles que sur un motif juridique valide — par exemple, un contrat avec la personne, son consentement, ou un intérêt légitime qui ne l'emporte pas sur ses droits. Sachez sur quel motif vous vous appuyez avant de donner les données à l'IA.

**N'utilisez que ce dont vous avez besoin.** Ne déversez pas toutes vos données personnelles dans un outil d'IA quand la tâche n'en demande qu'un peu. Minimisez ce que vous utilisez.

**Surveillez où ça va.** Si vous envoyez des données personnelles à un service d'IA tiers, les données quittent votre contrôle et le RGPD les suit dehors. La manipulation du fournisseur devient votre responsabilité. Les risques tiers sont au [Chapitre 9](ch09-third-party-services-and-shadow-ai.md).

**Respectez les droits des personnes.** Les personnes peuvent demander à voir, corriger ou supprimer leurs données. Votre usage de l'IA ne doit pas rendre cela impossible.

Ceci est un guide simple, pas un conseil juridique. Pour de vraies décisions, surtout au-delà des frontières, consultez un professionnel de la protection des données. Mais l'habitude — marquer les données personnelles, connaître votre motif, utiliser le minimum — est à vous de construire maintenant.

### 14.4 Sécurité, sauvegarde et accès

Les données sont un actif, et les actifs ont besoin d'être protégés. Trois bases couvrent la majeure partie du risque.

**Sécurité.** Protégez les données des attaquants et des fuites. Utilisez des mots de passe forts et l'authentification multifacteur, gardez les systèmes à jour, chiffrez les données sensibles, et soyez prudent avec les pièces jointes et les liens email. Le tableau complet de la sécurité, y compris les menaces propres à l'IA, est au [Chapitre 6](ch06-cybersecurity-in-the-ai-era.md).

**Sauvegarde.** Gardez des copies de vos données à l'abri du système principal. Si un système plante, est frappé par un rançongiciel, ou un fichier est supprimé, une sauvegarde fait la différence entre une mauvaise journée et perdre l'entreprise. Suivez une règle simple : gardez des copies à plus d'un endroit, sauvegardez régulièrement, et testez que vous pouvez réellement restaurer. Une sauvegarde dont vous n'avez jamais testé la restauration n'est qu'un espoir.

**Accès.** Contrôlez qui peut voir et modifier quoi. Tout le monde n'a pas besoin d'accéder à tout. Donnez aux gens l'accès minimal que leur rôle exige. Journalisez qui accède aux données sensibles. Limiter l'accès limite à la fois les accidents et les vols.

Ces trois fonctionnent ensemble. La sécurité garde les extérieurs dehors. La sauvegarde vous sauve quand quelque chose tourne mal malgré tout. L'accès limite les dégâts que n'importe quelle personne ou erreur peut causer. Aucun n'est facultatif.

Une habitude pratique : sauvegardez automatiquement, vérifiez la sauvegarde chaque mois, et revoyez qui a accès chaque trimestre. De petites routines, répétées, préviennent les catastrophes.

### 14.5 Comment organiser les données sans tout retourner

La plus grande peur du travail sur les données est que cela signifie une refonte énorme et perturbatrice. Ce n'est pas le cas. Vous pouvez améliorer vos données étape par étape sans arrêter l'entreprise.

**Choisissez une source unique de vérité par chose.** Pour chaque type important de données — clients, produits, commandes — choisissez un système comme étant l'officiel. Tout le reste devient une copie ou une vue. Cette seule règle corrige la plupart des confusions sans changer vos outils.

**Corrigez au point d'entrée.** Le moment le moins cher pour nettoyer des données est quand elles sont créées. Fixez des règles simples pour que les nouveaux dossiers aillent au bon endroit, une fois, avec les champs clés remplis. Empêcher le nouveau désordre bat nettoyer l'ancien désordre pour toujours.

**Ne faites pas bouillir l'océan.** N'essayez pas de tout nettoyer. Nettoyez seulement les données dont vos premiers projets d'IA ont besoin. Des données parfaites que vous n'utilisez jamais sont un effort gaspillé. Un nettoyage ciblé qui sert un vrai projet vaut la peine d'être fait.

**Standardisez un peu, pas parfaitement.** Convenez de quelques formats simples — comment écrire une date, un numéro de téléphone, un nom de client — et appliquez-les pour l'avenir. Vous n'avez pas besoin d'une grande norme, juste de la cohérence pour les champs qui comptent.

**Améliorez au fur et à mesure.** Traitez la qualité des données comme une habitude, pas un projet. Chaque petite correction rend le prochain usage de l'IA plus facile. Sur un an, de petites améliorations constantes s'additionnent en une solide fondation de données.

L'état d'esprit : vous ne reconstruisez pas la maison. Vous rangez le garde-manger, une étagère à la fois, pour que le prochain repas soit plus facile à cuisiner. Commencez par l'étagère dont votre premier projet a besoin.

## Éthique et responsabilité

Les données portent un poids éthique au-delà de la qualité et de la loi.

**Les données personnelles sont des personnes.** Derrière chaque dossier se trouve une personne avec des droits et des sentiments. Manipulez-les en gardant cela en tête, pas juste comme une ressource à extraire. Les principes sont au [Chapitre 4](ch04-ethical-ai-doing-the-right-thing.md).

**Le biais vit dans les données.** Si vos données sous-représentent un groupe, une IA entraînée dessus traitera ce groupe mal. Un jeu de données d'embauche avec surtout un seul type de candidat biaiserera l'IA de la même façon. Vérifiez les données de qui manquent, pas seulement si les données sont propres.

**N'utilisez pas des données que les gens n'attendaient pas.** Ce n'est pas parce que vous détenez des données que vous devriez les utiliser pour n'importe quelle finalité. Utiliser les données clients d'une façon à laquelle ils n'ont jamais consenti brise la confiance, même si c'est légal. Restez dans les attentes raisonnables.

**Soyez honnête sur ce que vous collectez et pourquoi.** Dites aux gens quelles données vous rassemblez et comment vous les utilisez. Une collecte cachée est une trahison de la confiance et souvent de la loi.

**Protégez-les comme si c'était les vôtres.** Une fuite blesse de vraies personnes, pas seulement votre réputation. Traitez la sécurité comme un devoir envers les personnes dans vos données, pas juste une case à cocher.

## Erreurs à éviter

### 14.7 Erreurs courantes avec les données

1. **Ignorer les données jusqu'à ce que le projet échoue.** L'erreur la plus courante. Vérifiez vos données avant de commencer, pas après qu'il cale.
2. **Supposer que vous avez des données quand vous avez des fragments.** Trois tableurs contradictoires ne font pas un jeu de données. Trouvez d'abord la vérité.
3. **Confondre volume et qualité.** Beaucoup de données n'est pas de bonnes données. Un petit jeu propre bat un grand jeu désordonné.
4. **Ne pas planifier le temps de nettoyage.** La préparation des données est la majeure partie du travail. Prévoyez-le ou le projet glisse.
5. **Pas de source unique de vérité.** Plusieurs versions « officielles » garantissent la confusion. Choisissez-en une.
6. **Utiliser des données personnelles sans base légale.** Un risque légal et un risque de confiance. Connaissez d'abord votre motif.
7. **Envoyer des données personnelles à une IA tierce sans soin.** Le RGPD suit les données dehors.
8. **Sauvegardes non testées.** Une sauvegarde qui ne peut pas restaurer n'est pas une sauvegarde. Testez-la.
9. **Tout le monde a accès à tout.** Un large accès signifie un large risque. Limitez-le au rôle.
10. **Essayer de tout nettoyer d'un coup.** Paralysie de refonte. Nettoyez seulement ce dont votre projet a besoin.
11. **Ignorer les données périmées.** Des données propres mais vieilles donnent quand même de mauvaises réponses. Vérifiez les dates.
12. **Oublier le biais dans les données.** Un manque dans qui est représenté devient un biais dans le résultat.

## Exercice pratique

### 14.8 Inventaire des données

Passez un après-midi à construire un simple inventaire des données. C'est la préparation la plus utile que vous puissiez faire pour l'IA.

Faites un tableau avec une ligne par source de données. Pour chacune, remplissez :

- **Source** — le système, le fichier ou l'endroit (par ex. « logiciel de comptabilité », « tableur de ventes », « boîte de réception email »).
- **Ce qu'elle contient** — clients, commandes, factures, CV, etc.
- **Propriétaire** — qui en est responsable.
- **Volume** — à peu près combien (lignes, fichiers, Go).
- **Données personnelles ?** — Oui / Non.
- **Qualité** — contrôle par échantillon de 20 dossiers ; notez blancs, doublons, erreurs. Notez propre / mitigé / médiocre.
- **À jour ?** — quand mis à jour pour la dernière fois.
- **Source unique de vérité ?** — Oui / Non / candidat.

Remplissez chaque source que vous pouvez trouver. Une fois fait, regardez l'image :

- Quelles sources sont propres et à jour ? Ce sont vos meilleures matières de départ.
- Lesquelles détiennent des données personnelles ? Marquez-les pour les bases RGPD du 14.3.
- Où avez-vous des doublons sans source unique de vérité ? Ce sont vos premières cibles de nettoyage.
- Que manque-t-il que votre premier projet d'IA demande ? Ce sont des manques à combler.

Ce tableau vous dit, honnêtement, si vous êtes prêt à démarrer un projet d'IA ou s'il faut d'abord corriger les données. Gardez-le et mettez-le à jour. C'est la liste du garde-manger pour tout ce que vous construirez ensuite.

## Liste de contrôle

### 14.9 Liste de contrôle des données

Avant de donner des données à un projet d'IA, vérifiez ceci.

- [ ] **Vous avez un inventaire des données** listant chaque source et ce qu'elle contient.
- [ ] **Vous savez où sont les bonnes données** et où sont les manques.
- [ ] **Vous avez une source unique de vérité** pour chaque type clé de données.
- [ ] **Vous avez fait un contrôle par échantillon de la qualité** et connaissez le taux d'erreur et de blancs.
- [ ] **Les données sont assez propres pour la tâche précise** que vous faites.
- [ ] **Les données sont à jour** et reflètent la réalité actuelle.
- [ ] **Vous avez marqué toutes les données personnelles** dans l'inventaire.
- [ ] **Vous avez une base légale** pour toute donnée personnelle que vous utilisez (voir [Chapitre 10](ch10-privacy-and-gdpr.md)).
- [ ] **Vous n'utilisez que le minimum de données personnelles** que la tâche demande.
- [ ] **Vous savez où vont les données** si un service d'IA tiers y touche.
- [ ] **Les bases de sécurité sont en place** — authentification forte, mises à jour, chiffrement pour les données sensibles.
- [ ] **Des sauvegardes existent, sont récentes, et ont été testées pour la restauration.**
- [ ] **L'accès est limité** aux rôles qui en ont besoin, avec journalisation sur les données sensibles.
- [ ] **Vous corrigez les nouvelles données au point d'entrée**, pas seulement en nettoyant les anciennes.
- [ ] **Vous avez vérifié le biais** — les données de qui manquent ?

Si une case est vide et que votre projet en dépend, corrigez cela avant de construire. De bonnes données ne sont pas un détail ; c'est la matière première sur laquelle tout le reste tourne.

## Points à retenir

- Les données sont la matière première de l'IA : de bonnes données entrent, des résultats utiles sortent ; de mauvaises données entrent, des résultats inutiles ou nuisibles sortent — le modèle n'est que le chef.
- Commencez par un inventaire des données : vous ne pouvez pas utiliser ce que vous ne pouvez pas trouver, et la plupart des patrons sont surpris par ce qu'ils ont et ce qui manque.
- La qualité signifie propre, complet et à jour ; planifiez le temps de nettoyage, car c'est la majeure partie du travail que tout le monde oublie.
- Les données personnelles portent des devoirs légaux — marquez-les, connaissez votre base légale, utilisez le minimum, et rappelez-vous que le RGPD les suit vers tout service tiers.
- Vous pouvez améliorer les données étape par étape sans refonte : choisissez une source unique de vérité, corrigez au point d'entrée, et nettoyez seulement ce dont votre projet a besoin.

<!-- BEGIN agentbridge-examples -->

## Essayez avec AgentBridge

Voici à quoi ressemble le même travail avec AgentBridge. Chaque encadré montre le résultat fini et la seule ligne que vous tapez pour l'obtenir.

### Posez des questions sur vos propres fichiers

![L'agent répondant à partir de vos propres documents](../../assets/examples/ask-your-documents.png)
*L'agent répondant à partir de vos propres documents*

**Ce que vous demandez :** `Quelle est notre politique d'annulation avec le fournisseur d'impression ?`

L'agent cherche dans votre espace de documents et répond avec ce que vos propres fichiers disent réellement, en pointant la source.

*Conseil : Gardez vos fichiers d'entreprise dans l'espace de documents et ils deviennent une connaissance consultable.*

---

### Retrouver ce vieux document

![Une recherche dans votre archive indexée](../../assets/examples/find-in-archive.png)
*Une recherche dans votre archive indexée*

**Ce que vous demandez :** `Retrouve la proposition que j'ai envoyée à l'hôtel au printemps dernier au sujet du réaménagement du hall.`

L'agent cherche dans votre archive indexée et vous rapporte le document que vous vouliez, même quand vous ne vous en souvenez qu'à moitié.

*Conseil : L'index se met à jour à mesure que vous ajoutez des fichiers, donc l'archive est toujours à jour.*

---

### Il se souvient de la façon dont vous aimez les choses

![L'agent appliquant vos préférences enregistrées](../../assets/examples/remember-preferences.png)
*L'agent appliquant vos préférences enregistrées*

**Ce que vous demandez :** `Fais une facture — tu sais comment je les aime.`

L'agent se souvient de votre style et de vos réglages d'avant et les applique sans que vous ayez à vous répéter.

*Conseil : Vous pouvez le corriger à tout moment ; il met à jour ce dont il se souvient.*

---

### Rien n'est jamais perdu

![L'historique des versions permet de revenir en arrière en toute sécurité](../../assets/examples/version-history.png)
*L'historique des versions permet de revenir en arrière en toute sécurité*

**Ce que vous demandez :** `Montre-moi la version précédente du contrat et restaure-la.`

Chaque version créée par l'agent est conservée. Vous pouvez voir le brouillon antérieur et le ramener, donc éditer est toujours sûr.

*Conseil : C'est pourquoi vous pouvez laisser l'agent réécrire librement — l'historique vous protège.*

<!-- END agentbridge-examples -->
