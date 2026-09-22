# Chapitre 16 — Objectifs, coûts et retour sur investissement

## En mots simples

Avant de dépenser de l'argent dans l'IA, vous devez répondre à trois questions simples. Que voulez-vous accomplir ? Combien cela coûtera-t-il ? Que récupérerez-vous ? Si vous ne pouvez pas répondre à cela, vous ne prenez pas une décision — vous devinez. Ce chapitre vous donne une façon simple et honnête d'y répondre.

L'idée centrale s'appelle le **ROI**, qui signifie **Retour sur Investissement**. En mots simples, le ROI mesure combien de valeur vous récupérez pour chaque unité d'argent que vous investissez. Si vous dépensez un euro et récupérez trois euros de valeur, c'est un bon retour. Si vous dépensez un euro et récupérez cinquante centimes, c'est un mauvais. Le ROI transforme un vague « est-ce que ça en vaut la peine ? » en un nombre avec lequel vous pouvez réfléchir.

Ce chapitre est le **foyer de la méthode ROI** pour ce livre. La formule simple, comment l'utiliser, et un exemple chiffré vivent tous ici. Quand d'autres chapitres parlent de mesurer les résultats ou le retour, ils pointent vers celui-ci. Apprenez la méthode ici une fois, et vous pouvez l'appliquer à tout projet d'IA.

Une image simple à garder : le ROI, c'est comme vérifier si une machine dans votre atelier vaut la peine d'être achetée. Vous demandez ce qu'elle coûte à acheter et à faire tourner, et combien d'argent ou de temps elle vous fait économiser. Si elle économise plus qu'elle ne coûte, elle se rembourse et puis encore un peu. Sinon, c'est un ornement cher. L'IA ne fait pas exception — sauf que ses coûts et ses bénéfices sont parfois cachés, donc vous devez chercher plus fort pour les deux.

Un avertissement honnête dès le départ : les nombres peuvent mentir si vous le voulez. Il est facile de gonfler les économies et de réduire les coûts pour faire paraître bonne une mauvaise idée. La méthode ici est conçue pour vous garder honnête. Utilisez-la ainsi, pas comme un moyen de justifier une décision déjà prise.

## Un peu d'histoire

**Début des années 1900 : le ROI naît pour les usines.** Un gestionnaire nommé Donaldson Brown, travaillant chez DuPont dans les années 1910 et 1920, a développé une façon de comparer à quel point différentes parties d'une entreprise utilisaient leur argent. Il l'a exprimé comme un ratio du profit sur l'argent investi. Cela permettait aux patrons de comparer une usine à une autre et de décider où mettre le prochain dollar. C'était une petite idée avec une énorme influence — elle a fait du « retour » un nombre que l'on pouvait piloter.

**Milieu des années 1900 : le délai de récupération.** Les entreprises ont ajouté un cousin plus simple du ROI : combien de temps avant que les économies couvrent le coût ? Si une machine se rembourse en deux ans, cela semblait sûr. Si cela prenait quinze ans, cela semblait risqué. Le délai de récupération est devenu une vérification rapide d'instinct pour les gros achats.

**Années 1980-1990 : les limites de compter l'argent.** Les gestionnaires ont réalisé que certaines des choses les plus importantes — satisfaction client, qualité, apprentissage, moral des employés — n'apparaissaient pas dans un simple chiffre de profit. Le « tableau de bord prospectif », développé par Kaplan et Norton au début des années 1990, a essayé de capturer ces éléments à côté de l'argent. La leçon : comptez ce qui compte, pas seulement ce qui est facile à compter.

**Années 2000 : les projets tech et le paradoxe de la productivité.** Les entreprises ont déversé de l'argent dans des logiciels et parfois vu peu de retour, menant à une blague célèbre voulant que les ordinateurs apparaissent partout dans les chiffres de l'économie sauf dans la productivité. La cause était rarement la technologie. C'étaient des objectifs vagues, des coûts cachés et une mauvaise adoption. Mesurer les bonnes choses est devenu une discipline à part entière.

**Années 2020 : l'IA impose un calcul honnête.** L'IA peut économiser du temps et de l'argent réels, mais ses coûts sont faciles à sous-estimer (abonnements, mise en place, formation, maintenance) et ses bénéfices faciles à surestimer (économies gonflées, courbes d'apprentissage ignorées). Une méthode ROI simple et honnête est désormais essentielle pour séparer les outils qui rapportent de ceux qui sonnent bien.

L'arc : d'un ratio d'usine à une discipline moderne. Les outils ont changé ; la question centrale n'a jamais changé — avez-vous récupéré plus que ce que vous avez investi ?

## Curiosité

### 16.7 L'entreprise qui a réduit le temps de résolution des questions de 99 %

L'un des exemples les plus frappants récemment de l'effet de l'IA sur un processus d'entreprise est la société de santé animale **Elanco**, qui a déclaré avoir réduit le temps de résolution de certaines questions internes d'information d'environ **99 %** après avoir mis au travail un assistant IA génératif — transformant une recherche qui prenait autrefois de nombreuses minutes en une réponse quasi instantanée.

Cela, c'est le titre. Le cas complet, avec les détails et les leçons derrière le nombre, est raconté au [Chapitre 25 — Administration et Finance](ch25-administration-and-finance.md), le foyer canonique de l'histoire d'Elanco. Le point pour ce chapitre tient en une ligne : une énorme économie de temps est un bénéfice réel et mesurable — et c'est exactement le genre de chose qu'un bon calcul de ROI est conçu pour capturer.

## Un exemple d'entreprise réel

*Ce qui suit est une illustration composite de schémas courants du monde réel, pas une seule entreprise nommée.*

Une entreprise de logistique voulait « utiliser l'IA », alors elle a acheté un chatbot pour les questions clients. Personne n'a fixé d'objectif clair d'abord. Six mois plus tard, le patron a demandé : « Est-ce que ça marche ? » et personne n'a pu répondre. Il n'y avait pas de chiffre de départ à comparer, donc pas moyen de dire si quoi que ce soit s'était amélioré. L'outil aidait probablement un peu, mais l'entreprise ne pouvait pas le prouver, pas le dimensionner, et pas décider s'il fallait l'étendre ou l'arrêter. L'argent était dépensé, et la leçon était perdue.

Une seconde entreprise a fait l'inverse. Avant d'acheter quoi que ce soit, elle a choisi un objectif clair : réduire le temps que son équipe passait à répondre aux mêmes dix questions clients répétées. Elle a mesuré le point de départ — environ 30 heures par semaine sur toute l'équipe. Elle s'est fixé une cible : la moitié, en trois mois. Elle a compté les coûts honnêtement, y compris le temps de mise en place et de formation. À la fin, elle avait un vrai chiffre avant-après et un vrai chiffre de coût, et elle pouvait calculer un retour clair. La décision de s'étendre a été facile parce que le calcul était clair.

La différence n'était pas l'IA. C'est que la seconde entreprise avait défini un objectif et l'avait mesuré avant de dépenser un euro. C'est ce que le reste de ce chapitre vous apprend à faire.

## Comment faire

### 16.1 Définir des objectifs simples et mesurables

Un objectif que vous ne pouvez pas mesurer est un souhait, pas un objectif. « Mieux utiliser l'IA » est un souhait. « Réduire de moitié le temps de traitement des factures d'ici juin » est un objectif. La première étape de tout calcul de ROI est de transformer votre intention en quelque chose que vous pouvez mesurer.

Un bon objectif a quatre parties :

- **Une métrique.** Choisissez un seul nombre qui compte — heures passées, coût par article, erreurs commises, temps de réponse, ventes conclues. Pas cinq nombres. Un.
- **Une référence.** Que vaut ce nombre *en ce moment* ? Mesurez-le avant de commencer. Sans référence, vous ne pouvez jamais prouver le changement. Si vous ne connaissez pas votre temps actuel de facturation, allez le mesurer cette semaine.
- **Une cible.** Que voulez-vous qu'il devienne ? Soyez précis : « la moitié », « deux minutes au lieu de dix », « dix erreurs de moins par semaine ».
- **Un horizon de temps.** Pour quand ? « Dans trois mois » donne à l'objectif une échéance et le rend réel.

Restez simple. Une petite entreprise n'a pas besoin d'un tableau de bord de cinquante métriques. Une métrique claire par projet, avec une référence et une cible, suffit pour piloter une vraie décision.

Écrivez l'objectif en une phrase : *« D'ici [quand], nous changerons [métrique] de [référence] à [cible]. »* Si vous ne pouvez pas remplir ces blancs, vous n'êtes pas prêt à dépenser. Retournez en arrière et définissez-le. Cette seule habitude prévient la plupart des dépenses d'IA gaspillées.

### 16.2 Coûts directs et indirects

Le prix affiché n'est pas le coût. La plupart des gens comptent l'abonnement et s'arrêtent là. Le vrai coût est plus grand, et les parties cachées sont ce qui transforme un projet d'apparence séduisante en puits à argent. Comptez les deux sortes.

**Coûts directs** sont les évidents que vous payez :

- **Logiciels et abonnements.** Le frais mensuel ou annuel pour l'outil d'IA.
- **Mise en place et intégration.** Le travail pour connecter l'outil à vos systèmes existants.
- **Matériel.** Tout équipement que vous devez acheter.
- **Aide externe.** Consultants, développeurs ou formateurs que vous payez.
- **Formation.** Le coût pour apprendre aux gens à l'utiliser.

**Coûts indirects** sont les cachés que les gens oublient :

- **Le temps du personnel pour le mettre en place et le faire tourner.** Les heures que vos propres gens passent à configurer, tester et gérer l'outil. C'est de l'argent réel, même si aucune facture ne le montre.
- **Le creux d'apprentissage.** Quand vous changez la façon dont les gens travaillent, ils ralentissent avant d'accélérer. Quelques semaines de productivité plus basse sont normales et coûtent quelque chose.
- **Maintenance et mises à jour.** Les outils ont besoin d'entretien — réparer les pannes, mettre à jour les réglages, gérer les nouveaux cas.
- **Revue et vérification.** Le temps humain pour vérifier le résultat de l'IA, que vous ne devriez jamais sauter.
- **Gouvernance et conformité.** L'effort pour garder l'outil dans les règles de vie privée et légales (voir [Chapitre 10](ch10-privacy-and-gdpr.md)).
- **Coûts de changement et de sortie.** Ce que coûte le fait de changer d'outil plus tard si celui-ci déçoit.

Une bonne règle : le prix visible n'est souvent que la moitié du vrai coût. Additionnez chaque coût auquel vous pouvez penser, y compris le temps de vos propres gens, et valorisez ce temps à ce qu'il vous coûte vraiment (salaire plus frais généraux, pas seulement le net à percevoir). Sous-estimer le coût est la façon la plus courante dont les gens se trompent eux-mêmes.

### 16.3 Bénéfices quantifiables et non quantifiables

Les bénéfices viennent en deux sortes. Certains peuvent être mis en nombre. D'autres non, mais ils comptent quand même. Un bon calcul traite les deux honnêtement.

**Bénéfices quantifiables** peuvent être transformés en argent :

- **Temps économisé.** Heures non passées sur une tâche, valorisées au coût de ce temps.
- **Erreurs évitées.** Moins d'erreurs signifie moins de remboursements, de reprises et de pénalités.
- **Cycles plus rapides.** Des factures plus rapides sont payées plus tôt ; des devis plus rapides gagnent plus d'affaires.
- **Plus de ventes ou de production.** Si l'IA vous aide à servir plus de clients ou produire plus.
- **Coûts de main-d'œuvre ou de matériaux plus bas.** Économies directes que vous pouvez montrer du doigt.

**Bénéfices non quantifiables** sont réels mais difficiles à chiffrer :

- **Satisfaction des employés.** Les gens peuvent aimer davantage leur travail quand les parties ennuyeuses sont automatisées.
- **Expérience client.** Un service plus rapide et plus clair rend les clients plus heureux, même si vous ne pouvez pas y accrocher un nombre aujourd'hui.
- **Moins de stress et moins de nuits tardives.** Gains de qualité de vie qui n'apparaissent pas dans un tableur.
- **De meilleures décisions.** L'IA peut faire surface des informations qui améliorent le jugement.
- **Réputation et prontitude.** Être une entreprise qui utilise bien les outils modernes.

Comment traiter les deux : **monétisez ce que vous pouvez honnêtement, et écrivez le reste à part.** Ne forcez pas un faux nombre sur quelque chose d'intangible. Ne faites pas semblant non plus que l'intangible vaut zéro. Listez-le, nommez-le, et pesez-le dans votre jugement à côté des chiffres durs. Un projet avec de modestes économies d'argent mais de gros gains en moral du personnel et bonheur client peut quand même valoir la peine d'être fait. Le point est de voir le tableau entier, pas un faux nombre unique.

### 16.4 Un calcul simple du ROI

Maintenant la méthode elle-même. La formule de base est simple.

**ROI = (Bénéfice net ÷ Coût total) × 100 %**

Où **Bénéfice net = Bénéfice total − Coût total**.

Un ROI positif signifie que vous avez gagné plus que vous n'avez dépensé. Un ROI négatif signifie que vous avez perdu de l'argent. Plus le pourcentage est élevé, meilleur est le retour.

**Un petit exemple chiffré.** Supposons qu'un outil d'IA coûte **10 000 €** au total pour la première année (abonnement plus mise en place plus formation). Vous mesurez qu'il fait économiser à votre équipe **25 000 €** de temps et d'erreurs sur cette année.

- Bénéfice net = 25 000 € − 10 000 € = **15 000 €**
- ROI = (15 000 € ÷ 10 000 €) × 100 % = **150 %**

Un retour de 150 % signifie que pour chaque euro dépensé, vous avez récupéré votre euro plus 1,50 € en plus. C'est un retour solide.

Le **délai de récupération** est le nombre compagnon : combien de temps avant que les économies couvrent le coût ? Si vous économisez 25 000 € par an, cela fait environ 2 083 € par mois. Pour couvrir un coût de 10 000 €, il faut environ **4,8 mois**. Après cela, les économies sont du pur gain.

Comment lire le résultat :

- **ROI clairement positif et récupération courte** (quelques mois) — un bon dossier pour avancer.
- **ROI positif mais récupération longue** (plusieurs années) — réfléchissez bien ; la marge est mince et des risques pourraient l'effacer.
- **ROI proche de zéro ou négatif** — l'outil ne se rembourse pas sur les chiffres que vous avez. Trouvez plus de bénéfice, coupez le coût, ou partez.

Deux habitudes honnêtes rendent cette méthode fiable. D'abord, utilisez votre vraie référence et votre coût complet, pas des estimations optimistes. Ensuite, faites le calcul sur une période claire (généralement un an) et répétez-le après le lancement avec des chiffres réels, pas des projections. Le premier calcul est une estimation pour décider ; le second est la vérité dont apprendre.

### 16.5 Exemple : automatiser les factures

Voici la méthode complète appliquée à un cas courant — l'automatisation du traitement des factures. *Tous les chiffres sont illustratifs ; remplacez-les par les vôtres.*

**La mise en place.** Une petite entreprise traite **2 000 factures par mois** (24 000 par an). En ce moment, le personnel les fait à la main.

**Étape 1 — Référence.** Chaque facture prend environ **10 minutes** à la main. Cela fait 240 000 minutes par an = **4 000 heures par an**. À un coût complet du personnel de **25 € de l'heure**, le travail manuel coûte environ **100 000 € par an**.

**Étape 2 — Ce que l'IA change.** L'outil automatise complètement environ **80 %** des factures, réduisant chacune d'entre elles de 10 minutes à environ 2 minutes de revue humaine. Il économise donc 8 minutes sur 19 200 factures (80 % de 24 000). Cela fait 153 600 minutes = **2 560 heures par an économisées**. À 25 €/heure, le **bénéfice brut est d'environ 64 000 € par an**.

**Étape 3 — Coût total.** Abonnement logiciel **12 000 €/an**, mise en place ponctuelle **8 000 €**, formation **2 000 €**. Coût total de la première année = **22 000 €**. Les années stables d'après, le coût tombe à environ **14 000 €** (abonnement plus maintenance).

**Étape 4 — ROI, première année.**
- Bénéfice net = 64 000 € − 22 000 € = **42 000 €**
- ROI = (42 000 € ÷ 22 000 €) × 100 % ≈ **191 %**

**Étape 5 — Récupération.** Économies mensuelles ≈ 64 000 € ÷ 12 ≈ 5 333 €. Pour couvrir le coût de 22 000 € de la première année, il faut environ **4 mois**.

**Étape 6 — État stable (année deux).**
- Bénéfice net = 64 000 € − 14 000 € = **50 000 €**
- ROI = (50 000 € ÷ 14 000 €) × 100 % ≈ **357 %**

**Lecture.** La première année rend environ 191 % et se rembourse en environ quatre mois. Après cela, le retour grimpe parce que les coûts ponctuels ont disparu. C'est un dossier clair et solide — et vous voyez exactement pourquoi, car chaque chiffre vient d'une référence mesurée et d'une liste de coûts complète. Maintenant imaginez faire cela avec *votre* nombre de factures, *votre* temps par facture, et *vos* coûts. C'est le calcul qui décide votre vrai choix.

## Éthique et responsabilité

Le ROI est un outil pour des décisions honnêtes, et il peut être mal utilisé.

**Ne gonflez pas les économies pour justifier des licenciements.** La façon la plus facile de faire paraître bon un mauvais projet est de surestimer les économies puis de couper des gens. Utilisez des chiffres honnêtes, et décidez des gens séparément et humainement (voir [Chapitre 15](ch15-people-roles-and-culture.md)).

**Comptez le coût humain.** Le creux d'apprentissage, le stress du changement, le temps que les gens passent à s'adapter — ce sont de vrais coûts. Laissez-les dans le calcul. Un chiffre propre qui cache une réalité désordonnée est un chiffre malhonnête.

**Ne truquez pas la référence.** Si vous faites paraître le point de départ pire qu'il n'était, l'amélioration paraît plus grande qu'elle n'est. Mesurez la référence honnêtement, avant d'avoir un intérêt au résultat.

**Valorisez le non quantifiable.** Ne traitez pas le moral du personnel, le bonheur client et le stress réduit comme zéro juste parce qu'ils n'ont pas de nombre. Ils appartiennent à la décision, même si seulement dans votre jugement.

**Soyez transparent avec les parties prenantes.** Si vous rapportez le ROI à un conseil, un partenaire ou un prêteur, montrez vos hypothèses et votre méthode, pas seulement le chiffre titre. Laissez les autres vérifier votre travail.

**Séparez la décision d'argent de la décision sur les gens.** Un ROI positif ne signifie pas automatiquement « couper du personnel ». Cela signifie que l'outil se rembourse. Ce que vous faites du temps et de l'argent libérés est un choix humain séparé.

Un calcul de ROI honnête vous protège de vous tromper vous-même et protège vos gens d'être une ligne dans un chiffre truqué.

## Erreurs à éviter

### 16.6 Erreurs d'évaluation

**Pas d'objectif clair.** Dépenser sans but mesurable, donc vous ne pouvez jamais dire si ça a marché. Définissez d'abord la métrique.

**Pas de référence.** Ne pas mesurer le point de départ, donc tout changement est improbable. Mesurez avant de commencer.

**Ignorer les coûts indirects.** Compter seulement l'abonnement et oublier la mise en place, le temps du personnel, le creux d'apprentissage et la maintenance. Les coûts cachés sont là où les projets meurent.

**Surestimer les économies.** Croire la promesse du meilleur cas du fournisseur au lieu de votre propre réalité mesurée. Soyez conservateur.

**Compter le brut au lieu du net.** Rapporter le bénéfice total sans soustraire le coût. Le ROI porte sur le gain *net*.

**Double comptage.** Compter la même économie deux fois, ou compter un bénéfice qui se recoupe avec un déjà compté.

**Ignorer la courbe d'apprentissage.** Supposer des économies complètes dès le premier jour. Les vraies économies montent sur des semaines.

**Un horizon temporel trop court.** Juger un outil après deux semaines, avant que les bénéfices apparaissent. Donnez-lui une période équitable, généralement un an.

**Ignorer la maintenance.** Oublier que les coûts continuent après le lancement. Un outil qui a besoin d'un entretien constant peut ne jamais se rembourser.

**Traiter le non quantifiable comme zéro.** Jeter de vrais bénéfices parce qu'ils n'ont pas de nombre. Listez-les et pesez-les.

**Théâtre du ROI.** Faire le calcul à l'envers pour justifier une décision déjà prise. Utilisez la méthode pour décider, pas pour décorer.

**Ne jamais refaire les chiffres.** Rester sur la projection et ne jamais vérifier contre la réalité. Remezurez après le lancement et apprenez.

## Exercice pratique

### 16.8 Calculez le ROI d'une activité

Choisissez une activité dans votre entreprise que l'IA pourrait aider — répondre aux emails, traiter les factures, résumer des documents, planifier. Faites la méthode complète dessus.

**Étape 1 — Définissez l'objectif.** Écrivez une phrase : *« D'ici [quand], nous changerons [métrique] de [référence] à [cible]. »* Si vous ne connaissez pas la référence, allez la mesurer cette semaine avant de continuer.

**Étape 2 — Mesurez la référence.** Combien de temps ou d'argent cette activité vous coûte-t-elle maintenant, par mois ou par an ? Pour le temps, multipliez les heures par un coût horaire complet (salaire plus frais généraux). Écrivez le nombre.

**Étape 3 — Listez tous les coûts.** Coûts directs (abonnement, mise en place, matériel, aide externe, formation) plus coûts indirects (le temps de votre personnel pour le mettre en place et le faire tourner, le creux d'apprentissage, la maintenance, le temps de revue). Additionnez-les en un total de première année et un total d'année stable.

**Étape 4 — Estimez le bénéfice.** Combien de temps ou d'argent l'IA économisera-t-elle réellement ? Soyez conservateur. Utilisez une fraction de la référence que vous avez mesurée, pas une fantaisie. Convertissez le temps économisé en argent à votre coût horaire.

**Étape 5 — Calculez le ROI.** Bénéfice net = Bénéfice total − Coût total. ROI = (Bénéfice net ÷ Coût total) × 100 %.

**Étape 6 — Calculez la récupération.** Divisez le coût total par vos économies mensuelles pour voir combien de mois avant que cela se rembourse.

**Étape 7 — Listez les bénéfices non quantifiables.** Écrivez les bénéfices que vous ne pouvez pas chiffrer — moral, bonheur client, moins de stress. Notez-les à côté du nombre.

**Étape 8 — Décidez.** Le ROI est-il clairement positif avec une récupération courte ? Bon dossier. Marge mince ? Soyez prudent. Négatif ? Partez ou trouvez plus de bénéfice.

Écrivez tout cela sur une page. Cette page est votre décision. Gardez-la, et après le lancement, remplissez les chiffres *réels* et comparez. L'écart entre votre estimation et la réalité est la leçon que vous porterez au prochain projet.

## Liste de contrôle

### 16.9 Liste de contrôle économique

Avant de dépenser dans un projet d'IA, vérifiez ceci.

- [ ] **Vous avez un objectif clair et mesurable** avec une seule métrique.
- [ ] **Vous avez mesuré la référence** (le nombre actuel) avant de commencer.
- [ ] **Vous avez une cible spécifique et un horizon de temps.**
- [ ] **Vous avez listé tous les coûts directs** — abonnement, mise en place, matériel, aide externe, formation.
- [ ] **Vous avez listé tous les coûts indirects** — temps du personnel, creux d'apprentissage, maintenance, revue, conformité.
- [ ] **Vous avez valorisé le temps du personnel à un taux complet**, pas juste le net à percevoir.
- [ ] **Vous avez estimé les économies prudemment**, pas à partir du battage du fournisseur.
- [ ] **Vous avez calculé le bénéfice net** (bénéfice total moins coût total).
- [ ] **Vous avez calculé le ROI** = (Bénéfice net ÷ Coût total) × 100 %.
- [ ] **Vous avez calculé le délai de récupération** en mois.
- [ ] **Vous avez listé les bénéfices non quantifiables** et les avez pesés dans votre jugement.
- [ ] **Vous avez utilisé un horizon temporel équitable** (environ un an), pas quelques semaines.
- [ ] **Vous n'avez rien compté deux fois.**
- [ ] **Vous referez les chiffres avec les résultats réels** après le lancement.
- [ ] **Vous avez gardé la décision d'argent séparée de la décision sur les gens.**

Si une case est vide, l'économie n'est pas réglée. Remplissez-la avant de dépenser. Un nombre auquel vous pouvez vous fier vaut plus qu'une promesse que vous ne pouvez pas vérifier.

## Points à retenir

- ROI = (Bénéfice net ÷ Coût total) × 100 %, où Bénéfice net = Bénéfice total − Coût total ; un nombre positif avec une récupération courte est un bon dossier pour avancer.
- Définissez un objectif mesurable avec une vraie référence avant de dépenser — sans chiffre de départ, vous ne pouvez jamais prouver le changement.
- Le prix visible n'est que la moitié du coût ; comptez les coûts indirects comme le temps du personnel, le creux d'apprentissage et la maintenance, sinon vous vous tromperez vous-même.
- Monétisez ce que vous pouvez honnêtement et écrivez le reste — les bénéfices non quantifiables comme le moral et le bonheur client appartiennent quand même à la décision.
- Utilisez la méthode pour décider, pas pour décorer : des chiffres honnêtes vous protègent des mauvais choix et vos gens d'être une ligne truquée.
