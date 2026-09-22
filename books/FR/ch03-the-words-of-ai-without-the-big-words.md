# Chapitre 3 — Les mots de l'IA, sans les gros mots

## En mots simples

La plupart des mauvaises décisions en IA ne viennent pas d'une mauvaise technologie. Elles viennent de mots que personne ne s'est arrêté à définir.

Un vendeur dit : « notre plateforme d'IA s'intègre à vos systèmes via une API low-code et utilise un grand modèle de langage. » Tout le monde hoche la tête. Personne ne demande ce que cela veut dire. Six mois plus tard, le projet a dépassé le budget, les données se trouvent quelque part d'inattendu, et personne ne peut dire qui possède quoi.

Les mots sont l'interface. Si votre équipe ne partage pas le même sens pour « modèle », « entraînement » et « intégration », vous ne pouvez pas prendre de bonnes décisions sur aucun d'entre eux. Vous ne pouvez pas comparer deux fournisseurs. Vous ne pouvez pas rédiger un contrat. Vous ne pouvez pas savoir quand quelque chose tourne mal.

Ce chapitre est un glossaire de travail, pas un dictionnaire. Chaque mot reçoit un sens simple, une analogie de tous les jours, et la seule question qu'il faut poser quand on l'entend.

Une règle les traverse tous. **Une vraie explication contient toujours un verbe et un complément.** Pas « c'est propulsé par l'IA », mais « il lit vos factures et met le total dans votre fichier comptable ». Si quelqu'un ne peut pas vous donner un verbe et un complément, il ne vous a rien dit.

### 3.1 Données, information, connaissance

Trois mots qu'on emploie comme s'ils étaient la même chose. Ce sont trois étapes différentes, et la différence compte quand on planifie.

Une **donnée** est un fait brut, sans sens attaché. Une colonne de chiffres. Un dossier de PDF. Une liste de dates. Une donnée seule ne vous dit rien. Le nombre 47 est une donnée.

Une **information** est une donnée mise en contexte. « La facture 47 était de 1 200 € et a été payée en retard. » Maintenant le nombre veut dire quelque chose. Une information, c'est une donnée placée quelque part.

Une **connaissance** est une information plus une compréhension de ce qu'il faut en faire. « Quand ce client paie en retard, c'est généralement parce que son propre client paie en retard, donc on le relance en douceur et il finit toujours par payer. » Ça, c'est de la connaissance. Elle vit dans la tête d'une personne, et elle a mis des années à se construire.

Pensez à un classeur. La donnée, c'est le papier. L'information, c'est le papier dans un dossier étiqueté. La connaissance, c'est savoir quels dossiers comptent le lundi matin et lesquels peuvent attendre jusqu'en mars.

**Pourquoi cela compte pour vous.** L'IA travaille sur des données. Elle n'acquiert pas automatiquement votre connaissance. Vous pouvez donner à un système dix mille factures et il y apprendra des schémas. Il n'apprendra pas pourquoi votre plus gros client paie toujours en retard exprès, parce que c'est une connaissance détenue par une seule personne qui ne l'a jamais écrite.

Avant tout projet d'IA, demandez : **quelle part de ce qui fait fonctionner cette tâche est écrite sous forme de données, et quelle part vit dans la tête de quelqu'un ?** L'écart entre ces deux chiffres est la taille de votre vrai problème. Le combler est généralement plus difficile, et plus précieux, que la partie IA.

**Demandez au vendeur :** « De quelles données avez-vous besoin de notre part, sous quelle forme, et en quelle quantité ? »

### 3.2 Algorithme, modèle, entraînement

**Algorithme.** Une recette. Un ensemble clair et ordonné d'étapes qui résout un problème. Faire du café est un algorithme. La division posée est un algorithme. Un algorithme n'a pas besoin d'un ordinateur ; il a juste besoin d'étapes. Le mot vient du nom du mathématicien du IXe siècle al-Khwarizmi, dont les travaux sur le calcul étape par étape ont été traduits en latin et nous ont fini par donner ce mot.

**Modèle.** Dans le langage courant de l'IA, un modèle est ce qu'on obtient à la fin de l'entraînement : un ensemble de réglages appris que l'on peut utiliser pour répondre à de nouveaux cas. Pensez-y comme à un employé formé. Vous n'avez pas à le re-enseigner chaque matin. Le savoir est en lui.

Le mot s'emploie de deux façons, et les mélanger crée la confusion. Dans le sens ancien, un modèle est une description écrite de la façon dont quelque chose fonctionne, comme un modèle financier dans un tableur. Dans le sens moderne de l'IA, un modèle est un fichier plein de chiffres qu'on a ajustés jusqu'à ce que les réponses sortent justes. Quand quelqu'un dit « le modèle » aujourd'hui, il veut généralement dire la deuxième chose.

**Entraînement.** Le processus qui mène de rien à un modèle. Montrez des exemples. Laissez le système deviner. Comparez avec la bonne réponse. Ajustez. Répétez de nombreuses fois. Le chapitre 2 a expliqué le mécanisme. Ce qui compte ici, c'est le sens commercial : **l'entraînement est une étape que vous payez une fois, et sa qualité fixe le plafond de tout ce qui vient après.** Un modèle entraîné sur de mauvais exemples ne peut pas être réparé par une meilleure interface. On ne peut que le réentraîner, ce qui veut dire repayer.

Trois questions qui éclaircissent presque n'importe quelle conversation :

1. **Quelle est l'entrée ?** Que fait-on entrer ?
2. **Quelle est la sortie ?** Que fait-il sortir ?
3. **Sur quoi a-t-il été entraîné ?** Quels exemples, depuis quand, combien ?

Si un vendeur ne peut pas répondre à la troisième question, vous n'achetez pas un modèle. Vous achetez une promesse.

### 3.3 IA générative, LLM, prompt

**L'IA générative** est une IA qui produit du nouveau contenu au lieu de seulement trier ou noter. Le chapitre 2 l'a définie. Voici le vocabulaire autour.

**LLM — grand modèle de langage.** « Grand » veut dire qu'il a beaucoup de réglages ajustables, mesurés en milliards. Ces réglages s'appellent des **paramètres**. Un modèle de 13 milliards de paramètres contient 13 000 000 000 nombres. « Langage » veut dire qu'il a été entraîné sur du texte. « Modèle » veut dire qu'il est le résultat utilisable de l'entraînement.

Un LLM est donc un très grand ensemble de nombres, ajustés en lisant une quantité énorme de texte, jusqu'à devenir bon à continuer du texte. C'est tout. Ce n'est pas une base de faits. C'est une machine à continuer du texte.

**Prompt.** Le texte que vous donnez au modèle. Votre question, votre instruction, votre requête. C'est tout ce qu'est un prompt.

Le mot compte plus qu'il n'y paraît, car ce que vous obtenez en retour dépend fortement du prompt. Un prompt vague donne une réponse vague. Un prompt avec du contexte, un exemple et un format clair en donne une bien meilleure. Apprendre à écrire de bons prompts est une vraie compétence commerciale, et cela prend environ une semaine pour bien l'apprendre.

Un prompt ressemble à un brief que vous donnez à un rédacteur freelance. Un mauvais brief — « écris quelque chose sur notre produit » — donne quelque chose d'inutile. Un bon brief — « écris 150 mots pour des petits commerçants, en français simple, dans ce ton, et laisse de côté les prix » — donne quelque chose d'utilisable. Le rédacteur est le même. Seul le brief a changé.

**Hallucination.** Quand un modèle affirme quelque chose de faux d'un air assuré. Le mot est imparfait, car le modèle n'hallucine pas au sens médical. Il continue du texte d'une façon qui semble juste, sans magasin séparé de faits auquel se confronter. C'est pourquoi l'IA générative a besoin d'une vérification pour tout ce qui compte.

**Fenêtre de contexte.** La quantité de texte que le modèle peut considérer à la fois. Pensez-y comme à un bureau. Tout ce que vous voulez qu'il regarde doit tenir sur le bureau. Le texte qui ne tient pas n'est tout simplement pas là. Les bureaux modernes sont grands, mais pas infinis, et un bureau encombré marche moins bien qu'un bureau rangé.

**Demandez au vendeur :** « Quel modèle utilisez-vous, qui l'a fabriqué, et où vont mon prompt et mes données quand je les envoie ? »

### 3.4 RPA, no-code, low-code

Ces trois mots se vendent comme si c'était de l'IA. En général, ce n'est pas le cas.

**RPA — automatisation robotisée des processus.** Un logiciel qui copie ce qu'une personne fait à un ordinateur : ouvrir ce système, copier ce champ, le coller dans ce système, cliquer sur Enregistrer. Il fonctionne en imitant les actions de souris et de clavier, ou en utilisant les mêmes écrans qu'une personne. Le terme est apparu au début des années 2000.

Le RPA n'est pas de l'IA. Il n'a ni apprentissage ni devinette. Il suit une séquence enregistrée à la lettre. Il est fiable et fragile en même temps. L'analogie est une macro dans un tableur : il fait les mêmes étapes à chaque fois, vite, et casse si la mise en page change.

**Quand le RPA est le bon choix :** la tâche est fixe, à gros volume, et les écrans ne changent pas. Copier des données de commande d'un e-mail dans votre système de commandes cent fois par jour est un travail classique de RPA. C'est bon marché et ça marche.

**Quand le RPA est le mauvais choix :** tout ce qui varie. Si l'entrée n'est pas toujours au même endroit, le RPA cassera, et il cassera souvent.

Un modèle courant et sensé : **l'IA lit et comprend l'entrée désordonnée ; le RPA fait la saisie ennuyeuse.** L'IA gère la variation. Le RPA gère la répétition.

**No-code.** Des outils où vous construisez une automatisation en cliquant, en glissant et en choisissant dans un menu, sans écrire de code de programme. Bien pour des flux simples et clairs. Rapide à démarrer.

**Low-code.** Semblable, mais vous pouvez écrire un peu de code quand le menu n'offre pas ce dont vous avez besoin. Plus souple, un peu plus technique.

Les deux sont vraiment utiles, et les deux ont un coût caché : c'est facile à commencer et difficile à terminer. Un flux no-code qui grossit jusqu'à vingt étapes, trois systèmes et quatre personnes qui le modifient devient difficile à comprendre et dangereux à changer. Il y a un schéma bien connu où une entreprise construit des dizaines de petites automatisations no-code, que personne ne peut toutes cartographier, et où il faut finir par tout reconstruire.

**Demandez au vendeur :** « Cela apprend-il vraiment quelque chose, ou suit-il une séquence fixe ? Si un écran change, qu'est-ce qui casse et qui le répare ? »

### 3.5 Cloud, API, intégration

**Cloud.** L'ordinateur de quelqu'un d'autre. Voilà la définition honnête. Vos fichiers et vos logiciels tournent sur des machines dans un grand centre de données qu'une autre entreprise possède et entretient, et vous payez à l'usage par internet.

Le cloud a de vrais avantages : pas de matériel à acheter, une capacité que vous pouvez faire grandir en quelques minutes, une maintenance automatique. Il a aussi une conséquence permanente : **vos données sont sur les machines de quelqu'un d'autre, dans un pays que vous n'avez peut-être pas choisi, sous un contrat que vous n'avez probablement pas lu.** Le [chapitre 8](ch08-self-hosting-keep-your-data-under-control.md) couvre le fait de tout faire tourner soi-même, et le [chapitre 11](ch11-digital-sovereignty.md) couvre le contrôle et la souveraineté.

**API — interface de programmation d'application.** Une façon définie pour un logiciel de demander à un autre de faire quelque chose.

Pensez à la cuisine d'un restaurant. Vous ne pouvez pas entrer et cuisiner votre propre repas. Vous allez à un guichet et commandez à une carte fixe. La cuisine vous dit exactement ce que vous pouvez commander et comment. Ce guichet est l'API : il laisse le monde extérieur utiliser la cuisine sans la casser.

En pratique, votre site web demande à l'API de l'entreprise de transport « combien coûte l'envoi de ce colis à Madrid ? » et reçoit un nombre en quelques secondes. Personne ne téléphone à personne.

Deux choses à savoir. D'abord, si le produit d'un vendeur n'a pas d'API, vous ne pouvez pas le connecter vous-même à quoi que ce soit, et vous dépendez de ce vendeur pour toujours. Ensuite, chaque appel d'API signifie que des données traversent une frontière. Chacune est une petite porte. Certaines portes sont verrouillées et journalisées. D'autres non.

**Intégration.** Relier des systèmes pour que les données circulent entre eux sans qu'une personne les transporte. C'est là que la plupart des projets passent réellement leur temps et leur argent, et les vendeurs disent rarement de quel niveau ils parlent :

1. **Fichiers.** Exporter un tableur, le téléverser quelque part. Simple, lent, sujet aux erreurs.
2. **API.** Une connexion en direct. Rapide, fiable, demande du travail de configuration.
3. **Natif.** Intégré dans la même plateforme. Le mieux, mais cela vous enferme dans cette plateforme.

**Demandez au vendeur :** « À quels systèmes vous connectez-vous aujourd'hui, par quelle méthode, qui fait la configuration, et que devient la connexion si nous partons ? »

## Un peu d'histoire

Les mots sont plus vieux que la technologie, et le savoir aide.

**Algorithme** vient d'al-Khwarizmi, un mathématicien persan du IXe siècle dont les livres décrivaient le calcul étape par étape. Le mot a plus de mille ans de plus que l'ordinateur. **Donnée** vient du latin signifiant « choses données » — des faits au sens simple, bien avant que cela ne veuille dire quelque chose de stocké. **Réseau de neurones** vient des années 1940, des premières tentatives de décrire une cellule du cerveau comme un minuscule interrupteur marche/arrêt ; l'expression est restée même si les systèmes modernes ressemblent peu aux vrais cerveaux. **Apprentissage automatique** a été nommé en 1959 par Arthur Samuel, un chercheur américain qui travaillait sur un programme de jeu de dames. **Grand modèle de langage** est entré dans l'usage courant vers 2018, quand des modèles entraînés sur du texte à l'échelle du web sont apparus. **Prompt** est emprunté à l'informatique plus ancienne, où il désignait l'endroit où l'on tape ; il veut maintenant dire l'instruction que vous donnez à un modèle, ce qui est un bien plus gros travail que taper. **RPA** est apparu au début des années 2000 pour décrire un logiciel qui imite un humain devant un écran, et **low-code** et **no-code** sont entrés dans le vocabulaire commercial vers 2014.

La leçon du vocabulaire est simple. Presque aucun de ces mots n'a été inventé par les gens qui ont construit la technologie. Ils ont été empruntés, étirés, puis vendus. C'est pour cela qu'ils semblent vagues. Ils sont vagues. Votre travail est de fixer chacun d'eux avant de signer quoi que ce soit.

## Curiosité

### 3.6 Un modèle entraîné uniquement sur des données des années 1930 écrivait du Python — comment est-ce possible ?

En avril 2026, une petite équipe de recherche a publié un modèle de langage inhabituel. Il s'appelait **talkie**, et tout son intérêt tenait dans ce qu'il ne savait pas.

L'équipe — Nick Levine, David Duvenaud de l'Université de Toronto, et Alec Radford — a entraîné un modèle de 13 milliards de paramètres sur du texte anglais publié uniquement avant 1931. Environ 260 milliards de tokens. Un **token** est un petit morceau de texte, à peu près un mot ou une partie de mot. Les sources étaient des livres numérisés, des journaux, des périodiques, des revues scientifiques, des brevets et de la jurisprudence.

Rien d'après 1930 n'est entré. Pas d'ordinateurs. Pas d'internet. Et surtout, pas de langage de programmation, parce que Python n'a été créé que vers la fin des années 1980.

Puis ils ont testé s'il pouvait écrire du Python.

**Le résultat.** Il le pouvait, un peu. L'équipe a donné au modèle un test de programmation standard appelé HumanEval, avec une particularité : chaque problème venait avec quelques fonctions d'exemple prises au hasard, montrées directement dans la question. Le modèle n'avait jamais vu de Python à l'entraînement. Mais il pouvait regarder les exemples devant lui et copier la structure.

Les résultats ont été honnêtes et modestes. Le modèle vintage a obtenu un score bien en dessous des modèles modernes. Chaque réponse correcte qu'il a produite était un petit programme d'une ligne, comme additionner deux nombres, ou une petite modification d'un des exemples qu'on lui montrait. Comme l'a dit l'équipe, il reste encore du chemin avant que cette capacité soit remarquable.

Mais un exemple était vraiment frappant. On lui a montré une fonction qui codait un chiffrement par rotation — un code où chaque lettre décale d'une quantité fixe — et le modèle a produit la fonction de déchiffrement en changeant un seul caractère, transformant une addition en soustraction. Il n'avait jamais vu de Python. Il n'avait jamais vu d'ordinateur. Il a compris, à partir de la forme de l'exemple devant lui, que déchiffrer est l'inverse de chiffrer.

**Comment est-ce possible ?** La réponse est un comportement appelé **apprentissage en contexte** : saisir un schéma à partir des exemples placés directement dans la question, plutôt qu'à partir de l'entraînement.

Voici la version simple. Pour bien lire du texte, un modèle doit devenir extrêmement bon à remarquer la structure. Quel mot suit quel mot. Qu'est-ce qui s'ouvre et qu'est-ce qui se ferme. Qu'est-ce qu'une définition et qu'est-ce qu'un exemple. Qu'est-ce qu'une cause et qu'est-ce qu'un effet. Il apprend tout cela de livres et de journaux ordinaires.

La structure, il se trouve, se transmet. Un modèle devenu très bon à remarquer « ce bloc s'ouvre ici, se ferme là, et cette valeur coule dans celle-là » peut appliquer cette même compétence à un bloc de Python qu'il n'a jamais vu. Il n'utilise pas de connaissance de Python. Il utilise une connaissance de la structure sur de la matière Python.

C'est pour cela qu'il a pu inverser la fonction de chiffrement. Ce n'était pas de la programmation. C'était du suivi de schéma appliqué à un sujet qui n'existait pas dans ses données d'entraînement.

**Pourquoi les chercheurs l'ont fait.** La raison est pratique et maligne : un modèle entraîné uniquement sur du texte d'avant 1931 n'a pas pu mémoriser le test. Les modèles modernes sont entraînés sur le web moderne, qui contient les réponses à la plupart des questions de test publiques. Cela s'appelle la **contamination des données**, et cela rend les benchmarks modernes peu fiables. Un modèle peut bien scorer parce qu'il a vu la réponse avant, pas parce qu'il sait raisonner. Talkie est propre par construction. Tout ce qu'il fait, il l'a vraiment fait.

**Les limites honnêtes.** L'équipe a aussi signalé que talkie marchait moins bien dans l'ensemble que son « jumeau moderne » — un modèle identique entraîné sur des données web modernes — même après avoir corrigé le fait que les questions modernes perturbent un modèle des années 1930. Ils ont mis une partie de l'écart sur le compte du bruit OCR : en 1930 rien n'était numérique, donc chaque page devait être scannée et retranscrite, ce qui introduit des erreurs que le texte numérique natif n'a pas. Ils ont dit que comme effort de recherche amateur, ils ne s'attendaient jamais à combler totalement l'écart. Ils ont estimé que le corpus historique pourrait grossir jusqu'à bien plus d'un billion de tokens, assez pour un modèle à peu près comparable à l'original ChatGPT.

**La leçon commerciale.** Deux choses.

D'abord, ces modèles suivent la structure plus qu'ils ne collectionnent les faits. Cela explique à la fois leur puissance et leur manque de fiabilité. La structure se transmet bien. La vérité, elle, ne vient pas avec.

Ensuite, **la contamination des données est un vrai problème dans les affirmations des vendeurs.** Quand un vendeur dit « notre modèle obtient 94 % sur ce benchmark », demandez si le benchmark se trouvait dans les données d'entraînement. Ce n'est pas un petit détail technique. C'est la différence entre une capacité mesurée et une réponse mémorisée. Posez la question à chaque réunion de vendeur.

## Un exemple réel d'entreprise

### Quand les mots sont le produit : le « AI washing »

En septembre 2024, la Commission fédérale du commerce des États-Unis a annoncé une opération de répression qu'elle a appelée **Operation AI Comply**. La cible : des entreprises qui faisaient des affirmations exagérées ou trompeuses sur ce que leurs produits pouvaient faire avec l'intelligence artificielle. Le propre nom de la FTC pour cette pratique est **AI washing**.

Le schéma décrit par les régulateurs est simple, et il vaut la peine de le reconnaître, car c'est ainsi que commencent les mauvais achats d'IA.

Une entreprise a un produit ordinaire. Peut-être un outil de planification, ou un outil d'automatisation marketing, ou un chatbot construit à partir d'une liste fixe de réponses. L'entreprise ajoute « propulsé par l'IA » au marketing. Rien dans le produit ne change. Le prix monte. Les ventes montent.

La position de la FTC est que c'est un problème de protection du consommateur, pas un problème technique. Si vous revendiquez une capacité que vous n'avez pas, c'est une affirmation trompeuse, et l'étiquette « IA » ne vous en protège pas.

**Pourquoi c'est un exemple commercial et pas seulement juridique.** Parce que le même piège fonctionne dans les deux sens. Les vendeurs utilisent les mots à la légère pour vendre. Les acheteurs utilisent les mots à la légère pour justifier un budget en interne. Un manager qui ne peut pas expliquer ce que fait la technologie écrit « automatisation pilotée par l'IA » dans une proposition, obtient l'approbation du budget, puis doit faire marcher quelque chose que personne n'a défini.

L'opération du régulateur vous est utile comme une liste de contrôle à l'envers. Avant d'acheter, demandez :

1. **Quelle affirmation précise est faite ?** Écrivez-la en une phrase avec un verbe et un complément.
2. **Comment saurions-nous si cette affirmation était fausse ?** Si personne ne peut nommer un test, l'affirmation est du décor.
3. **L'affirmation est-elle dans le contrat ?** Le langage marketing n'est pas un engagement. Si une capacité compte, elle devrait être écrite avec un nombre et une date.
4. **Qui est responsable si cela ne performe pas ?** Nommez une personne, pas une entreprise.

Un vendeur honnête répond aux quatre sans difficulté. Un vendeur qui fait du lavage devient vague. La vague dans la réponse à des questions précises est en soi la réponse.

## Comment faire

### Le test des mots simples

Utilisez-le chaque fois qu'un terme technique apparaît dans une réunion.

**Étape 1 : Arrêtez-vous sur le mot.** Ne le laissez pas passer parce qu'il semble important.

**Étape 2 : Demandez une phrase avec un verbe et un complément.** Pas « il utilise un grand modèle de langage », mais « il lit nos e-mails de support et rédige une réponse ». Si le locuteur ne peut pas en produire une, le mot n'a pas encore de contenu.

**Étape 3 : Demandez ce qui entre et ce qui sort.** Tout vrai système a une entrée et une sortie. Écrivez les deux.

**Étape 4 : Demandez ce qui le casse.** Chaque technologie a un mode de défaillance. Un vendeur honnête nomme le sien.

**Étape 5 : Écrivez votre propre définition sur une ligne et relisez-la.** Si un collègue intelligent ne pouvait pas la comprendre, la définition n'est pas finie.

### Votre tableau de traduction de travail

| Mot que vous entendez | Sens simple | Que demander |
|---|---|---|
| Propulsé par l'IA | Utilise un composant appris, peut-être minuscule | Quelle partie, exactement ? |
| Modèle | Un fichier de réglages appris qui répond à de nouveaux cas | Entraîné sur quoi, quand, combien ? |
| Entraînement | Ajuster des réglages contre des exemples jusqu'à ce que les réponses correspondent | Qui l'a fait, et qui l'a vérifié ? |
| LLM | Un très grand système de continuation de texte | Lequel, fabriqué par qui, tournant où ? |
| Prompt | L'instruction que vous donnez au modèle | Pouvons-nous écrire et réutiliser les nôtres ? |
| Hallucination | Une affirmation assurée qui est fausse | Comment la détectez-vous et la corrigez-vous ? |
| RPA | Un logiciel qui imite une personne cliquant sur des écrans | Qu'est-ce qui casse quand l'écran change ? |
| No-code | Construire en cliquant, sans programmation | Que ne peut-il pas faire ? |
| Low-code | Surtout cliquer, un peu de programmation permise | Qui le maintient ici ? |
| Cloud | Tourne sur les ordinateurs de quelqu'un d'autre | Quel pays, quel contrat, quelles données partent ? |
| API | Une fenêtre définie pour qu'un système en utilise un autre | Existe-t-elle ? Pouvons-nous l'utiliser nous-mêmes ? |
| Intégration | Les données circulent entre systèmes sans personne | Quelle méthode, qui la configure, et si nous partons ? |
| Token | Un petit morceau de texte | Combien par usage typique, et combien cela coûte ? |
| Fenêtre de contexte | La quantité de texte que le modèle peut regarder à la fois | Que se passe-t-il quand notre document est trop gros ? |

### Construisez un glossaire partagé pour votre entreprise

Faites-le une fois et gardez-le vivant.

1. Commencez une seule page. Tout terme qui surgit dans une discussion IA va dessus.
2. Chaque entrée reçoit trois lignes : le sens simple, ce que cela veut dire *dans notre entreprise*, et une question à laquelle nous ne pouvons pas encore répondre.
3. Une personne nommée possède la page. Pas un comité.
4. Avant toute réunion de vendeur, lisez la page. Pendant la réunion, ajoutez-y.
5. Retirez les entrées que vous n'utilisez jamais. Gardez-la sous deux pages.

Un glossaire partagé est une petite chose avec un effet démesuré. Il transforme « nous avons acheté de l'IA » en « nous utilisons un modèle de texte pour rédiger des réponses et un outil à règles pour les classer, et une personne vérifie les deux ».

## Éthique et responsabilité

### 3.7 Vie privée, sécurité, biais — la version courte

Trois mots que vous entendrez constamment. Voici l'introduction simple. Le traitement complet se trouve ailleurs, et vous devriez lire ces chapitres avant de déployer quoi que ce soit qui touche des données clients.

La **vie privée** concerne qui a le droit de voir et d'utiliser des informations personnelles. La question pratique pour chaque outil d'IA est simple : *quand je colle quelque chose, où cela va-t-il, qui peut le lire, et que gardent-ils ?* Ne mettez jamais les détails personnels d'un client dans un outil que vous n'avez pas vérifié. Le [chapitre 10](ch10-privacy-and-gdpr.md) couvre le droit de la vie privée et le RGPD comme il faut.

La **sécurité** concerne la protection des systèmes contre les attaques, les abus et les accidents. L'IA ajoute de nouvelles façons d'être attaqué, y compris tromper un modèle avec une entrée soigneusement formulée et empoisonner les données sur lesquelles il apprend. Le [chapitre 6](ch06-cybersecurity-in-the-ai-era.md) couvre cela en détail.

Le **biais** est quand un système traite certaines personnes moins bien que d'autres de façon systématique, parce que les exemples dont il a appris étaient inégaux. Si les décisions d'embauche passées favorisaient un groupe, un modèle entraîné sur elles apprendra à favoriser ce groupe. Le biais n'est pas un défaut moral de la machine. C'est un miroir tendu aux exemples. Le [chapitre 4](ch04-ethical-ai-doing-the-right-thing.md) couvre le biais, la transparence, l'explicabilité et la responsabilité humaine comme partie du cadre éthique complet.

La seule chose à retenir de cette section : **on ne peut pas gérer un risque qu'on ne peut pas nommer.** Apprendre les mots n'est pas académique. C'est la première condition pour poser les bonnes questions.

## Erreurs à éviter

**Erreur 1 : Accepter « l'IA » comme une fonctionnalité.** Ce n'est pas une fonctionnalité. C'est une catégorie contenant des dizaines de technologies très différentes. Demandez laquelle.

**Erreur 2 : Croire que no-code veut dire sans réflexion.** Le no-code enlève la programmation. Il n'enlève ni la conception, ni la maintenance, ni le risque d'un enchevêtrement d'automatisations impossible à cartographier.

**Erreur 3 : Confondre RPA et IA.** Si cela suit une séquence enregistrée, cela n'apprend rien. Ce peut être exactement ce que vous voulez, ou exactement ce qui échouera.

**Erreur 4 : Croire qu'une API veut dire que vous êtes intégré.** Une API est une possibilité, pas une connexion. Quelqu'un doit encore construire et maintenir la connexion.

**Erreur 5 : Ne pas demander où est réellement le cloud.** « Le cloud » est un centre de données, dans un pays, sous un contrat. Demandez lequel.

**Erreur 6 : Laisser un vendeur définir vos termes.** Si le vocabulaire du vendeur est le seul vocabulaire dans la pièce, le vendeur contrôle la réunion.

**Erreur 7 : Sauter le test des mots simples parce que cela semble lent.** Cinq minutes de « qu'est-ce que cela veut vraiment dire ? » coûtent moins cher que six mois d'un projet que personne ne peut décrire.

**Erreur 8 : Croire un benchmark sans demander la contamination.** L'expérience Talkie existe précisément parce que les résultats de tests modernes peuvent être gonflés par des réponses déjà présentes dans les données d'entraînement.

## Exercice pratique

### 3.8 Traduire une phrase technique en mots simples

C'est la compétence la plus utile de ce chapitre. Entraînez-vous sur ces six phrases. Écrivez votre réponse avant de lire la réponse modèle.

**Phrase 1 :** « Notre plateforme s'appuie sur un grand modèle de langage pour offrir un traitement intelligent de documents à grande échelle. »

*Réponse modèle :* « Il lit des documents et en extrait les champs que vous voulez. Il utilise un gros modèle de texte fabriqué par quelqu'un d'autre. "À grande échelle" veut dire qu'il peut en faire beaucoup à la fois. »

**Phrase 2 :** « La solution est un robot RPA low-code avec intégration d'API dans le cloud. »

*Réponse modèle :* « Un robot qui copie des données d'un écran à un autre. Vous pouvez le configurer surtout en cliquant. Il parle à d'autres systèmes par internet via une connexion définie. Il tourne sur les ordinateurs du vendeur. »

**Phrase 3 :** « Nous utilisons la génération augmentée par récupération (retrieval) pour ancrer le modèle dans votre base de connaissances. »

*Réponse modèle :* « Avant de répondre, il cherche les pages pertinentes dans vos propres documents et s'en sert comme base. Cela réduit les réponses inventées. Cela ne marche que si vos documents sont bons et à jour. »

**Phrase 4 :** « Le modèle est ajusté finement sur vos données de domaine. »

*Réponse modèle :* « Ils ont pris un modèle général existant et l'ont entraîné davantage sur vos exemples, pour qu'il colle mieux à votre entreprise. Vous payez pour ça. Cela veut aussi dire que vos données ont été envoyées à celui qui a fait l'entraînement. »

**Phrase 5 :** « Notre IA fournit une prise de décision explicable et transparente. »

*Réponse modèle :* « Ils prétendent que vous pouvez voir pourquoi il a décidé ce qu'il a décidé. Demandez-leur de vous montrer, sur un vrai cas, maintenant. S'ils ne le peuvent pas, l'affirmation est du décor. »

**Phrase 6 :** « C'est un système multi-agents avec orchestration. »

*Réponse modèle :* « Plusieurs composants d'IA travaillent sur une tâche en séquence ou en parallèle, et quelque chose les coordonne. Demandez : combien de composants, que fait chacun, et que se passe-t-il si l'un tombe en panne ? »

**Maintenant faites le vôtre.** Trouvez une phrase d'un e-mail de vendeur reçu le mois dernier. Traduisez-la avec la même méthode : verbe et complément, entrée, sortie, ce qui casse. Renvoyez votre traduction au vendeur et demandez si elle est correcte. Sa réaction vous apprendra beaucoup.

## Liste de contrôle

### 3.9 Votre glossaire minimum

- [ ] Je peux expliquer données, information et connaissance, et je sais quelle part de ma connaissance d'entreprise est écrite.
- [ ] Je peux définir algorithme comme « une recette » : un ensemble ordonné d'étapes.
- [ ] Je peux définir modèle comme « la chose entraînée que vous utilisez pour répondre à de nouveaux cas ».
- [ ] Je peux définir entraînement comme « ajuster des réglages contre des exemples jusqu'à ce que les réponses correspondent ».
- [ ] Je sais qu'un LLM est un système de continuation de texte, pas une base de faits.
- [ ] Je sais qu'un prompt est l'instruction que je donne au modèle, et que sa qualité change le résultat.
- [ ] Je sais ce qu'est un token et à peu près ce que les tokens coûtent par usage typique.
- [ ] Je sais ce qu'est une fenêtre de contexte et ce qui se passe quand un document est trop gros pour elle.
- [ ] Je sais que « hallucination » veut dire une affirmation assurée mais fausse, et qu'elle a besoin d'une vérification.
- [ ] Je sais distinguer le RPA de l'IA, et je sais que le RPA est bon marché et fragile.
- [ ] Je sais que no-code et low-code enlèvent la programmation, pas la conception ni la maintenance.
- [ ] Je sais que « le cloud » veut dire les ordinateurs de quelqu'un d'autre, dans un pays précis, sous un contrat précis.
- [ ] Je sais qu'une API est une fenêtre définie pour qu'un système en utilise un autre, et je demande toujours s'il en existe une.
- [ ] Je sais les trois niveaux d'intégration : fichiers, API, natif.
- [ ] J'utilise le test des mots simples : un verbe, un complément, une entrée, une sortie, et ce qui casse.
- [ ] J'ai commencé un glossaire partagé d'une page avec un propriétaire nommé.
- [ ] Je sais que la vie privée, la sécurité et le biais ont chacun un chapitre complet, et je les ai lus ou vais les lire.

## Points à retenir

- La plupart des mauvaises décisions en IA viennent de mots non définis, pas d'une mauvaise technologie.
- Une vraie explication contient toujours un verbe et un complément ; si vous ne pouvez pas en nommer un, on ne vous a rien dit.
- Les modèles suivent la structure, ils ne gardent pas les faits, ce qui explique pourquoi ils transfèrent des compétences d'un sujet à l'autre et pourquoi ils énoncent des faussetés avec assurance.
- L'expérience Talkie montre qu'un modèle sans aucune connaissance des ordinateurs peut quand même écrire un peu de Python, et elle existe parce que les résultats de benchmarks modernes peuvent être gonflés par des données contaminées.
- Fixez chaque terme avant de signer : ce qui entre, ce qui sort, ce qui le casse, et qui le possède.
