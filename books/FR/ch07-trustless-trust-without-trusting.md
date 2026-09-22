# Chapitre 7 — Confiance sans avoir à faire confiance

## En mots simples

Le mot « trustless » (sans confiance) est mal choisi. Il évoque un monde sans confiance, où personne ne croit rien. Ce n'est pas ce que cela veut dire, et la vraie idée est bien plus utile.

« Trustless » signifie : **vous n'avez pas à faire confiance à une personne ou à une institution, parce que vous pouvez vérifier le fait vous-même.**

Partons d'un contraste familier. Vous engagez une entreprise de déménagement. Vous versez un acompte. Vous dépendez maintenant qu'ils se présentent. Vous devez leur faire confiance, ou faire confiance à leur marque, ou faire confiance à la loi pour les punir s'ils ne viennent pas. Pensez maintenant à un distributeur automatique. Vous mettez des pièces, la boisson tombe. Il n'y a pas de relation, pas de promesse, et pas besoin de croire qui que ce soit. La machine fait respecter le deal par la façon dont elle est construite. C'est le sentiment du « trustless » : l'accord est fait respecter par un système au lieu des bonnes intentions d'une personne.

Trois outils rendent cela possible.

**La vérification au lieu des promesses.** Au lieu que quelqu'un vous dise qu'une chose est vraie, vous la vérifiez. Une signature numérique est l'exemple courant. Elle prouve qu'un fichier vient de qui détient une certaine clé, et que le fichier n'a pas changé depuis qu'il a été signé. Vous n'avez pas à faire confiance à l'expéditeur. Vous vérifiez la signature.

**La transparence au lieu du secret.** Au lieu de garder un registre dans un carnet privé unique, vous le gardez quelque part où beaucoup peuvent lire et où personne ne peut réécrire en douce. Si tout le monde peut voir le registre, une partie ne peut pas réécrire l'histoire à son avantage.

**L'application automatique au lieu de l'espoir.** Au lieu de convenir de conditions et d'espérer qu'elles soient respectées, vous écrivez les conditions pour qu'un logiciel les exécute. L'argent est libéré quand la condition est remplie. Personne n'a à courir après une facture.

Maintenant l'avertissement honnête, dit d'emblée : « trustless » ne veut pas dire sans risque. Vous avez déplacé votre confiance des gens vers des systèmes, et les systèmes sont construits par des gens. Le code a des bugs. Les flux qui disent à un système ce qui s'est passé dans le monde réel peuvent être faux ou mentis. Les clés se perdent, et une clé perdue peut signifier de l'argent perdu. Le but n'est pas de supprimer la confiance. C'est de placer la confiance quelque part que vous pouvez inspecter, et de réduire la quantité dont vous avez besoin.

Pourquoi s'en donner la peine ? Parce que la confiance coûte cher. Chaque intermédiaire sur qui vous comptez — une banque, un séquestre, un courtier, un notaire, une plateforme qui retient les fonds jusqu'à ce que le travail soit fait — prend une commission et prend du temps. Les systèmes « trustless » en retirent une partie, et rendent ce qui reste moins cher, plus rapide et visible. Ce n'est pas réservé aux banques et aux programmeurs ; cela a un usage direct dans toute entreprise qui achète à des fournisseurs, embauche des freelances, et a besoin d'enregistrements dont son comptable peut se fier.

La question plus large de qui contrôle vos outils numériques est dans le [Chapitre 11 — Souveraineté numérique](ch11-digital-sovereignty.md). Savoir si cela rapporte est une question du [Chapitre 16 — Objectifs, coûts et retour sur investissement](ch16-goals-costs-and-return-on-investment.md). Le volet sécurité de la vérification est dans le [Chapitre 6 — Cybersécurité à l'ère de l'IA](ch06-cybersecurity-in-the-ai-era.md).

## Un peu d'histoire

**2008.** En octobre, un article intitulé « Bitcoin : un système de monnaie électronique pair à pair » est publié sous le nom de Satoshi Nakamoto. Son but affiché est le paiement électronique sans tiers de confiance. L'astuce est un registre partagé et ordonné — une blockchain — tenu ensemble par beaucoup d'ordinateurs indépendants, de sorte qu'aucun seul ne peut le réécrire.

**2009.** Le réseau Bitcoin commence à tourner en janvier. Pour la première fois, deux inconnus peuvent régler de la valeur sans banque au milieu, et aucun n'a à faire confiance à l'autre.

**2015.** Ethereum arrive et ajoute la mise à niveau clé : les contrats intelligents. Un contrat intelligent est un programme stocké sur le réseau qui s'exécute exactement comme écrit quand ses conditions sont remplies. L'argent peut désormais être lié à une règle.

**2016.** Un projet appelé The DAO détient des fonds dans un contrat intelligent et est vidé à cause d'une faille dans ce contrat. Les conséquences divisent la communauté. La leçon est nette et toujours vraie : l'application automatique applique les bugs avec la même loyauté qu'elle applique les fonctionnalités.

**2017 à 2021.** La finance décentralisée devient un vrai secteur : prêt, échange et règlement gérés par des contrats au lieu de banques, avec des stablecoins — des jetons censés maintenir une valeur stable — comme monnaie de travail. Elle montre aussi les mêmes échecs à plus grande échelle : mauvais code, flux de prix erronés, opérateurs malhonnêtes. En **2019**, le W3C, l'organisme qui fixe les standards du web, publie les Identifiants Vérifiables (Verifiable Credentials) : une façon pour une autorité d'émettre une affirmation numérique — un diplôme, une licence, une preuve d'âge — que n'importe qui peut vérifier sans téléphoner à l'émetteur. C'est la moitié identité du tableau.

**2021 à 2023.** Un standard appelé ERC-4337, connu comme l'abstraction de compte, est proposé en 2021 puis finalisé plus tard. Il permet à un compte d'être un petit programme au lieu d'une seule clé privée, si bien que le compte peut porter ses propres règles : plafonds de dépense, liste de bénéficiaires autorisés, une seconde signature pour les gros montants, et récupération si une clé est perdue.

**Mai 2025.** Une mise à niveau d'Ethereum appelée Pectra entre en service sur le réseau principal. Elle permet à une adresse de portefeuille ordinaire de pointer vers du code de contrat intelligent, apportant le regroupement de transactions, des frais sponsorisés et une meilleure récupération à des adresses qui n'en avaient aucune auparavant. Elle augmente aussi la mise maximale qu'un seul validateur peut détenir.

**Août 2025.** Un projet de standard appelé ERC-8004 apparaît, intitulé « Trustless Agents » (Agents sans confiance). Il est écrit pour le problème dont ce chapitre parle vraiment : des agents logiciels qui traitent avec les agents d'autres personnes.

Lisez la chronologie comme un long argument. Chaque étape a déplacé l'application des mains d'une personne vers un système vérifiable : d'abord l'argent, puis les accords, puis l'identité, puis les permissions, et plus récemment les agents.

## Curiosité

### 7.6 Ethereum construit la plomberie d'une économie d'agents

En août 2025, un projet de standard appelé **ERC-8004** est publié sur le site officiel des standards d'Ethereum. Son titre est « Trustless Agents », et son but affiché est de laisser des agents logiciels découvrir, choisir et travailler avec d'autres agents au-delà des frontières organisationnelles sans aucune confiance préalable.

Il définit trois registres, tous sur la chaîne (on-chain).

**Identité.** Chaque agent reçoit un identifiant sur la chaîne, construit sur le standard de jeton courant ERC-721, qui pointe vers un fichier d'enregistrement. Ce fichier contient les métadonnées de l'agent, les adresses avec qui vous pouvez parler, et quels modèles de confiance il prend en charge. En termes simples : un agent peut dire qui il est, pour qui il agit, et comment vous pouvez le vérifier, et vous pouvez consulter cela au lieu de le croire sur parole.

**Réputation.** Une façon standard de publier et lire des retours sur un agent, pour que l'historique de performance ne soit pas enfermé dans la notation par étoiles privée d'une seule plateforme. N'importe qui peut contribuer des signaux, et l'agrégation peut se faire hors chaîne (off-chain). L'idée est la portabilité : le dossier d'un agent le suit, au lieu d'être remis à zéro à chaque fois qu'il change de marché.

**Validation.** Des points d'accroche (hooks) pour obtenir une vérification indépendante du travail d'un agent. Le standard liste plusieurs méthodes : faire ré-exécuter la tâche par une autre partie avec de l'argent en jeu, utiliser des preuves de machine learning à divulgation nulle de connaissance (zero-knowledge) — une façon de prouver qu'un calcul a été fait correctement sans révéler les données ni le modèle derrière — utiliser des enclaves matérielles de confiance, ou utiliser un juge humain de confiance.

Pourquoi un dirigeant de petite entreprise devrait-il se soucier d'un projet de standard ? Il montre où l'industrie pense que se trouve le problème difficile : non pas « un agent peut-il faire la tâche » mais « comment savoir si je dois croire cet agent » — une question de business, pas technique. Si cela réussit, vous pourrez consulter un registre public au lieu de faire confiance à un argumentaire commercial, ce qui change qui détient le pouvoir dans la conversation. Et les trois mêmes questions sont une checklist utile aujourd'hui, sans aucune blockchain : *Qui êtes-vous, et pour qui agissez-vous ? Comment vous êtes-vous comporté auparavant ? Votre travail peut-il être vérifié indépendamment ?*

Deux autres morceaux de la même plomberie sont déjà en service. L'abstraction de compte, le standard ERC-4337, signifie qu'un agent peut détenir un budget avec des règles imposées par le code : un plafond de dépense dur, une liste blanche de bénéficiaires autorisés, une seconde signature humaine au-dessus d'un seuil. Et depuis la mise à niveau Pectra en mai 2025, une adresse ordinaire peut pointer vers un tel code. Cette combinaison — un agent qui peut payer, dans une boîte dont il ne peut pas sortir — est la forme pratique d'une économie d'agents « trustless ».

Traitez tout cela comme une direction, pas comme un produit à acheter ce trimestre. ERC-8004 est un projet. Les concepts, eux, sont utilisables maintenant.

## Un exemple d'entreprise réel

### La mangue qui a mis sept jours à tracer, puis deux secondes

En 2017, Walmart et IBM ont mené un pilote dans les chaînes d'approvisionnement alimentaire, et les chiffres qu'ils ont publiés sont devenus célèbres dans le secteur. Tracer l'origine d'une mangue sourcée en Amérique centrale ou du Sud prenait environ sept jours d'appels, d'emails et de paperasse. Avec les registres tenus sur un grand livre partagé, le même traçage a pris environ 2,2 secondes. IBM l'a décrit comme une traçabilité complète de bout en bout. Un pilote parallèle suivait le porc en Chine.

Deux notes honnêtes. Le chiffre venait d'un pilote contrôlé, pas d'un déploiement complet en conditions réelles, et les 2,2 secondes sont le temps d'interroger le registre, pas le temps de corriger une cargaison contaminée.

Regardez maintenant ce qui a changé. Avant, chaque partie gardait son propre carnet : la ferme écrivait la date de récolte, l'emballeur le lot, le transporteur le conteneur, le magasin la livraison. Pour répondre à une seule question, il fallait demander à quatre entreprises de fouiller leurs carnets privés et espérer qu'elles répondent vite et honnêtement. Après, tout le monde écrivait dans le même registre au fur et à mesure. Personne ne pouvait réécrire sa page en douce, et « d'où vient ceci » est devenu une consultation au lieu d'une négociation.

C'est la valeur « trustless » en une phrase : **vous avez remplacé une chaîne de promesses par un seul registre partagé que vous pouvez lire.**

Cela montre aussi la limite, qui compte plus que la victoire. Un registre partagé prouve ce qui a été écrit. Il ne prouve pas que l'écriture était vraie. Si un fournisseur entre une fausse ferme ou une fausse date, le grand livre préserve le mensonge parfaitement. Le maillon faible est le moment où un humain ou un capteur met un fait dans le système. Tout projet « trustless » qui ignore ce moment est du décor.

## Comment faire

### 7.3 Comment cela fonctionne en pratique : identité vérifiable, réputation, paiements programmables

Vous n'avez pas besoin d'une cryptomonnaie pour utiliser la pensée « trustless ». Quatre blocs de base s'appliquent au business ordinaire.

**Bloc 1 : Identité vérifiable.**
La question est : est-ce vraiment qui ça prétend être, et puis-je vérifier sans téléphoner à personne ? Les certificats numériques et les signatures numériques répondent déjà à cela pour vous chaque jour. Quand un fournisseur envoie un document signé avec une signature numérique reconnue, vous pouvez vérifier à la fois qui l'a signé et que rien n'a changé après. Un identifiant vérifiable va plus loin : votre comptable peut prouver qu'il détient une licence à jour, ou un membre du personnel peut prouver qu'il a passé une vérification d'antécédents, sans remettre tout le certificat et sans que vous appeliez l'organisme émetteur.

**Bloc 2 : Registres infalsifiables.**
La question est : quelqu'un peut-il réécrire l'histoire en douce ? Un grand livre partagé est une réponse. Un truc plus simple appelé empreinte (hash) en est une autre — une courte empreinte calculée à partir d'un fichier. Si vous enregistrez l'empreinte d'un document au moment où vous le convenez, et que le fichier est changé plus tard, l'empreinte ne correspondra pas. Vous pouvez produire cette empreinte plus tard et prouver l'état du document à ce moment-là. Cela ne coûte presque rien et ne demande aucune permission spéciale.

**Bloc 3 : Paiements programmables.**
La question est : l'argent peut-il bouger tout seul quand la condition est remplie ? La séquestre (escrow) est la vieille version : un tiers retient les fonds et les libère sur un déclencheur. La version plus récente écrit le déclencheur dans du code, si bien qu'aucune décision humaine n'est nécessaire au moment de la libération. Le paiement par jalons pour un freelance est le cas évident : le paiement est libéré quand le livrable est accepté, et la règle d'acceptation est écrite à l'avance.

**Bloc 4 : Auditabilité.**
La question est : après coup, pouvons-nous tous les deux voir la même vérité ? Chaque action devrait laisser un enregistrement horodaté, ordonné et non modifiable. Quand les deux côtés lisent le même registre, les disputes sont courtes. Votre comptable, votre auditeur et votre client peuvent tous vérifier la même chose sans vous demander une faveur.

**Comment commencer petit, aujourd'hui :**

1. Choisissez un processus où vous courez actuellement après une confirmation.
2. Écrivez la condition de libération comme une seule phrase testable. Si vous ne pouvez pas l'écrire comme une phrase testable, le processus n'est pas prêt.
3. Demandez si une machine peut mesurer le déclencheur. Livré veut dire un bon de livraison signé scanné. Approuvé veut dire un clic sur un bouton d'approbation. Terminé veut dire un changement de statut dans votre propre système.
4. Mettez l'argent derrière une règle qui attend cette mesure : un service de séquestre, un échéancier de paiement dans votre système comptable, ou un workflow qui exige le déclencheur avant la libération.
5. Journalisez chaque étape là où les deux côtés peuvent la voir.
6. Seulement alors automatisez.

### 7.4 Des agents IA qui interagissent entre eux : le futur du business automatisé

La version intéressante est proche. Votre agent logiciel parle à l'agent logiciel d'un fournisseur, et ils règlent une transaction sans humain à chaque étape.

Pour que cela fonctionne en sécurité, cinq choses doivent exister.

**Identité et autorité.** Non seulement « ceci est l'agent du fournisseur X », mais « cet agent est autorisé à s'engager jusqu'à 500 unités à un prix inférieur à 4,20 l'unité ». L'autorité doit être prouvable et bornée, pas supposée.

**Un deal lisible par machine.** Les deux côtés ont besoin des termes sous une forme structurée — quantité, prix, date de livraison, pénalité — pas un gentil fil d'emails. Un humain peut pardonner l'ambiguïté. Un système automatisé soit cale dessus, soit l'exploite.

**Un circuit de paiement qui peut attendre.** Le paiement doit être conditionnel : retenu, puis libéré sur preuve. Un paiement instantané et inconditionnel enlève tout levier et toute raison de performer.

**Des preuves.** Une confirmation de livraison, un enregistrement d'acceptation, un reçu signé, sous une forme que les deux systèmes peuvent lire et qu'aucun ne peut altérer en douce.

**Un chemin de litige.** Quelque chose doit gérer le cas où les deux agents ne sont pas d'accord, ou où le monde ne s'est pas passé comme la règle le supposait. Sans route d'escalade, un petit désaccord devient un paiement bloqué et un fournisseur en colère.

Ce qui est réaliste maintenant : les agents peuvent déjà chercher, comparer, rédiger des devis et préparer des commandes. Ce qui n'est pas encore courant, c'est de les laisser engager de l'argent et des termes juridiques seuls. Le chemin sensé est un humain qui approuve l'engagement final pendant que l'agent prépare tout. Cela garde la vitesse et enlève le risque.

### 7.5 Ce que cela signifie pour votre entreprise : contrats intelligents, paiements automatiques, auditabilité

**Les contrats intelligents, en mots simples.** Un contrat intelligent est un programme qui détient un accord et le exécute quand la condition énoncée se produit. Il n'est pas malin et ce n'est pas un contrat au sens de l'avocat. C'est un distributeur automatique très littéral. Écrivez la règle soigneusement et c'est un excellent serviteur. Écrivez-la vaguement et c'est un excellent serviteur aussi — à ce que vous avez réellement écrit.

**Paiements automatiques.** La forme pratique est un paiement qui attend. Il attend une confirmation de livraison, un clic d'approbation, un jalon accepté, une date atteinte. Chacun est plafonné, journalisé et visible des deux côtés avant de bouger.

**Auditabilité.** Chaque étape laisse un enregistrement. Votre comptable clôture le mois plus vite parce qu'il n'y a rien à reconstruire. Une dispute client se termine en minutes parce que les deux côtés regardent la même ligne. Si un régulateur demande, vous produisez le registre au lieu d'une histoire.

**Où cela s'adapte bien :** paiements de fournisseurs transfrontaliers où l'application est lente ; jalons de freelances et de sous-traitants ; marchés où acheteur et vendeur sont des inconnus ; accords de partage de données où vous devez prouver ce que vous avez libéré et quand ; assurance qui paie sur un événement mesuré, comme un retard de vol.

**Où cela s'adapte mal :** tout ce qui a besoin de jugement, de négociation, ou d'une relation. Tout ce où le déclencheur ne peut pas être mesuré honnêtement. Tout ce où un mauvais paiement automatique est difficile à récupérer.

## Éthique et responsabilité

Les systèmes « trustless » changent qui est redevable, c'est exactement pourquoi ils demandent une réflexion soignée.

**Un code qui impose impose aussi les erreurs.** Si votre règle libère un paiement sur une condition facile à falsifier, vous avez automatisé une perte. Écrivez la règle pour le cas malhonnête, pas seulement pour celui efficace.

**Les oracles sont des gens.** Un « déclencheur mesurable par machine » dépend souvent d'un humain qui entre des données quelque part. Le maillon faible d'une chaîne « trustless » est le moment où une personne tape la vérité dedans. Concevez pour que cette personne soit pressée, trompée, ou corrompue.

**L'immutabilité entre en collision avec la vie privée.** Mettre des données personnelles sur un registre permanent et immuable peut entrer en conflit avec les droits de protection des données, y compris le droit à l'effacement. Gardez les données personnelles hors des grands livres publics ; ne stockez que des références et des empreintes. Le détail juridique est dans le [Chapitre 10 — Vie privée et RGPD](ch10-privacy-and-gdpr.md).

**Ne retirez pas l'humain d'un problème humain.** Les clients mécontents ne veulent pas d'une règle parfaitement appliquée ; ils veulent que quelqu'un les écoute. Le « trustless » est pour le milieu ennuyeux d'une transaction, pas pour le moment où quelqu'un est contrarié.

**Soyez transparent, et gardez un responsable nommé.** Dites aux gens dont le travail est maintenant mesuré par le système, et expliquez comment une décision peut être renversée ; une règle que personne n'a le droit de contester finira par être fausse sans que personne puisse la corriger. L'application automatique n'enlève pas la responsabilité — quelqu'un dans votre entreprise doit quand même posséder le résultat, comme l'expose le [Chapitre 4 — IA éthique : faire ce qui est juste](ch04-ethical-ai-doing-the-right-thing.md).

## Erreurs à éviter

### 7.7 Tout n'a pas besoin d'être « trustless »

1. **Utiliser une blockchain là où un tableur suffirait.** Si les parties se font confiance, le registre est petit, et un contrat normal fonctionne, un grand livre distribué ajoute du coût et de la complexité pour rien.
2. **Confondre « trustless » et sans risque.** Le code a des bugs, les flux peuvent être faux, les clés peuvent être perdues, et il n'y a souvent pas de numéro d'assistance à appeler.
3. **Automatiser un mauvais processus.** Un système « trustless » imposera votre mauvais processus plus vite et plus constamment qu'une personne ne l'a jamais fait.
4. **Mettre des données personnelles sur une chaîne publique.** Elles ne peuvent pas être supprimées plus tard.
5. **Pas d'interrupteur d'arrêt.** Tout système de paiement automatisé a besoin d'un moyen de l'arrêter en un clic.
6. **Pas de plafond de dépense.** Un agent avec un portefeuille ouvert est un chéquier ouvert.
7. **Trop faire confiance au déclencheur.** Demandez comment le déclencheur pourrait être falsifié, puis décidez si cela compte.
8. **Courir après un pitch.** « Trustless » est une idée de design utile, pas une raison d'acheter un jeton. Si une proposition ne peut pas expliquer le déclencheur, le registre et le chemin de litige, c'est du marketing.
9. **Éliminer chaque intermédiaire.** Certains intermédiaires méritent leur commission. Un notaire, un transitaire en douane ou un assureur font peut-être un vrai travail que le code ne peut pas faire.
10. **Oublier qui est redevable.** Même avec une application automatique, un humain nommé doit posséder le résultat.

## Exercice pratique

### 7.8 Pensez à un processus d'entreprise qui pourrait bénéficier d'une automatisation « trustless »

Choisissez un processus où vous passez du temps à vérifier, courir après, ou disputer. Travaillez ces neuf questions par écrit.

1. **Qui sont les parties ?** Nommez-les. Notez si elles se font déjà confiance.
2. **Que doit-il être vrai avant que l'argent bouge ?** Une phrase.
3. **Qui vérifie cela aujourd'hui ?** Une personne ? Combien de temps cela prend-il ? À quelle fréquence est-ce faux ?
4. **Que coûte cette vérification ?** Temps, frais, retards. Des chiffres approximatifs suffisent ; marquez-les comme approximatifs.
5. **Une machine peut-elle mesurer le déclencheur ?** Si oui, quel est le signal ? Si non, le processus peut-il être repensé pour le pouvoir ?
6. **Quelle est la piste de preuves ?** Quel registre existe, où, et l'un ou l'autre côté peut-il le changer ?
7. **Que se passe-t-il en cas de litige ?** Qui décide, et à quelle vitesse ?
8. **Quel est le pire façon dont cela pourrait être abusé ?** Écrivez le scénario malhonnête avant celui efficace.
9. **Quel est le plafond ?** La perte maximale si la règle est fausse.

Maintenant notez-le. Si le coût de vérification est une grande part de la valeur de la transaction, le déclencheur est mesurable par machine, et vous pouvez fixer une perte maximale basse, le processus est un solide candidat. Si le déclencheur ne peut pas être mesuré par une machine, ou la perte maximale est élevée, gardez un humain dedans.

Écrivez une page. Apportez un candidat à votre prochaine réunion.

## Checklist

### 7.9 Quand envisager une approche « trustless »

- [ ] **Vous payez un intermédiaire surtout pour retenir ou vérifier quelque chose**, et cette vérification pourrait être écrite comme une règle.
- [ ] **Les parties ne se font pas déjà confiance**, et construire la confiance serait lent ou impossible.
- [ ] **La condition de libération peut être énoncée comme une seule phrase testable** qu'une machine peut mesurer.
- [ ] **La transaction se produit souvent**, si bien que le coût de mise en place est réparti sur beaucoup d'usages.
- [ ] **Elle est transfrontalière ou inter-entreprises**, là où l'application locale est lente ou floue.
- [ ] **Vous avez besoin d'un registre partagé et non modifiable** que les deux côtés et votre auditeur peuvent lire.
- [ ] **Vous pouvez fixer un plafond de dépense dur** et un arrêt en un clic avant d'automatiser.
- [ ] **Aucune donnée personnelle n'a besoin de siéger sur le registre permanent.**
- [ ] **Un chemin de litige existe** et nomme un humain qui peut renverser la règle.
- [ ] **Vous l'avez comparé honnêtement** à un contrat normal et un processus normal, et le « trustless » gagne encore en coût, vitesse ou risque.

## Points clés à retenir

- « Trustless » ne veut pas dire pas de confiance ; cela veut dire que vous vérifiez un fait au lieu de faire confiance à une personne pour le dire.
- Les trois pièces qui fonctionnent sont une identité vérifiable, des registres infalsifiables, et l'application automatique d'une condition écrite.
- Le projet ERC-8004 d'Ethereum et les standards d'abstraction de compte montrent où va le business d'agent à agent : identité, réputation et validation indépendante, avec des budgets bornés par le code.
- Le maillon faible est le déclencheur — le moment où un humain ou un capteur dit au système ce qui s'est vraiment passé.
- N'utilisez pas le « trustless » là où un contrat normal fonctionne ; utilisez-le là où la vérification coûte cher, le déclencheur est mesurable, et la perte maximale est plafonnée.
