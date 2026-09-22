# Chapitre 17 — Choisir ses outils sans se faire avoir

## En mots simples

Chaque fournisseur d'IA vous dira que son outil est facile, bon marché et révolutionnaire. Certains disent la vérité. Beaucoup non. Ce chapitre est votre défense. Il vous apprend à voir au-delà de la démo séduisante et du commercial convaincant, et à choisir un outil qui convient vraiment à votre entreprise.

L'idée la plus importante est simple : **vous n'achetez pas un outil, vous achetez un résultat.** Un outil ne vaut que ce qu'il fait pour vous. Un produit magnifique qui ne résout pas votre problème est un jouet coûteux. Votre travail consiste à relier chaque choix à un vrai problème et à un vrai chiffre.

Une bonne analogie est l'achat d'une voiture. Le showroom rend chaque voiture magnifique. Le cuir brille, le moteur ronronne, le commercial est charmant. Mais vous n'achetez pas une voiture pour le showroom. Vous l'achetez pour la route que vous parcourez vraiment, les passagers que vous transportez vraiment et le carburant que vous pouvez vous permettre. Alors vous posez des questions difficiles, vous faites un essai sur *vos* routes, et vous lisez les coûts d'utilisation. Choisir des outils d'IA demande la même discipline.

Ce chapitre explique comment trancher entre acheter un logiciel prêt à l'emploi, en faire développer un sur mesure, ou le faire soi-même. Il vous donne les questions exactes à poser à un fournisseur. Il montre où se cachent les coûts cachés. Il explique pourquoi une démo ne suffit pas et comment mener plutôt un petit pilote. Et il examine les outils open source — des logiciels dont le code est libre d'utilisation et de modification — comme une option réelle et abordable.

Une règle à garder avec vous : **ralentissez.** Le commercial veut de l'urgence. « Ce prix se termine vendredi. » « Il ne reste que deux licences. » L'urgence est une astuce pour vous empêcher de réfléchir. Un bon outil survit à une semaine de réflexion attentive. Un mauvais compte sur le fait que vous ne réfléchirez pas. Prenez cette semaine.

## Un peu d'histoire

**Années 1960–1970 : le logiciel est sur mesure.** Aux débuts, si une entreprise voulait un logiciel, elle payait des spécialistes pour l'écrire de zéro. Il n'y avait pas d'option « du commerce ». Le logiciel était un costume sur mesure, fait à la mesure, coûteux et long à livrer.

**Années 1980 : la révolution des logiciels packagés.** Des produits comme les tableurs et les traitements de texte sont arrivés dans une boîte. Pour la première fois, une entreprise pouvait acheter un outil général et l'adapter à beaucoup de tâches. C'était moins cher et plus rapide que les développements sur mesure. Le marché moderne du logiciel était né.

**Années 1990–2000 : les grandes suites et le piège de l'enfermement.** Les grands fournisseurs vendaient d'immenses suites intégrées — un produit pour tout. Elles fonctionnaient bien, mais s'en détourner était douloureux et coûteux. Les entreprises ont découvert que le choix facile du jour pouvait devenir une prison coûteuse le lendemain. Le mot **enfermement fournisseur** — se retrouver bloqué avec un fournisseur parce que partir est trop difficile — est entré dans le vocabulaire des affaires. (L'enfermement est traité en détail au [Chapitre 9](ch09-third-party-services-and-shadow-ai.md).)

**Années 2000 : l'open source devient courant.** Linux, Apache, puis des milliers de projets libres ont prouvé qu'un logiciel pouvait être construit par des communautés et offert, tout en faisant tourner les plus grands sites du monde. L'open source a cessé d'être un passe-temps pour devenir une option sérieuse et fiable.

**Années 2010 : l'ère de l'abonnement.** Le logiciel est passé du « acheter une fois » au « payer chaque mois ». Cela a abaissé le prix d'entrée mais a ajouté un nouveau type de coût qui ne s'arrête jamais. Les abonnements ont rendu le démarrage facile et il est devenu facile de perdre la trace de ce à quoi on payait.

**Années 2020 : la ruée vers l'IA.** Des centaines d'outils d'IA sont apparus presque du jour au lendemain, beaucoup avec de gros financements et de plus grosses promesses. L'écart entre ce qu'une démo montre et ce qu'un outil livre dans le vrai travail n'a jamais été aussi grand. Bien choisir est aujourd'hui une compétence centrale de l'entreprise, pas un simple bonus.

L'arc : du sur mesure, à la boîte, à l'abonnement, à l'inondation. Les outils n'en finissent pas de changer. Le besoin de choisir avec soin, jamais.

## Curiosité

### 17.6 Le livre « Headcount Zero » — une entreprise sans employés

Jusqu'où peut aller l'idée « pas besoin de gens » ? Il existe un livre qui la pousse à l'extrême. Il s'appelle **« Headcount Zero: How to Build an AI-Run Company with Paperclip »**, d'**Anthony David Adams**. Il est publié comme livre open source sur GitHub (le dépôt `AnthonyDavidAdams/zero-employee-company-book`), donc n'importe qui peut le lire gratuitement.

La question que pose le livre est : *et si vous n'aviez jamais à embaucher personne ?* Au lieu d'employés, le fondateur dirige une entreprise faite d'**agents IA** — des programmes informatiques capables d'accomplir des tâches seuls. Le fondateur devient une sorte de manager d'un organigramme rempli de travailleurs IA, coordonnés par une plateforme open source que le livre appelle **Paperclip**.

Ce n'est pas un plan que la plupart des petites entreprises devraient suivre dès demain. Une entreprise littéralement sans aucun humain est une expérience de pensée extrême, et elle a des limites évidentes : qui est responsable quand quelque chose tourne mal ? Qui porte la responsabilité légale ? Qui comprend le besoin non dit d'un client ? (Ce sont exactement les rôles humains discutés au [Chapitre 15](ch15-people-roles-and-culture.md).)

Mais comme lentille, « Headcount Zero » est utile. Il force une question honnête : **quelle part de votre travail est vraiment humaine, et quelle part est de la routine qu'une machine pourrait porter ?** La plupart des entreprises constatent qu'une part surprenante des tâches quotidiennes est routinière. Cela ne veut pas dire licencier tout le monde. Cela veut dire libérer les gens des parties ennuyeuses pour qu'ils fassent le jugement, les relations et le travail créatif que les machines ne peuvent pas. Lisez le livre comme une provocation, pas comme une consigne. Il vous montre la limite du possible, et la limite est là où vivent les questions intéressantes.

## Un exemple d'entreprise réel

*Ce qui suit est une composition illustrative de schémas réels courants, pas une seule entreprise nommée.*

Un petit cabinet comptable voulait « automatiser avec l'IA ». Un fournisseur a fait une démo éblouissante : l'outil lisait une pile de reçus et produisait un résumé net en quelques secondes. Le patron a signé un contrat de deux ans sur le coup, ébloui.

Six mois plus tard, la réalité avait une autre tête. La démo avait utilisé une poignée de reçus propres et parfaits. Les vrais reçus du cabinet étaient froissés, flous, en trois langues, et pleins de cas limites. L'outil se trompait assez souvent pour que le personnel doive tout revérifier, ce qui faisait que l'« économie » était minuscule. Le contrat de deux ans les a enfermés. L'abonnement continuait de facturer. L'outil est devenu un ornement coûteux.

Un second cabinet a choisi autrement. Avant de signer quoi que ce soit, il a demandé au fournisseur un **essai sur ses propres données désordonnées**, pas sur le jeu de démo propre du fournisseur. Il a mené un pilote de deux semaines sur de vrais reçus. L'outil en gérait bien environ 70 % et échouait sur le reste. Ce chiffre — 70 % — a permis au cabinet de prendre une décision claire : garder l'outil pour les 70 % faciles, garder des humains sur les 30 % difficiles, et signer seulement un contrat d'un an avec une sortie claire. Le même outil, choisi avec discipline au lieu d'éblouissement, est devenu une vraie aide.

La différence n'était pas le logiciel. C'est que le second cabinet a refusé de se faire avoir par une démo et a testé d'abord sur sa propre réalité.

## Comment faire

### 17.1 Logiciel du commerce, développement sur mesure, ou faire soi-même

Quand vous avez besoin d'un outil, vous avez trois grandes voies. Chacune a sa place.

**Du commerce (acheter prêt à l'emploi).** C'est un logiciel auquel vous vous abonnez ou que vous achetez tel quel, comme un service de chatbot ou une application de résumé de documents. C'est la façon la plus rapide et souvent la moins chère de démarrer. Vous l'obtenez aujourd'hui, il fonctionne dès la sortie de la boîte, et quelqu'un d'autre l'entretient. La contrepartie : il fait ce que *lui* a été construit pour faire, pas exactement ce que *vous* vouliez. Si votre besoin est courant, un outil du commerce est presque toujours le bon premier choix.

**Sur mesure (payer quelqu'un pour le construire).** Un développeur écrit un logiciel rien que pour vous. Cela colle parfaitement à vos besoins. Mais c'est lent, coûteux, et vous possédez désormais une chose qui demande un entretien pour toujours. Le sur mesure n'a de sens que si votre besoin est particulier et qu'aucun outil prêt à l'emploi ne le couvre — et si la valeur est assez élevée pour justifier le coût. Pour la plupart des petites entreprises, le sur mesure est rarement le premier mouvement.

**Faire soi-même (vous le construisez, avec du no-code ou des outils légers).** Des outils comme les applications d'automatisation vous permettent de connecter des services vous-même sans écrire de code. C'est bon marché et flexible, et on apprend beaucoup. La contrepartie : cela prend votre temps, et si vous partez, ce que vous avez construit peut être difficile à entretenir par quelqu'un d'autre. Le fait-maison est excellent pour les petites automatisations que vous pouvez posséder et garder simples.

Une règle simple : **commencez par du commerce. Passez au fait-maison pour les petites soudures entre outils. N'allez sur mesure que si rien d'autre ne convient et que la récompense est grosse.** La plupart des entreprises vivent heureuses avec les deux premières.

### 17.2 Les questions à poser au fournisseur

Ne prenez jamais la parole d'un fournisseur pour argent comptant. Posez des questions directes et écoutez attentivement les réponses — surtout ce qu'ils esquivent. Gardez celles-ci prêtes :

- **Que fait exactement ceci, et que ne fait-il PAS ?** Forcez-les à dépasser le marketing. Un « ça gère tout » assuré est un signal d'alarme.
- **À quoi cela ressemble-t-il quand ça échoue ?** Chaque outil échoue quelque part. Un fournisseur honnête peut nommer ses points faibles. Un fournisseur qui dit « ça ne rate jamais » ment ou est inconscient.
- **Quel est le coût total sur trois ans, pas seulement le premier mois ?** Faites-leur dire le chiffre complet à voix haute.
- **Que devient ma donnée ?** Où est-elle stockée, qui peut la voir, et entraînez-vous votre IA dessus ? (Cela compte pour la vie privée — voir [Chapitre 10](ch10-privacy-and-gdpr.md).)
- **Puis-je récupérer ma donnée, et dans quel format ?** C'est votre issue de secours. Si vous ne pouvez pas partir proprement, vous êtes enfermé.
- **Quelle assistance ai-je, et à quelle vitesse ?** Délais de réponse, canaux, et si l'assistance est incluse ou coûte en plus.
- **Qui d'autre utilise ceci dans mon secteur, et puis-je leur parler ?** Une vraie référence vaut dix démos.
- **Quelle est votre feuille de route, et à quel point l'entreprise est-elle stable ?** Un outil d'une startup fragile peut disparaître. Demandez depuis combien de temps ils sont en activité et qui les finance.
- **Quel est le contrat, et comment je résilie ?** Lisez les conditions de sortie avant de signer, pas après.

Écrivez les réponses. Comparez les fournisseurs sur les mêmes questions. Le fournisseur qui répond clairement et honnêtement se distingue de celui qui agite les bras et charme.

### 17.3 Coûts cachés et abonnements

Le prix affiché est le plus petit des coûts. Le vrai coût se cache là où la plupart des gens ne regardent jamais. (La méthode complète des coûts se trouve au [Chapitre 16](ch16-goals-costs-and-return-on-investment.md) ; voici la version propre au fournisseur.)

Méfiez-vous de ceci :

- **Tarif par poste.** Beaucoup d'outils facturent par utilisateur. Un outil « bon marché » devient cher quand on ajoute toute l'équipe. Comptez les postes avant de signer.
- **Frais à l'usage.** Certains outils d'IA facturent par tâche, par message ou par document. Un mois chargé peut produire une facture surprise. Demandez exactement comment l'usage est mesuré.
- **Frais de mise en place et d'intégration.** Démarrer peut coûter en plus, parfois plus que la première année d'abonnement.
- **Coûts d'intégration.** Connecter l'outil à vos systèmes existants peut demander une aide payante.
- **Fonctions premium derrière un paywall.** La fonction qui vous a vendu est peut-être sur une offre supérieure. Vérifiez quelle offre il vous faut vraiment.
- **Formation et assistance en options.** « Assistance incluse » veut souvent dire un article d'aide, pas une personne. La vraie aide peut coûter plus.
- **L'abonnement sans fin.** Une redevance mensuelle semble petite mais ne s'arrête jamais. Multipliez-la par trois ou cinq ans pour voir le vrai poids.
- **Coûts de sortie et de changement.** Résilier peut être difficile, et déplacer vos données ailleurs peut demander un travail payant.

Avant de signer, construisez un **coût total sur trois ans** pour chaque option. Ajoutez chacun de ces éléments. Le prix mensuel du fournisseur n'est souvent qu'un tiers du vrai chiffre sur trois ans.

### 17.4 Démos et projets pilotes

Une démo est une représentation. Elle montre l'outil à son meilleur, sur des données choisies pour vous convaincre. Ne décidez jamais sur une démo seule.

Un **projet pilote** est l'alternative honnête. Un pilote est un essai petit et limité dans le temps de l'outil sur *votre* vrai travail, avec *vos* vraies données désordonnées, mesurant *votre* vrai résultat. Là où une démo vous montre un best-of, un pilote vous montre la vérité.

Comment mener un bon pilote :

- **Utilisez vos propres données, y compris les cas désordonnés.** N'acceptez pas l'échantillon propre du fournisseur.
- **Gardez-le petit et court.** Deux à quatre semaines sur un processus suffisent pour apprendre beaucoup.
- **Définissez la réussite avant de commencer.** Quel chiffre l'outil doit-il atteindre pour compter comme une réussite ? (Cela se rattache à la méthode du pilote au [Chapitre 18](ch18-your-first-pilot-project.md).)
- **Testez l'échec, pas seulement la réussite.** Poussez-le avec des cas difficiles exprès.
- **Essayez l'assistance.** Envoyez une demande d'assistance pendant le pilote et voyez à quel point ils sont rapides et utiles.
- **Testez la sortie.** Essayez d'exporter vos données. Assurez-vous de pouvoir partir.

Un fournisseur qui refuse un vrai pilote sur vos données vous dit quelque chose. Un fournisseur qui l'accueille est confiant pour une bonne raison.

### 17.5 Outils open source : une alternative abordable et flexible

**Open source** signifie que le code source du logiciel — les instructions qui le font fonctionner — est libre pour n'importe qui de le voir, l'utiliser et le modifier. Vous ne le « piratez » pas ; l'open source est une façon légale, courante et souvent excellente dont le logiciel est fait. Le web que vous utilisez en ce moment tourne probablement sur des logiciels open source.

Pourquoi y penser pour l'IA :

- **Coût de licence faible ou nul.** Beaucoup d'outils open source sont libres d'utilisation.
- **Pas d'enfermement.** Parce que vous pouvez voir et modifier le code, vous n'êtes pas piégé avec un seul fournisseur.
- **Vous pouvez l'exécuter vous-même.** Des modèles d'IA open source peuvent tourner sur vos propres machines, ce qui garde votre donnée sous votre contrôle (c'est l'**auto-hébergement**, traité au [Chapitre 8](ch08-self-hosting-keep-your-data-under-control.md)).
- **Une communauté derrière.** Les projets populaires s'améliorent vite et ont beaucoup d'utilisateurs pour apprendre.

Les contreparties :

- **Vous aurez peut-être besoin de plus de compétence pour le configurer.** L'open source suppose souvent que vous savez configurer des choses, ou pouvez embaucher quelqu'un qui le sait.
- **L'assistance est communautaire.** Il n'y a peut-être personne à appeler. Vous comptez sur la documentation et les forums.
- **Vous possédez la maintenance.** Si vous l'exécutez vous-même, le garder à jour et sécurisé est à votre charge.

L'équilibre honnête : l'open source est une voie puissante et abordable, surtout quand le contrôle des données compte. Mais il échange de l'argent contre de l'effort et de la compétence. Si vous n'avez ni l'un ni l'autre, un outil du commerce payant est peut-être un départ plus sage. Si vous avez un peu d'aide technique, l'open source peut vous faire économiser beaucoup et vous libérer de l'enfermement.

## Éthique et responsabilité

Choisir des outils n'est pas éthiquement neutre. Vos choix affectent vos clients, votre personnel et vos données.

**Protégez la donnée de vos clients dans le choix lui-même.** Avant qu'un outil ne touche une donnée client, sachez où elle va et qui peut la voir. Un outil qui entraîne son IA sur les informations privées de vos clients sans consentement peut enfreindre la loi (voir [Chapitre 10](ch10-privacy-and-gdpr.md)).

**Ne laissez pas le battage d'un fournisseur piloter une décision qui touche des gens.** Si un outil doit changer les postes de votre personnel, choisissez-le pour des raisons honnêtes et impliquez vos gens, pas parce qu'un commercial a créé une fausse urgence.

**Préférez des outils que vous pouvez auditer et quitter.** Un outil qui cache comment il fonctionne, ou piège votre donnée, est un mauvais choix éthique autant qu'un mauvais choix commercial. La transparence et une sortie propre sont les signes d'un fournisseur qui vous respecte.

**Soyez honnête dans vos propres affirmations.** Si vous achetez un outil d'IA et dites aux clients « notre service utilise l'IA », assurez-vous que c'est vrai et non un marketing exagéré.

**Considérez l'éthique du fournisseur lui-même.** Où vit leur donnée ? Respectent-ils les lois sur la vie privée ? Sont-ils stables et honnêtes ? Vous vous associez avec eux ; choisissez un partenaire à qui vous confieriez votre nom.

Un outil est une relation. Choisissez le partenaire avec autant de soin que vous choisiriez un associé.

## Erreurs à éviter

### 17.7 Erreurs courantes

**Acheter sur la démo.** Décider d'après une représentation soignée sur des données propres. Menez toujours un pilote sur votre propre réalité désordonnée.

**Ignorer le coût sur trois ans.** Regarder le prix mensuel et pas le total. L'abonnement ne s'arrête jamais.

**Tomber dans l'urgence.** « Le prix se termine vendredi » est une astuce de vente. Un bon outil survit à une semaine de réflexion.

**Pas de plan de sortie.** Signer sans vérifier comment récupérer vos données. C'est ainsi que l'enfermement arrive.

**Acheter avant de définir le problème.** Prendre un outil puis chercher un usage. Définissez d'abord le problème, puis trouvez l'outil.

**Confondre popularité et adéquation.** Un outil utilisé par des milliers de gens peut quand même ne pas coller à *votre* flux de travail.

**Sauter le test de l'assistance.** Ne pas vérifier comment le fournisseur se comporte après la vente. Testez l'assistance pendant le pilote.

**Sur-customiser trop tôt.** Payer pour un développement sur mesure quand un outil du commerce couvrirait 80 % du besoin.

**Sous-estimer la maintenance du fait-maison.** Le construire soi-même et oublier qu'il faut maintenant le maintenir en vie.

**Croire « ça gère tout ».** Aucun outil ne le fait. Un fournisseur qui affirme le contraire ne vous dit pas la vérité.

**Ne pas lire le contrat.** Signer sans lire les conditions de résiliation et de donnée. Lisez avant, pas après.

**Choisir l'étiquette la moins chère.** Le prix mensuel le plus bas peut cacher le coût total le plus élevé.

## Exercice pratique

### 17.8 Exercice : une grille d'évaluation

Construisez une simple grille de notation pour comparer les outils côte à côte. Cela transforme un choix flou en un choix clair.

**Étape 1 — Listez vos options.** Écrivez deux ou trois outils candidats (ou voies : du commerce, fait-maison, open source).

**Étape 2 — Listez les critères.** Utilisez ceux-ci, ou ajoutez les vôtres :

- Correspond à mon vrai problème (0–5)
- Gère bien mes données désordonnées (0–5)
- Coût total sur trois ans (moins c'est mieux — notez-le)
- Facilité d'utilisation pour mon personnel (0–5)
- Vie privée et contrôle des données (0–5)
- Facilité de sortie / pas d'enfermement (0–5)
- Qualité de l'assistance (0–5)
- Stabilité du fournisseur (0–5)

**Étape 3 — Notez chaque outil.** Donnez un chiffre pour chaque critère. Soyez honnête, pas optimiste.

**Étape 4 — Pondérez ce qui compte le plus.** Si la vie privée des données est critique pour vous, doublez son poids. Si le coût compte le plus, pondérez-le plus haut.

**Étape 5 — Additionnez.** L'outil avec le score pondéré le plus élevé est votre favori.

**Étape 6 — Testez le favori avec un pilote.** La grille resserre le terrain ; le pilote le confirme. Ne sautez pas le pilote.

Mettez la grille sur une page. Elle rend la décision visible et défendable, et elle empêche un commercial charmant de faire passer votre jugement à la trappe avec son charme.

## Liste de contrôle

### 17.9 Liste de contrôle pour évaluer un fournisseur

Avant de signer avec un fournisseur d'IA, cochez chaque case.

- [ ] **Je peux énoncer le problème exact que cet outil résout pour moi.**
- [ ] **Je sais ce que l'outil ne fait PAS, et où il échoue.**
- [ ] **J'ai un coût total sur trois ans, pas seulement le prix mensuel.**
- [ ] **Je sais comment la tarification fonctionne** — par poste, à l'usage, offres, frais de mise en place.
- [ ] **Je sais où ma donnée est stockée et qui peut la voir.**
- [ ] **Je sais si le fournisseur entraîne son IA sur ma donnée, et j'accepte ou je refuse.**
- [ ] **J'ai testé l'outil sur mes propres données désordonnées, pas le jeu de démo du fournisseur.**
- [ ] **J'ai mené un petit pilote avec un chiffre de réussite défini.**
- [ ] **J'ai testé l'assistance du fournisseur pendant l'essai.**
- [ ] **J'ai testé l'export de mes données hors de l'outil.**
- [ ] **J'ai lu les conditions de résiliation avant de signer.**
- [ ] **J'ai une référence d'une autre entreprise de mon domaine, ou j'ai essayé d'en obtenir une.**
- [ ] **J'ai vérifié la stabilité du fournisseur et depuis combien de temps il est en activité.**
- [ ] **J'ai résisté à l'urgence et pris le temps de réfléchir.**
- [ ] **J'ai comparé au moins deux options sur les mêmes critères.**

Si une case est vide, vous n'avez pas fini d'évaluer. Remplissez-la avant de signer. Un outil choisi la tête claire vaut bien plus qu'un outil acheté dans l'éblouissement.

## Points clés

- Vous n'achetez pas un outil, vous achetez un résultat — reliez chaque choix à un vrai problème et à un vrai chiffre.
- Une démo est une représentation sur des données propres ; un pilote sur vos propres données désordonnées est le seul test honnête.
- Le prix mensuel n'est qu'une fraction du coût — construisez toujours un total sur trois ans qui inclut les postes, l'usage, la mise en place, l'assistance et la sortie.
- L'open source est une voie réelle, abordable et sans enfermement, mais il échange de l'argent contre de l'effort et de la compétence ; choisissez-le quand vous avez l'aide pour le faire tourner.
- Refusez l'urgence : un bon outil survit à une semaine de réflexion attentive, et un fournisseur qui accueille un vrai pilote est confiant pour une bonne raison.

<!-- BEGIN agentbridge-examples -->

## Essayez avec AgentBridge

Voici à quoi ressemble le même travail avec AgentBridge. Chaque encadré montre le résultat fini et la seule ligne que vous tapez pour l'obtenir.

### Comparer des produits avant d'acheter

![Une comparaison de produits côte à côte](../../assets/examples/product-compare.png)
*Une comparaison de produits côte à côte*

**Ce que vous demandez :** `Compare ces deux imprimantes pour un petit bureau : prix, coût de fonctionnement et fiabilité.`

L'agent étudie les deux produits et dispose une comparaison claire pour que vous puissiez choisir la meilleure option selon votre budget et votre usage.

*Astuce : Demandez le coût total de possession, pas seulement le prix affiché.*

<!-- END agentbridge-examples -->
