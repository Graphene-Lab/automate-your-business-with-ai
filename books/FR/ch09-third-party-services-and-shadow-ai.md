# Chapitre 9 — Services tiers et IA fantôme

## En mots simples

Un service d'IA tiers, c'est toute IA que vous utilisez et qui tourne sur les ordinateurs de quelqu'un d'autre. Vous tapez une question ou envoyez un fichier. Cela voyage sur internet jusqu'à leurs machines. Leur logiciel fait le travail. La réponse revient. Vous ne voyez jamais ce qu'il y a à l'intérieur.

C'est la façon normale dont la plupart des entreprises utilisent l'IA aujourd'hui. C'est facile, c'est peu cher au départ, et c'est puissant. C'est pour ça que presque tout le monde l'utilise.

Mais cela a un coût caché. Dès que votre texte quitte votre bâtiment, vous en perdez le contrôle direct. Vous dépendez désormais d'une entreprise que vous n'avez pas conçue, de règles que vous n'avez pas écrites, d'un serveur que vous ne pouvez pas inspecter.

L'« IA fantôme » est la seconde moitié de cette histoire. IA fantôme signifie que des employés utilisent des outils d'IA sans que l'entreprise le sache, l'approuve ou le surveille. Une assistante marketing colle une liste de clients dans un chatbot gratuit. Un comptable dépose une facture dans une application web pour la résumer. Personne aux commandes ne sait que cela se passe. Les données sont parties, et il n'y a ni trace, ni contrat, ni contrôle.

Pensez à l'imprimante de bureau il y a vingt ans. Tout le monde l'utilisait. Personne ne savait qu'elle gardait une copie de chaque page. L'IA fantôme, c'est la même surprise, sauf que les pages sont vos listes de clients, vos contrats et vos prix.

Ce chapitre porte sur deux choses : ce qui arrive réellement à vos données quand vous utilisez un service tiers, et comment empêcher votre propre personnel de créer en silence des risques. Le schéma opposé — faire tourner l'IA sur vos propres machines — est traité au [Chapitre 8](ch08-self-hosting-keep-your-data-under-control.md). Le volet juridique des données personnelles est le sujet central du [Chapitre 10](ch10-privacy-and-gdpr.md). La question plus large de contrôler vos propres outils est au [Chapitre 11](ch11-digital-sovereignty.md).

## Un peu d'histoire

**Années 1990 à 2000 : le logiciel quitte l'étagère.** Avant, vous achetiez un programme sur un CD et vous le faisiez tourner sur votre propre ordinateur. Puis l'email, les agendas et le stockage de fichiers sont passés sur internet. Vous avez cessé de posséder le logiciel et avez commencé à louer un accès à celui-ci.

**Années 2000 à 2015 : le SaaS devient normal.** Le « logiciel en tant que service » signifiait payer un abonnement mensuel pour utiliser le logiciel de quelqu'un d'autre sur le web. Salesforce, Google Workspace et Microsoft 365 l'ont rendu ordinaire. La commodité a gagné. La plupart des petites entreprises ont cessé de faire tourner leurs propres serveurs.

**2016 à 2022 : les données partent avec le logiciel.** Une fois vos fiches clients, vos documents et vos messages hébergés dans le cloud d'un fournisseur, vos données d'entreprise étaient définitivement hors de vos murs. La plupart des gens l'ont accepté parce que les outils étaient bons et le prix bas.

**Novembre 2022 : ChatGPT ouvre la porte à tout le monde.** Une IA puissante est devenue disponible dans une simple boîte web gratuite. Vous n'aviez plus besoin d'un contrat fournisseur pour utiliser l'IA. Il ne fallait plus qu'une adresse email. C'est le moment où l'IA fantôme a commencé, car un seul employé pouvait désormais envoyer des données de l'entreprise à un modèle de pointe sans demander à personne.

**2023 : les premières alertes en entreprise.** Des entreprises ont découvert que leur personnel collait des documents confidentiels dans des chatbots publics. L'affaire Samsung, dans la section Curiosité, est la plus célèbre. Plusieurs banques et cabinets professionnels ont interdit ou restreint les outils d'IA publics cette année-là.

**2023 à 2026 : les fournisseurs ajoutent des offres « entreprise ».** En réponse, les fournisseurs d'IA ont vendu des formules professionnelles promettant de ne pas s'entraîner sur vos données, de garder les données séparées et d'ajouter des contrôles d'administration. La commodité est restée ; les promesses se sont améliorées. Mais une promesse n'est pas un contrôle, et c'est pourquoi ce chapitre compte.

## Curiosité

### 9.7 Le fabricant de semi-conducteurs qui a collé ses secrets dans ChatGPT

Début 2023, Samsung Electronics — l'une des plus grandes entreprises technologiques au monde — a découvert que ses propres ingénieurs avaient mis des documents confidentiels dans un chatbot IA public.

Les informations, publiées d'abord par le quotidien financier coréen *Korea Economic Daily* en avril 2023 et largement reprises ensuite, décrivaient trois incidents distincts au sein de la division semi-conducteurs. Dans le premier, un ingénieur a collé du code source défectueux d'un programme servant à télécharger des données de mesure depuis une usine de puces, espérant que le chatbot trouverait le bug. Dans le second, du personnel a téléversé du code lié aux équipements de semi-conducteurs et à la détection de défauts. Dans le troisième, des employés ont soumis des transcriptions d'enregistrements de réunions à l'outil pour obtenir des résumés. Tout cela s'est produit en à peu près trois semaines après que la division a autorisé l'accès à l'outil.

Une fois les données dans le chatbot, elles se trouvaient sur des machines que Samsung ne possédait pas. L'entreprise ne pouvait pas facilement les récupérer, et ne pouvait pas être sûre qu'elles ne seraient pas utilisées ou vues par d'autres.

La réponse de Samsung a été sans détour. Elle a interdit les outils d'IA générative, dont ChatGPT, sur les ordinateurs, tablettes et téléphones de l'entreprise ainsi que sur son réseau interne. Enfreindre la règle pouvait entraîner des sanctions disciplinaires allant jusqu'au licenciement. Il a été demandé aux employés utilisant de tels outils sur des appareils personnels de ne jamais soumettre d'informations de l'entreprise ni de données personnelles pouvant révéler la propriété intellectuelle de Samsung. Un sondage interne a révélé que 65 % des personnes interrogées estimaient que les services d'IA représentaient un risque pour la sécurité. Dans le même temps, Samsung a dit construire ses propres outils d'IA internes pour la traduction, le résumé de documents et le développement logiciel, et travailler à bloquer l'envoi d'informations sensibles vers des services extérieurs.

La leçon n'est pas que Samsung a été négligent. C'est que si une entreprise disposant de milliards en budget de sécurité a été prise au dépourvu par un chatbot gratuit, une petite entreprise sans équipe de sécurité est encore moins protégée. La commodité est réelle, et la fuite aussi.

## Un exemple d'entreprise réel

### L'agence qui a perdu sa liste de clients deux fois

Prenons une petite agence de marketing, vingt personnes, pas de service informatique. C'est une histoire composite, mais chaque partie arrive chaque semaine dans de vraies entreprises.

Première fuite : une directrice de compte senior veut réécrire rapidement une proposition. Elle ouvre un chatbot IA gratuit sur son ordinateur portable et colle le brouillon, qui contient le nom d'un produit non encore lancé chez un client, des chiffres de budget et des coordonnées. Elle obtient un plus joli paragraphe. Elle ne pense jamais à l'endroit où le texte est allé.

Deuxième fuite : la même directrice, un mois plus tard, s'inscrit à un « assistant de rédaction IA » payant qui promet de meilleurs résultats. Pour le configurer, elle le connecte à l'email et au disque partagé de l'agence afin qu'il « apprenne la voix de l'entreprise ». Désormais, le fournisseur peut tout lire : chaque client, chaque contrat, chaque blague interne qui se transforme en note stratégique.

Puis le problème de l'évolution arrive. Un an plus tard, le fournisseur change son offre. Les fonctionnalités qu'elle payait passent dans une formule supérieure. Le prix double. Le modèle derrière l'outil est remplacé par un plus récent, et le style d'écriture sur lequel elle avait formé son équipe change en silence. Elle veut partir, mais tout est branché sur cet outil. Changer veut dire reconnecter toute l'agence ailleurs et tout le monde reformer. C'est l'enfermement, et c'est arrivé sans une seule mauvaise décision — seulement une série de décisions commodes.

Rien de tout cela n'a exigé de la malveillance. Il a fallu la commodité et l'absence d'une règle. La solution n'est pas de craindre l'IA. C'est de décider, à l'avance, quelles données peuvent aller où, et de donner aux gens un bon outil pour qu'ils n'aillent pas en chercher un risqué.

## Comment faire

### 9.1 La commodité des services cloud : pourquoi tout le monde les utilise

L'IA tierce est populaire pour des raisons honnêtes, et vous devriez les nommer avant de plaider contre elle.

Il n'y a aucune installation. Vous n'achetez pas de matériel, n'embauchez pas d'ingénieur, n'installez rien. Vous ouvrez une page web et vous commencez. Pour une petite entreprise sans personnel technique, c'est tout l'attrait.

Il n'y a pas de coût initial. La plupart des outils ont une formule gratuite ou un faible abonnement mensuel. Vous pouvez essayer une idée pour le prix d'un café au lieu d'un investissement en capital.

La qualité est élevée. Les meilleurs modèles du monde se trouvent derrière ces services. Une entreprise de deux personnes peut utiliser la même capacité qu'une grande société.

Cela monte en charge instantanément. Besoin de dix fois plus de travail aujourd'hui ? Les machines du fournisseur l'absorbent. Vous ne faites rien.

C'est pour cela que l'IA cloud s'est répandue plus vite que toute technologie avant elle. Le but de ce chapitre n'est pas de vous retirer tout cela. C'est de vous la faire utiliser les yeux ouverts, car chacune de ces commodités s'achète avec un morceau de contrôle que vous ne vous êtes pas vu vendre.

### 9.2 Ce qui arrive à vos données quand elles quittent l'entreprise

Quand vous collez du texte dans une IA tierce, plusieurs choses peuvent se passer, et vous ne pouvez généralement pas voir lesquelles.

Vos données traversent internet vers les serveurs du fournisseur, souvent dans un autre pays. Une fois là-bas, elles sont stockées, au moins un moment, sur un matériel que vous ne contrôlez pas et ne pouvez pas inspecter.

Elles peuvent être lues par des systèmes automatisés pour un filtrage de sécurité. Elles peuvent être journalisées pour le débogage. Du personnel de support dans un autre pays peut les voir. Rien de tout cela n'est inhabituel ; c'est ainsi que fonctionnent les grands services.

Surtout, elles peuvent être utilisées pour entraîner le modèle du fournisseur. « Entraîner » signifie que l'entreprise nourrit son système avec votre texte pour que le modèle apprenne de celui-ci. Si cela arrive, un fragment de votre texte confidentiel peut façonner les réponses données à d'autres clients. C'est la raison numéro un d'être prudent.

Certaines formules professionnelles promettent de ne pas s'entraîner sur vos données. Cette promesse a de la valeur, mais c'est une clause de contrat, pas un mur. Vous faites confiance au fournisseur pour l'honorer sur chaque produit et dans chaque pays. La règle sûre est simple : traitez toute IA tierce comme si tout ce que vous envoyiez pouvait devenir public. Si cette idée est inacceptable pour un fichier donné, n'envoyez pas ce fichier.

### 9.3 Le problème de la transparence : vous ne savez jamais vraiment comment vos données sont utilisées

Vous ne pouvez pas voir à l'intérieur d'un service d'IA tiers. C'est le problème central, et il ne va pas disparaître.

Vous ne savez pas quel modèle vous a répondu. Les fournisseurs échangent les modèles sans vous le dire. Vous ne savez pas où vos données ont été stockées, qui pouvait y accéder, ni combien de temps elles ont été gardées. Vous ne savez pas si un sous-traitant dans un autre pays les a traitées. Vous ne savez pas si elles ont servi à l'entraînement, même quand vous croyez que non.

La politique de confidentialité du fournisseur est écrite par des avocats, pas par des ingénieurs, et elle décrit ce qu'ils *peuvent* faire, pas ce qu'ils *feront* dans votre cas précis. La lire donne rarement une réponse claire.

C'est pourquoi le test pratique est si utile. Au lieu d'essayer de comprendre le système, posez une seule question sur les données : *serait-ce acceptable si cela devenait public demain ?* Pour un article de blog public, oui. Pour le fichier des salaires d'un client, non. Ce seul test remplace mille questions auxquelles vous ne pouvez pas répondre.

Si vous avez besoin d'une vraie transparence, la seule source honnête est un système que vous pouvez inspecter — votre propre machine, ou un logiciel ouvert que quelqu'un peut auditer. C'est le sujet du [Chapitre 8](ch08-self-hosting-keep-your-data-under-control.md) et du [Chapitre 11](ch11-digital-sovereignty.md).

### 9.4 Le problème de l'évolution : les modèles changent, les contrats changent, les prix changent

Un service tiers n'est pas une chose que vous achetez ; c'est une relation qui continue de changer sous vos pieds.

Le modèle change. L'outil d'aujourd'hui tournera peut-être sur un autre modèle le trimestre prochain. Les réponses changent. Le style change. Quelque chose qui marchait bien dans votre flux de travail peut empirer, ou simplement devenir différent, sans avertissement et sans moyen de rester sur l'ancienne version.

Le contrat change. Les conditions acceptées à l'inscription peuvent être mises à jour. Des fonctionnalités sur lesquelles vous comptiez peuvent passer derrière une formule plus chère. La promesse sur les données d'entraînement peut être reformulée.

Le prix change. Un outil bon marché que vous avez désormais branché sur votre entreprise peut augmenter son prix, et vous faites face à un choix douloureux : payer plus, ou tout arracher.

C'est le risque caché de la commodité. Vous construisez sur un terrain que quelqu'un d'autre contrôle, et il peut déplacer le terrain quand il veut. La défense est de garder vos données importantes et vos flux de travail essentiels portables, et de ne jamais laisser un seul fournisseur devenir le seul endroit où votre travail peut se faire.

### 9.5 L'enfermement : à quel point il est difficile de changer de fournisseur plus tard

L'enfermement signifie que quitter un fournisseur coûte tellement cher, en temps, en argent ou en perturbation, que vous ne pouvez pas raisonnablement le faire. Vous êtes « enfermé ».

Cela arrive de trois façons. **Enfermement des données :** vos données sont stockées dans un format que seul ce fournisseur lit bien, ou vous ne pouvez pas les exporter proprement. **Enfermement du flux de travail :** votre processus quotidien est construit autour de cet outil, donc changer veut dire reformer tout le monde et reconstruire les modèles. **Enfermement de l'intégration :** l'outil est connecté à votre email, votre CRM, vos fichiers, et le retirer casse tous ces liens.

L'enfermement donne du pouvoir au fournisseur sur vous. Il sait que partir est difficile, ce qui affaiblit votre position quand il augmente les prix ou change les conditions.

Pour rester libre, exigez trois choses dès le départ. D'abord, vos données doivent être exportables dans un format simple et courant. Ensuite, gardez vos données principales quelque part où vous les contrôlez, et laissez le fournisseur travailler sur une copie. Enfin, concevez votre flux de travail pour que l'IA soit une étape, pas toute la machine, afin de pouvoir échanger l'étape. Le but n'est pas d'éviter les fournisseurs. C'est de pouvoir en quitter un en une semaine, pas en un an.

### 9.6 L'IA fantôme : quand les employés utilisent des outils non autorisés

L'IA fantôme est le risque que vous ne pouvez pas voir, car il est créé par votre propre personnel de confiance.

Cela arrive parce que les bons outils officiels sont lents à approuver, alors que les outils gratuits risqués sont instantanés. Un employé sous pression de temps colle un email client dans un chatbot gratuit pour rédiger une réponse. Personne ne l'en empêche, parce que personne ne le sait.

Pourquoi c'est dangereux : les données partent sans contrat, sans examen et sans trace. Vous ne pouvez pas le dire au client, vous ne pouvez pas retrouver les données plus tard, et vous ne pouvez pas prouver ce qui s'est passé. Si l'outil s'entraîne sur ces données, vos informations confidentielles peuvent finir par façonner un modèle public.

Comment le repérer : des facturations inhabituelles sur les cartes de l'entreprise pour des abonnements d'IA ; du personnel qui se plaint que les outils approuvés sont trop lents ; des améliorations « magiques » soudaines dans les résultats qu'aucun outil approuvé n'explique.

Comment l'arrêter : ne faites pas que bannir. Une interdiction sans bonne alternative ne fait que pousser le comportement dans la clandestinité. Donnez aux gens un outil approuvé qui est rapide et assez bon, et ils l'utiliseront. Puis rendez la règle claire, formez dessus, et surveillez légèrement. Le volet politique complet est à la section 9.8 et dans les modèles de politique d'IA d'entreprise en annexes du livre.

### 9.8 Comment atténuer les risques : diligence raisonnable, contrats, politique interne

Vous réduisez le risque avec trois couches. Faites les trois.

**Couche 1 : Diligence raisonnable — vérifiez avant d'acheter.**
Avant d'adopter un fournisseur d'IA, posez les questions qui fâchent. Où les données sont-elles stockées, et dans quels pays ? Vous entraînez-vous sur les données clients, et pouvez-vous garantir par écrit que non ? Qui peut y accéder, y compris les sous-traitants ? Combien de temps sont-elles gardées, et comment sont-elles supprimées ? Sont-elles chiffrées en transit et au repos ? Quelles certifications détenez-vous ? Obtenez les réponses par écrit, pas dans un appel commercial. Un fournisseur qui ne peut pas répondre clairement vous dit quelque chose. Une version notée de ces questions se trouve dans la grille d'évaluation de diligence fournisseur en annexes.

**Couche 2 : Contrats — mettez les promesses sur le papier.**
Une assurance verbale ne vaut rien. Dans le contrat, exigez : pas d'entraînement sur vos données ; la résidence des données dans un pays que vous acceptez ; le droit d'exporter toutes vos données dans un format utilisable ; le droit à la suppression ; l'obligation de vous informer des violations et des changements majeurs de modèle ou de conditions ; et des limites sur les sous-traitants. Si le fournisseur ne signe pas ces clauses, c'est votre réponse.

**Couche 3 : Politique interne — dites à vos gens les règles.**
Écrivez une politique d'IA courte et simple. Dites quels outils sont approuvés. Dites quelles données ne doivent jamais entrer dans une IA externe — données personnelles des clients, dossiers financiers, contrats, code source, mots de passe. Donnez au personnel un outil approuvé rapide pour qu'il n'aille pas en chercher un risqué. Formez tout le monde à la règle en une courte session. Revoyez la liste des outils approuvés chaque trimestre. Un modèle se trouve en annexes.

L'ordre compte. Vérifiez d'abord, contractez ensuite, politique en troisième. La plupart des entreprises sautent les deux premières et se demandent pourquoi elles se sont exposées.

## Éthique et responsabilité

L'IA tierce soulève un devoir que vous devez à deux groupes : les personnes dont vous détenez les données, et votre propre personnel.

**À vos clients et vos employés.** Quand un client vous donne des données personnelles, il vous fait confiance pour les protéger. Envoyer ces données à une IA tierce que vous n'avez pas vérifiée peut briser cette confiance, même s'il n'arrive rien de mauvais. Vous êtes responsable de l'endroit où vont leurs données. Les obligations légales sont exposées au [Chapitre 10](ch10-privacy-and-gdpr.md) ; le principe éthique est simple — ne mettez pas les informations privées de quelqu'un quelque part où vous ne mettriez pas les vôtres.

**À votre personnel, à propos de l'IA fantôme.** Attention à ne pas transformer la protection en surveillance. Si vous surveillez l'usage de l'IA, dites aux gens ce que vous surveillez et pourquoi. Une règle claire plus un bon outil, c'est juste. Une surveillance secrète d'un personnel de confiance abîme le moral et la confiance. Visez des garde-fous, pas un État policier.

**Soyez honnête sur ce que vous ne contrôlez pas.** Si un client demande si ses données entraînent un modèle externe, vous devriez pouvoir répondre honnêtement. Si vous ne savez pas, dites-le, et corrigez la situation. Surréserver la sécurité est pire que d'admettre une faille.

## Erreurs à éviter

1. **Regarder la démo, pas le flux de données.** Une démo léchée ne vous dit rien sur l'endroit où vont vos données. Posez d'abord les questions de stockage et d'entraînement.
2. **Faire confiance à un « on ne s'entraîne pas sur vos données » verbal.** Si ce n'est pas dans le contrat, cela n'existe pas.
3. **Connecter un outil à tout votre disque.** « Apprendre notre voix » signifie souvent « tout lire ». Donnez à l'outil le strict nécessaire.
4. **Bannir l'IA fantôme sans alternative.** Une interdiction sans bon outil approuvé ne fait que cacher le comportement.
5. **Pas de politique écrite.** Si la règle n'est pas écrite et enseignée, ce n'est pas une règle.
6. **Ignorer la question du pays.** Des données stockées sous un système juridique différent peuvent être consultées différemment. Sachez où elles se trouvent.
7. **Supposer qu'une formule payante égale sécurité.** Une formule grand public payante n'est pas la même chose qu'une formule entreprise contractuelle avec les bonnes conditions.
8. **Pas de plan d'export.** Si vous ne pouvez pas faire sortir vos données, vous êtes enfermé dès le premier jour.
9. **Traiter la politique de confidentialité comme une garantie.** Elle énumère ce qu'ils *peuvent* faire, pas ce qu'ils feront pour vous.
10. **Oublier l'humain.** La fuite commence presque toujours par une personne sous pression de temps. Corrigez la pression et donnez un chemin sûr.

## Exercice pratique

### 9.9 Analysez vos fournisseurs d'IA actuels

Prenez une heure et faites cela pour chaque outil d'IA que votre entreprise utilise aujourd'hui, y compris ceux que le personnel utilise en silence.

Faites un tableau. Une ligne par outil. Colonnes :

- **Nom de l'outil** et qui l'a activé.
- **Quelles données entrent.** Soyez précis : emails clients, factures, contrats, code, texte public.
- **Où c'est stocké,** si vous le savez. Si inconnu, écrivez « inconnu ».
- **S'entraînent-ils sur nos données ?** Oui / Non / Inconnu.
- **Y a-t-il un contrat,** ou juste une case à cocher en ligne ?
- **Pouvons-nous exporter nos données ?** Oui / Non / Inconnu.
- **Niveau de risque** pour les données que vous y mettez réellement : Faible / Moyen / Élevé.

Lisez maintenant les lignes à risque Élevé. Pour chacune, demandez-vous : serait-il acceptable que ces données deviennent publiques ? Si non, vous avez trois choix — arrêter d'y mettre ces données, passer à un fournisseur qui signe les bonnes conditions, ou déplacer cette tâche vers un outil que vous contrôlez (voir [Chapitre 8](ch08-self-hosting-keep-your-data-under-control.md)).

Enfin, faites le tour. Envoyez un message honnête à votre équipe : « Quels outils d'IA utilisez-vous pour le travail dont nous n'avons pas parlé ? » Les réponses sont votre vraie liste d'IA fantôme. Ne punissez pas l'honnêteté ; corrigez les failles qu'elle révèle.

## Liste de contrôle

### 9.10 Questions à poser à chaque fournisseur d'IA

Avant de mettre de vraies données dans un service d'IA tiers, obtenez une réponse écrite à chacune de ces questions.

- [ ] **Où nos données sont-elles physiquement stockées,** et dans quels pays ?
- [ ] **Entraînez-vous vos modèles sur nos données ?** Pouvez-vous vous engager sur « non » dans le contrat ?
- [ ] **Qui peut accéder à nos données,** y compris les employés et les sous-traitants, et depuis où ?
- [ ] **Combien de temps gardez-vous nos données,** et comment obtenons-nous leur suppression ?
- [ ] **Nos données sont-elles chiffrées** à la fois en transit et au repos ?
- [ ] **Pouvons-nous exporter toutes nos données** à tout moment, dans un format courant et utilisable ?
- [ ] **Nous informerez-vous** en cas de violation de données, et sous quel délai ?
- [ ] **Nous préviendrez-vous** avant de changer le modèle, le prix ou les conditions ?
- [ ] **Quelles certifications de sécurité** détenez-vous, et pouvez-vous les montrer ?
- [ ] **Y a-t-il des sous-traitants,** et sont-ils liés par les mêmes conditions ?
- [ ] **Quel est notre recours légal** si vous abusez de nos données ?
- [ ] **Y a-t-il une console d'administration** pour que nous puissions voir et contrôler l'usage ?

Si un fournisseur ne peut pas répondre clairement et par écrit à ces questions, traitez l'outil comme à risque élevé et gardez les données sensibles hors de lui.

## Points à retenir

- Un service d'IA tiers tourne sur les ordinateurs de quelqu'un d'autre, donc dès que vos données partent, vous échangez le contrôle contre la commodité.
- Le plus grand risque est que vos données confidentielles puissent servir à entraîner un modèle qui sert d'autres personnes, et vous ne pouvez souvent ni le voir ni l'empêcher.
- Les fournisseurs changent de modèles, de contrats et de prix sous vos pieds, et l'enfermement rend le départ coûteux — gardez donc vos données exportables et votre flux de travail interchangeable.
- L'IA fantôme, c'est votre propre personnel utilisant des outils non approuvés ; arrêtez-la avec un bon outil approuvé plus une règle écrite claire, pas avec des interdictions seules.
- Protégez-vous en trois couches : vérifiez d'abord le fournisseur, mettez ensuite les promesses dans un contrat, et définissez en troisième une politique interne.
