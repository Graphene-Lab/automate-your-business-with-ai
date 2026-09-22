# Chapitre 19 — Connecter l'IA aux systèmes que vous utilisez déjà

## En mots simples

Votre entreprise tourne déjà sur des logiciels : le système qui suit vos clients, l'email auquel vous répondez, les tableurs dans lesquels vous vivez, le programme de comptabilité depuis lequel vous facturez. L'IA est la plus utile quand elle se branche sur ces systèmes existants au lieu de rester dans un coin à ne rien faire. Ce chapitre parle de cette connexion — comment l'IA parle aux outils que vous avez déjà.

L'idée clé est l'**intégration** : un lien qui laisse un logiciel passer des informations à un autre automatiquement. Quand votre IA peut lire votre liste de clients, rédiger une réponse dans votre boîte de réception, et écrire une note dans vos enregistrements, elle devient un vrai assistant. Quand elle ne peut se connecter à rien, c'est juste une fenêtre de chat intelligente dans laquelle vous devez copier-coller.

Une bonne analogie est la plomberie. Un nouveau filtre à eau est inutile s'il n'est pas connecté à vos tuyaux. La valeur vient de la connexion, pas du filtre seul. Les intégrations sont les tuyaux qui laissent l'IA couler dans votre travail quotidien. Votre travail est de comprendre quels tuyaux existent, lesquels vous pouvez connecter vous-même, et quand vous avez besoin d'un plombier.

Ce chapitre examine les systèmes courants auxquels l'IA se connecte — logiciels de gestion, CRM, email, tableurs. Il donne des exemples d'automatisations simples que vous pouvez vous représenter. Il explique ce qu'est une **API** en mots simples (c'est plus simple que ça n'en a l'air). Il vous dit quand vous pouvez le faire vous-même et quand appeler un technicien. Et il vous avertit des pièges : les dépendances qui vous bloquent, et la maintenance que chaque connexion exige.

La promesse : une IA connectée fait gagner du temps réel chaque jour. La mise en garde : une mauvaise connexion peut casser des choses ou vous piéger. Faites-le avec une carte et un plan.

## Un peu d'histoire

**Années 1960-1970 : des programmes qui se parlent.** Les premiers logiciels d'entreprise devaient échanger des données — un système de stock alimentant un système comptable. Les ingénieurs ont construit les premiers liens entre programmes, souvent à la main, en partageant des fichiers dans des formats convenus. L'intégration est née d'une pure nécessité.

**Années 1990 : l'intégration d'entreprise devient un métier.** Comme les entreprises faisaient tourner beaucoup de systèmes à la fois, les connecter est devenu un domaine entier. Des outils aux noms longs — intergiciels (middleware), intégration d'applications d'entreprise — essayaient d'être le carrefour central qui reliait tout. C'était puissant, cher, et demandait souvent des spécialistes.

**Années 2000 : l'économie de l'API.** Les logiciels ont commencé à exposer des portes propres et documentées pour que d'autres logiciels les utilisent. Ces portes s'appellent des API. D'un coup, une petite entreprise pouvait se connecter à de grands services — cartes, paiements, messagerie — sans les construire. Toute une économie de logiciels connectés est apparue.

**Années 2010 : le no-code et l'intégrateur citoyen.** Des outils comme Zapier et Make ont permis aux non-programmeurs de connecter des applications populaires en pointant et cliquant. Vous pouviez dire « quand un nouveau prospect arrive dans mon formulaire, ajoute-le à mon CRM et envoie-moi un email » sans écrire de code. L'« intégrateur citoyen » — une personne du métier qui construit ses propres connexions — est devenu réel.

**Années 2020 : l'IA comme nouveau connecteur.** Les outils d'IA ont acquis la capacité de lire, écrire et agir à travers les systèmes via leurs propres API. Maintenant l'IA peut être celle qui fait la connexion : lire votre boîte de réception, mettre à jour vos enregistrements, rédiger vos réponses. La plomberie est devenue plus intelligente, et le besoin de la comprendre a grandi tout aussi vite.

L'arc : des liens de fichiers construits à la main à un monde où le logiciel s'attend à être connecté. La connexion n'est plus un luxe ; c'est là que vit la valeur.

## Curiosité

### Le mémo qui a connecté le monde

En 2002, le PDG d'Amazon, Jeff Bezos, a envoyé un mémo interne devenu célèbre à ses équipes d'ingénierie. Les détails sont largement rapportés dans l'histoire de la tech. L'ordre central était net : désormais, chaque équipe doit partager ses données et ses fonctions via une interface propre et documentée — une API — et rien d'autre. Pas d'accès direct à la base de données d'une autre équipe. Pas de raccourcis par derrière. Si une équipe voulait quelque chose d'une autre équipe, elle devait le demander via l'interface publiée, ou le construire elle-même.

La raison n'était pas le rangement. C'était de rendre Amazon rapide et flexible. Quand chaque partie de l'entreprise pouvait être atteinte par une porte propre, les équipes pouvaient changer leurs propres systèmes sans casser celles des autres, et de nouveaux services pouvaient être construits vite par-dessus les anciens.

Cette discipline est largement créditée comme une fondation de ce qui est devenu **Amazon Web Services (AWS)** — la plateforme cloud qui propulse maintenant une énorme part d'internet. Une règle sur la façon dont un logiciel parle à un logiciel dans une seule entreprise est devenue l'un des plus grands business technologiques de la planète.

La leçon pour une petite entreprise est la même en miniature : **des connexions propres et documentées vous rendent flexibles ; des raccourcis désordonnés vous rendent fragiles.** Quand vous connectez l'IA à vos systèmes, construisez des liens propres, pas des bidouilles par derrière. Le tuyau soigné d'aujourd'hui est la liberté pour laquelle vous vous remercierez demain.

## Un exemple d'entreprise réel

*Ce qui suit est une composition illustrative de schémas courants du monde réel, pas une seule entreprise nommée.*

Une petite société de gestion immobilière tournait sur trois systèmes qui ne se parlaient pas : un CRM contenant les contacts des locataires, une boîte de réception partagée pour les demandes de maintenance, et un tableur suivant les travaux de réparation. Chaque demande signifiait recopier les détails à la main de la boîte de réception vers le tableur, puis vers le CRM. Le personnel passait des heures par jour sur du copier-coller, et des détails passaient entre les mailles.

Ils ont connecté les trois avec une simple automatisation. Quand un email de maintenance arrivait, une IA le lisait, extrayait le nom du locataire, la propriété et le problème, et créait une ligne dans le tableur automatiquement. Elle rédigeait aussi une réponse au locataire confirmant la demande. Un humain vérifiait le brouillon et appuyait sur envoyer. La note dans le CRM était ajoutée par la même automatisation.

Le résultat n'était pas de la magie — c'était de la plomberie. Les heures de copier-coller ont en grande partie disparu. Moins de demandes étaient perdues, parce que la même automatisation signalait pour un humain tout ce qu'elle ne pouvait pas lire clairement. La société n'a pas remplacé le personnel ; elle a retiré la partie ennuyeuse de leur journée pour qu'ils puissent gérer plus de propriétés sans plus de gens.

La leçon : la victoire est venue de connecter des systèmes qui existaient déjà, pas d'acheter quelque chose de neuf et de spectaculaire.

## Comment faire

### 19.1 Logiciels de gestion, CRM, email, tableurs

Ce sont les quatre systèmes que la plupart des entreprises font déjà tourner, et les quatre auxquels l'IA se connecte le plus souvent.

- **Logiciel de gestion (ERP).** Un système qui gère le cœur de votre entreprise — stock, commandes, production, finance. ERP signifie Enterprise Resource Planning (planification des ressources d'entreprise). L'IA peut lire des rapports dedans, signaler des chiffres inhabituels, ou rédiger des résumés.
- **CRM.** Signifie **Customer Relationship Management** (gestion de la relation client) — le système qui détient vos clients, vos prospects, et chaque interaction avec eux. L'IA peut rédiger des réponses aux prospects, journaliser les appels, et tirer l'historique d'un client pour vous aider à répondre plus vite.
- **Email.** La boîte de réception est où vit la plupart du travail des petites entreprises. L'IA peut trier, résumer et rédiger des réponses ici. C'est souvent la connexion la plus précieuse qui soit.
- **Tableurs.** L'outil universel. L'IA peut les remplir, les lire et les mettre à jour depuis d'autres sources.

Commencez là où la douleur est la plus forte. Pour la plupart des petites entreprises, ce sont l'email et le CRM. Connecter l'IA à ces deux-là donne le plus grand soulagement quotidien. N'essayez pas de tout connecter d'un coup — choisissez ce qui fait le plus mal et commencez là.

### 19.2 Exemples d'automatisations simples

Des exemples concrets aident à se représenter ce qui est possible. Chacune de celles-ci est une petite connexion courante :

- **Boîte de réception vers CRM.** Un nouvel email de demande crée automatiquement un prospect dans votre CRM, avec les coordonnées de l'expéditeur remplies.
- **Formulaire vers tableur.** Un client remplit un formulaire web ; les réponses atterrissent dans une ligne de tableur automatiquement, et l'IA étiquette la demande par type.
- **Email vers brouillon de réponse.** L'IA lit une demande standard et écrit un brouillon de réponse dans votre boîte de réception ; vous vérifiez et envoyez.
- **Document vers enregistrement.** L'IA lit un PDF de facture et écrit le montant, la date et le fournisseur dans votre système comptable.
- **Réunion vers notes.** L'IA transforme une réunion enregistrée en un résumé et des points d'action, puis les range là où votre équipe peut les voir.
- **Ticket vers alerte.** L'IA lit les messages de support entrants et signale en premier les en colère ou urgents à un humain.

Remarquez le schéma : l'IA lit depuis un endroit, fait quelque chose d'utile, et écrit dans un autre, avec une vérification humaine là où ça compte. C'est la forme de presque toute bonne automatisation.

### 19.3 Quand vous avez besoin d'un technicien

Vous pouvez faire une quantité surprenante vous-même avec des outils no-code. Mais certains travaux demandent un professionnel. Sachez lesquels.

**Vous pouvez probablement le faire vous-même** quand : les applications sont populaires (donc des connecteurs no-code existent), les données sont simples, l'automatisation est petite, et une erreur est peu coûteuse. Les outils de point-and-click couvrent beaucoup ici.

**Appelez un technicien quand :**

- **La connexion touche de l'argent, des registres juridiques, ou des données sensibles.** Une erreur ici est coûteuse ou dangereuse.
- **Les systèmes sont vieux ou sur mesure** et n'ont pas de connecteur prêt à l'emploi.
- **Vous avez besoin d'un lien fiable et toujours actif** qui ne doit pas échouer.
- **La sécurité est en jeu** — se connecter à des données clients signifie bien gérer le contrôle d'accès (voir [Chapitre 20 — Mettre en œuvre l'IA en sécurité](ch20-implementing-ai-securely.md)).
- **Vous ne comprenez pas ce que vous connectez.** Ne connectez jamais ce que vous ne pouvez pas expliquer.

Un technicien n'est pas un aveu d'échec. C'est le bon choix pour les parties risquées ou complexes, de même que vous appelez un plombier pour la canalisation principale et réparez le robinet vous-même.

### 19.4 Les API et les intégrations expliquées simplement

Une **API** sonne technique, mais l'idée est simple. Une API est un **menu qu'un logiciel offre à un autre.** C'est une liste de choses que vous êtes autorisé à lui demander de faire, et comment demander.

Pensez à une cuisine de restaurant. Vous n'entrez pas et ne commencez pas à cuisiner. Vous regardez le menu, commandez ce qui est proposé, et la cuisine l'apporte. Le menu est l'API. Il vous dit ce que vous pouvez demander (« obtenir les détails de ce client », « ajouter une nouvelle ligne », « envoyer cet email ») et comment le demander. Vous ne pouvez pas commander quelque chose hors du menu, et vous ne touchez jamais la cuisine directement.

Pourquoi c'est important pour l'IA : quand un système a une API, une IA peut utiliser ce menu pour lire et écrire des données de façon sûre et prévisible. Quand un système n'a pas d'API, s'y connecter est difficile ou impossible. Donc quand vous choisissez un logiciel, une bonne question est : **a-t-il une API ?** Si oui, l'IA peut probablement s'y connecter. Si non, vous êtes peut-être bloqué.

Une **intégration** est la connexion que vous construisez en utilisant une ou plusieurs API — l'acte de câbler le menu d'un système aux besoins d'un autre. L'API est la porte ; l'intégration est le couloir que vous construisez à travers elle.

Deux termes simples que vous entendrez :

- **Accès en lecture** — l'IA peut regarder les données mais pas les changer. Plus sûr.
- **Accès en écriture** — l'IA peut changer les données. Plus puissant, plus risqué. Donnez l'accès en écriture seulement là où vous en avez besoin.

### 19.5 Éviter les dépendances et les blocages

Chaque connexion crée une **dépendance** — une chose compte maintenant sur une autre. Les dépendances sont normales, mais trop, ou les mauvaises, peuvent vous bloquer.

Surveillez ces pièges :

- **Un point de défaillance unique.** Si une connexion casse et que tout votre workflow s'arrête, c'est un point unique fragile. Ayez un repli : une façon de le faire à la main si le lien meurt.
- **Une chaîne de dépendances.** Si A a besoin de B a besoin de C a besoin de D, un maillon cassé arrête tout. Gardez les chaînes courtes.
- **Une dépendance sur un outil qui peut disparaître.** Si vous vous connectez à un petit service qui ferme, votre automatisation meurt. Préférez des outils stables et établis.
- **L'enfermement (lock-in) par l'intégration.** Si tous vos systèmes sont câblés ensemble d'une façon qu'un seul vendeur comprend, partir devient dur. Gardez les connexions propres et documentées pour pouvoir recâbler plus tard. (L'enfermement est traité au [Chapitre 9 — Services tiers et IA fantôme](ch09-third-party-services-and-shadow-ai.md).)
- **Connexions non documentées.** Un lien dont personne ne sait comment il marche est une bombe à retardement. Documentez chaque connexion.

La règle : **construisez des connexions propres, courtes et documentées avec un repli manuel.** La leçon du mémo d'Amazon encore — des portes propres, pas de bidouilles par derrière.

### 19.6 Maintenance et mises à jour

Une connexion n'est pas « installer et oublier ». C'est une chose vivante qui demande des soins.

- **Les systèmes changent.** Votre CRM se met à jour, votre fournisseur d'email change un format, une API prend une nouvelle version. Quand un côté change, la connexion peut casser.
- **Défaillances silencieuses.** Une connexion peut cesser de marcher en silence, et les données cessent de couler sans que personne ne s'en aperçoive. Vérifiez que les données arrivent vraiment.
- **De nouveaux cas apparaissent.** L'automatisation gérait les cas courants ; un nouveau type de demande arrive et elle ne sait quoi en faire. Revoyez ce qui lui manque.
- **Mises à jour de sécurité.** Les connexions aux données ont besoin que leur accès soit revu avec le temps, surtout quand du personnel arrive ou part.

Planifiez la maintenance : désignez quelqu'un pour surveiller les connexions, les vérifier régulièrement, et réparer les cassures vite. Construisez une simple alerte — si aucune donnée ne coule pendant une journée, quelqu'un devrait le savoir. Un peu d'entretien empêche la plomberie d'inonder.

## Éthique et responsabilité

Connecter l'IA à vos systèmes signifie la connecter aux données de vraies personnes. Cela porte une responsabilité.

**Connectez avec consentement et soin.** Si l'IA va lire des emails ou des enregistrements clients, sachez ce que vous connectez et si c'est permis. Respectez les règles de vie privée (voir [Chapitre 10 — Vie privée et RGPD](ch10-privacy-and-gdpr.md)).

**Moindre accès.** Donnez à l'IA seulement l'accès dont elle a besoin. Si elle a seulement besoin de lire, ne lui donnez pas l'écriture. Si elle a seulement besoin d'un dossier, ne lui donnez pas tout le disque. Cela limite les dégâts si quelque chose tourne mal.

**Gardez un humain à l'envoi.** Pour tout ce qui atteint un client, un humain devrait vérifier avant que ça parte. Une automatisation qui agit seule sur des messages destinés au client peut causer un vrai tort.

**Documentez pour la redevabilité.** Quand quelque chose tourne mal, vous devez savoir ce que l'automatisation a fait et pourquoi. Une connexion documentée est une connexion redevable.

**Ne connectez pas ce que vous ne pouvez pas expliquer.** Si vous ne pouvez pas dire en mots simples ce qu'une connexion fait aux données de qui, vous ne devriez pas la construire. Une complexité que vous ne comprenez pas est un risque que vous ne contrôlez pas.

Construisez les connexions comme vous voudriez que vos propres données soient traitées.

## Erreurs à éviter

**Tout connecter d'un coup.** Essayer de câbler chaque système dès le premier jour. Choisissez ce qui fait le plus mal et commencez là.

**Pas de carte.** Connecter sans savoir ce que vous avez et comment ça se relie. Dessinez la carte d'abord.

**Bidouilles par derrière.** Raccourcis rapides et non documentés qui cassent plus tard et vous piègent. Construisez des portes propres à la place.

**Trop d'accès.** Donner à l'IA un accès en écriture à tout quand elle n'a besoin que d'en lire une seule chose. Utilisez le moindre accès.

**Pas de repli.** Une connexion qui, quand elle casse, arrête tout le workflow sans plan manuel. Ayez toujours un repli.

**Ignorer les défaillances silencieuses.** Présumer que la connexion marche parce que personne ne s'est plaint. Vérifiez que les données arrivent vraiment.

**Pas de plan de maintenance.** Câbler et s'en aller. Les connexions demandent des soins.

**Se connecter à un outil qui peut disparaître.** Construire sur un service branlant qui peut disparaître. Préférez des outils stables.

**Laisser l'IA agir seule sur les messages clients.** Pas de vérification humaine sur ce qui atteint un client. Gardez un humain à l'envoi.

**Liens non documentés.** Personne ne sait comment la connexion marche. Documentez-les tous.

**Oublier les changements de personnel.** Ne pas mettre à jour les accès quand des gens arrivent ou partent. Revoyez les accès régulièrement.

## Exercice pratique

### 19.7 Exercice : une carte des systèmes de votre entreprise

Vous ne pouvez pas connecter ce que vous ne voyez pas. Dessinez une carte des systèmes sur lesquels votre entreprise tourne.

**Étape 1 — Listez chaque système.** Écrivez chaque logiciel que votre entreprise utilise quotidiennement : CRM, email, comptabilité, tableurs, stock, planification, formulaires du site web, outils de chat. N'en laissez aucun dehors.

**Étape 2 — Pour chacun, notez quatre choses :**

- **Ce qu'il détient** (quelles données y vivent).
- **Qui l'utilise** (quelles personnes ou rôles).
- **A-t-il une API ?** (Vérifiez le site du vendeur ou demandez ; marquez oui / non / inconnu.)
- **À quel point les données sont sensibles ?** (Faible / moyen / élevé.)

**Étape 3 — Dessinez les liens actuels.** Sur papier, dessinez des lignes entre les systèmes qui échangent déjà des données aujourd'hui, même si un humain les porte par copier-coller. Marquez quels liens sont manuels.

**Étape 4 — Repérez la douleur.** Entourez les liens manuels qui dévorent le plus de temps ou causent le plus d'erreurs. Ce sont vos meilleurs candidats à l'automatisation.

**Étape 5 — Marquez le risque.** Pour chaque candidat, notez la sensibilité. Les liens à haute sensibilité demandent un technicien et une vérification humaine ; les liens à basse sensibilité, vous pouvez les essayer vous-même.

**Étape 6 — Choisissez un.** Choisissez le seul lien à plus forte douleur et plus faible risque comme première intégration. Menez-le en pilote (voir [Chapitre 18 — Votre premier projet pilote](ch18-your-first-pilot-project.md)).

Gardez la carte sur une page. Mettez-la à jour au fil des changements de systèmes. La carte est votre plan et votre défense contre connecter à l'aveugle.

## Checklist

### 19.8 Checklist d'intégration

Avant de connecter l'IA à un système, et après, cochez chaque case.

- [ ] **J'ai une carte de tous mes systèmes et de ce que chaque système détient.**
- [ ] **Je sais quels systèmes ont une API et lesquels n'en ont pas.**
- [ ] **Je sais à quel point les données dans chaque système sont sensibles.**
- [ ] **J'ai choisi le lien à plus forte douleur et plus faible risque à connecter en premier.**
- [ ] **J'ai utilisé une connexion propre et documentée, pas une bidouille par derrière.**
- [ ] **J'ai donné à l'IA seulement l'accès dont elle a besoin (moindre accès).**
- [ ] **Je connais la différence entre accès en lecture et en écriture et je n'ai utilisé l'écriture que là où nécessaire.**
- [ ] **Un humain vérifie tout ce qui atteint un client.**
- [ ] **J'ai un repli manuel si la connexion casse.**
- [ ] **J'ai vérifié que la connexion est stable et pas un point de défaillance unique.**
- [ ] **J'ai construit un moyen de détecter les défaillances silencieuses (alerte si aucune donnée ne coule).**
- [ ] **J'ai documenté comment la connexion marche et qui la maintient.**
- [ ] **J'ai désigné quelqu'un pour maintenir et surveiller la connexion.**
- [ ] **J'ai revu les accès pour le personnel actuel et je les reverrai quand le personnel change.**
- [ ] **J'ai fait tourner la connexion en pilote avant de lui faire pleinement confiance.**

Si une case est vide, la connexion n'est pas prête. Remplissez-la d'abord. Une IA connectée est un assistant puissant ; une IA connectée à l'aveugle est une responsabilité.

## Points clés à retenir

- La valeur de l'IA vient de se connecter aux systèmes que vous faites déjà tourner — la connexion est la plomberie, et la valeur coule à travers elle.
- Une API est simplement un menu qu'un logiciel offre à un autre ; si un système a une API, l'IA peut probablement s'y connecter, alors demandez « a-t-il une API ? » quand vous choisissez un logiciel.
- Utilisez le moindre accès — donnez à l'IA seulement ce dont elle a besoin, préférez la lecture à l'écriture, et gardez un humain sur tout ce qui atteint un client.
- Construisez des connexions propres, courtes et documentées avec un repli manuel ; les bidouilles par derrière et les défaillances silencieuses sont les pièges qui vous cassent.
- Les connexions sont des choses vivantes qui demandent maintenance, surveillance et revues d'accès — mettez-les en place et ne vous en allez jamais.

<!-- BEGIN agentbridge-examples -->

## Essayez avec AgentBridge

Voici à quoi ressemble le même travail avec AgentBridge. Chaque encadré montre le résultat fini et la seule ligne que vous tapez pour l'obtenir.

### Vérifier un fournisseur avant de s'engager

![Une synthèse de diligence raisonnable d'un fournisseur](../../assets/examples/due-diligence.png)
*Une synthèse de diligence raisonnable d'un fournisseur*

**Ce que vous demandez :** `Étudie ce fournisseur et dis-moi sa réputation, depuis combien de temps il existe, et tout signal d'alerte.`

L'agent rassemble ce qui est publiquement disponible et vous donne une image équilibrée avec des sources, pour que vous décidiez les yeux ouverts.

*Astuce : Demandez-lui de lister ce qu'il n'a pas pu trouver, pour savoir où creuser davantage.*

---

### Vérifier une commande dans votre système

![Un statut de commande tiré du système de gestion](../../assets/examples/order-status.png)
*Un statut de commande tiré du système de gestion*

**Ce que vous demandez :** `Quel est le statut de la commande 4821 ?`

L'agent consulte la commande dans votre système connecté et vous donne son statut en mots simples — sans chercher dans les menus.

*Astuce : Cela fonctionne une fois votre système de gestion connecté. Voir le chapitre connexion du livre.*

---

### Le même assistant dans votre navigateur

![Le chat web d'AgentBridge dans une fenêtre de navigateur](../../assets/examples/web-chat.png)
*Le chat web d'AgentBridge dans une fenêtre de navigateur*

**Ce que vous demandez :** `(browser) Rédige un mot de remerciement à nos clients fidèles.`

Ouvrez l'adresse web et discutez dans le navigateur. Mêmes outils, mêmes documents, même mémoire — juste une fenêtre différente.

*Astuce : Pratique quand vous êtes sur une machine différente mais voulez quand même votre propre assistant.*

---

### Le brancher sur vos propres outils

![L'API HTTP laisse d'autres programmes utiliser l'assistant](../../assets/examples/http-api.png)
*L'API HTTP laisse d'autres programmes utiliser l'assistant*

**Ce que vous demandez :** `POST /v1/chat/completions  { "model": "default-agent", "messages": [...] }`

Vos propres programmes peuvent appeler l'assistant via une API web standard, comme ils appelleraient n'importe quel service en ligne. Une intégration, beaucoup d'usages.

*Astuce : C'est pour l'étape technique — le chapitre connexion du livre vous y guide.*

---

### Connecter d'autres outils IA à lui

![AgentBridge connecté à d'autres outils IA via MCP](../../assets/examples/mcp-connector.png)
*AgentBridge connecté à d'autres outils IA via MCP*

**Ce que vous demandez :** `(MCP) Connecte AgentBridge comme serveur d'outils.`

D'autres applications IA peuvent utiliser les outils d'AgentBridge via le standard MCP, si bien que toute votre boîte à outils travaille ensemble.

*Astuce : MCP est pour connecter des outils ; pour un usage quotidien, le chat suffit.*

<!-- END agentbridge-examples -->
