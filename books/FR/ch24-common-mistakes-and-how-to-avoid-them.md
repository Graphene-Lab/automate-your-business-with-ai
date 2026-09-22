# Chapitre 24 — Les erreurs fréquentes et comment les éviter

## En termes simples

La plupart des projets d'IA échouent pour les mêmes quelques raisons. Pas parce que la technologie est faible, mais à cause d'erreurs prévisibles que les gens répètent sans fin. La bonne nouvelle, c'est qu'une fois que vous connaissez ces erreurs, vous pouvez presque toutes les éviter. Ce chapitre est une visite guidée des plus grosses, avec la solution pour chacune.

Voyez-le comme une liste de mines. Chacune est facile sur laquelle on marche si l'on ne sait pas qu'elle est là, et facile à contourner si on le sait. Le but n'est pas de vous faire peur de l'IA. C'est de faire de vous le genre de chef d'entreprise qui ne fait pas sauter son propre projet par accident.

Les six grandes erreurs sont : automatiser le mauvais processus, sous-estimer les données et les gens, faire trop confiance à l'IA, démarrer trop gros, ignorer les règles et la sécurité, et ne pas mesurer les résultats. Chacune est courante, chacune coûte cher, et chacune a une façon claire de l'éviter. Nous les prenons une par une, nous expliquons pourquoi elle arrive et ce qu'elle coûte, et nous vous renvoyons au chapitre qui traite la solution en détail.

Une image simple à garder en tête : adopter l'IA, c'est comme partir pour une longue marche à travers la campagne. La plupart des gens n'échouent pas parce que la route est impossible. Ils échouent parce qu'ils ont choisi la mauvaise destination, emporté trop peu d'eau, fait confiance à une carte fautive, voulu marcher trop loin dès le premier jour, ignoré la météo, et jamais vérifié s'ils allaient dans la bonne direction. Les erreurs sont ordinaires et évitables. Ce chapitre est le briefing de sécurité avant le départ.

Lisez-le comme une liste de contrôle face à vos propres plans. Si vous vous reconnaissez dans l'un de ces cas, arrêtez-vous et corrigez avant de dépenser plus d'argent ou de griller davantage de confiance.

## Un peu d'histoire

**Années 1980 : l'effondrement des systèmes experts a enseigné la leçon du mauvais processus.** Pendant le boom des systèmes experts, les entreprises ont déversé de l'argent pour encoder les règles des experts humains. Beaucoup de projets ont échoué parce qu'ils ont essayé d'automatiser des tâches trop désordonnées, trop rares, ou trop dépendantes du jugement pour être encodées. Les systèmes étaient fragiles et coûteux à mettre à jour, et le marché s'est effondré. La leçon : automatiser la mauvaise chose gaspille une fortune, aussi bonne soit la technologie.

**Années 1990 : « poubelle dedans, poubelle dehors » est devenu un mantra.** À mesure que les entreprises se sont informatisées, elles ont appris qu'un système nourri de mauvaises données produit de mauvais résultats, aussi intelligent soit le logiciel. Ce vieux dicton de l'informatique est devenu central dans chaque projet de données. C'est l'ancêtre de l'erreur d'aujourd'hui : « sous-estimer les données ».

**Années 1990-2000 : le schéma d'échec du big-bang.** Les projets de logiciels d'entreprise des années 1990 et 2000 étaient célèbres pour partir en « big-bang » — tout remplacer d'un coup, selon un grand plan, sur plusieurs années. Beaucoup ont dépassé le budget, dépassé les délais, et échoué carrément. Le schéma était si courant que « mise en œuvre big-bang » est devenu un terme d'avertissement. La solution qui en est sortie : commencer petit, prouver la valeur, puis grandir. C'est l'ancêtre de « démarrer trop gros ».

**Années 2000 : la complaisance face à l'automatisation.** Des chercheurs étudiant les systèmes automatisés — pilotes automatiques, surveillance automatisée — ont découvert un échec surprenant : quand un système fonctionne bien la plupart du temps, les humains cessent de faire attention et lui font trop confiance. Puis il échoue sur un cas rare et personne ne le repère. On appelle cela la **complaisance face à l'automatisation** ou le **biais d'automatisation**, et c'est exactement l'erreur de « faire trop confiance à l'IA ». Elle a été documentée bien avant les chatbots et elle est plus pertinente que jamais.

**Années 2010 : la réglementation rattrape tout le monde.** À mesure que les fuites de données et les mauvais usages faisaient la une, les gouvernements ont commencé à écrire des règles strictes — le RGPD en Europe étant le plus important. Les entreprises qui avaient traité les données à la légère se sont retrouvées face à de lourdes amendes et à des risques juridiques. La leçon : ignorer les règles n'est pas un raccourci ; c'est une responsabilité en attente d'être déclenchée.

**Années 2020 : les mêmes vieilles erreurs, une nouvelle technologie.** La vague d'IA actuelle répète chacune de ces erreurs à toute vitesse. Des outils bon marché et impressionnants rendent facile de démarrer gros, de faire trop confiance, de sauter le travail sur les données, d'ignorer les règles et de sauter la mesure. La technologie est nouvelle ; les modes d'échec sont vieux et bien documentés. Connaître l'histoire est la défense la moins chère qui soit.

Le fil conducteur : chaque génération de technologies d'entreprise a fait les mêmes quelques erreurs. Aucune n'est nouvelle. Toutes sont évitables si vous les avez déjà vues.

## Curiosité

### 24.7 L'effet Eliza : pourquoi nous faisons plus confiance aux machines qu'elles ne le méritent

Une raison pour laquelle les gens font trop confiance à l'IA remonte à un programme de conversation de 1966 appelé ELIZA et à l'habitude humaine qui porte son nom — l'**effet Eliza** : nous accordons volontiers de la compréhension et des sentiments à une machine qui ne fait que les imiter, et nous faisons plus confiance à ses résultats qu'ils ne le méritent.

L'histoire complète d'ELIZA, et pourquoi elle compte pour la façon dont vous concevez et supervisez tout outil d'IA, est racontée dans le [Chapitre 1 — Une brève histoire de l'IA](ch01-a-short-history-of-ai.md), la maison de référence de l'effet Eliza. Le rappel en une ligne ici : une machine fluide et polie nous fait trop lui faire confiance, et cette habitude est la racine de l'erreur 24.3 ci-dessous.

## Un exemple d'entreprise réel

*Ce qui suit est une illustration composite de schémas réels fréquents, pas une seule entreprise nommée.*

Une entreprise de commerce voulait « utiliser l'IA », alors elle a fait presque tout sur cette liste de travers, puis presque tout bien.

La version fausse : le propriétaire a lu des choses sur l'IA, s'est emballé, et a décidé de « transformer le service client ». Sans choisir de problème précis, il a acheté un chatbot et l'a déployé d'un coup sur toute sa clientèle. Il lui a donné une pile de vieux documents désordonnés en espérant le meilleur. Il a désactivé la vérification humaine parce que « l'IA est plus rapide ». Il n'a jamais vérifié si elle donnait des réponses correctes. En quelques semaines, le chatbot affirmait avec assurance aux clients de fausses politiques de retour et de faux prix. Les clients se sont plaints. L'entreprise n'en avait aucune idée jusqu'à ce que les plaintes s'accumulent. Le projet était un désastre, et le propriétaire a conclu : « l'IA ne marche pas ».

La version juste : après le désastre, le propriétaire a redémarré avec discipline. Il a choisi un petit problème clair — répondre aux dix questions « où en est ma commande ? » les plus courantes, qui dévoraient le temps du personnel. Il a d'abord vérifié les données et a trouvé qu'il disposait de données de suivi de commandes propres pouvant répondre à ces questions de façon fiable. Il a commencé par un petit pilote sur ces seules questions, avec un humain vérifiant chaque réponse. Il a mesuré le résultat : le temps de réponse a baissé, la satisfaction s'est maintenue, et les réponses étaient correctes parce que les données étaient bonnes et le périmètre étroit. Ce n'est qu'ensuite qu'il s'est étendu, pas à pas, en gardant la vérification humaine sur les cas plus difficiles.

La technologie était la même. La première tentative a échoué à cause de six erreurs. La seconde a fonctionné parce que chaque erreur a été évitée. La leçon n'est pas « l'IA est risquée ». La leçon est « les erreurs sont le risque, et elles sont évitables ».

## Comment faire

### 24.1 Automatiser le mauvais processus

L'erreur la plus coûteuse est de dépenser de l'argent pour automatiser quelque chose qui n'a jamais valu d'être automatisé. Un mauvais processus rapide reste mauvais, et maintenant il est mauvais à grande échelle.

**Pourquoi ça arrive.** L'enthousiasme. Vous avez un outil et vous voulez l'utiliser, alors vous le pointez sur ce qui se trouve devant vous au lieu de choisir avec soin. Ou vous automatisez un processus qui va déjà bien, faisant gagner un temps que personne n'avait besoin de gagner, pendant que le vrai goulot d'étranglement reste intact.

**Ce que ça coûte.** De l'argent dépensé pour un outil qui rapporte peu, plus le coût d'opportunité du vrai problème que vous n'avez pas résolu. Pire, une automatisation mal choisie peut aggraver les choses — automatiser un processus cassé produit simplement des résultats cassés plus vite et cache la casse.

**La solution : choisir avant d'acheter.** Avant tout outil, choisissez le processus par deux tests. D'abord, l'*impact* : ce compte-t-il vraiment ? Coûte-t-il du vrai temps, du vrai argent, ou du vrai bonheur client ? Ensuite, l'*adéquation* : le processus se prête-t-il à l'automatisation — répétitif, à base de règles ou d'exemples, avec des données disponibles ? La matrice impact-vers-facilité du [Chapitre 12 — Où l'IA peut aider votre entreprise](ch12-where-ai-can-help-your-business.md) est l'outil pour cela. Servez-vous-en. Choisissez la cible à fort impact et forte adéquation, pas la première chose à laquelle vous avez pensé.

**Réparez le processus avant de l'automatiser.** Si un processus est cassé, réparez-le d'abord, puis automatisez la version réparée. Automatiser un désordre vous donne un désordre automatisé. Parfois, la meilleure première étape est de simplifier ou de supprimer une étape entièrement, pas de l'automatiser.

### 24.2 Sous-estimer les données et les gens

L'IA tourne sur deux choses : les données et les gens. Les deux sont généralement plus difficiles et plus importantes que le modèle lui-même, et les deux sont régulièrement sous-estimées.

**L'erreur des données.** L'IA n'est bonne que dans la mesure des données que vous lui donnez. Des données désordonnées, incomplètes, périmées ou biaisées produisent des résultats désordonnés, incomplets, périmés ou biaisés — aussi bon soit l'outil. Les gens s'imaginent que l'IA va « se débrouiller » avec ce qu'ils ont. Elle ne le peut pas. Si vos dossiers sont un désordre, l'IA hérite du désordre. Le traitement complet de la qualité des données est dans le [Chapitre 14 — Les données : la matière première](ch14-data-the-raw-material.md). La version courte : vérifiez vos données avant d'attendre de bons résultats, et corrigez les données avant d'accuser l'IA.

**L'erreur des gens.** Comme le montre le Chapitre 15, un outil qui fonctionne en test peut rester inutilisé parce que personne n'a été informé de pourquoi il existe, personne n'a été formé, et personne ne s'est senti en sécurité. Les gens ne sont pas une note de bas de page ; ils sont la raison pour laquelle les projets vivent ou meurent. Sous-estimer le côté humain — la formation, la peur, la confiance, la gestion du changement — est l'une des causes d'échec les plus courantes. Les compétences de gestion du changement sont dans le [Chapitre 21](ch21-managing-change-in-your-company.md). Budgétez le travail humain aussi sérieusement que vous budgétez le logiciel.

**Pourquoi ça arrive.** Le travail sur les données et sur les gens est lent, ingrat et ennuyeux comparé à l'outil enthousiasmant. Il est tentant de les sauter pour arriver à la démo. Mais les sauter, c'est sauter les fondations. Le bâtiment s'écroule.

**La solution.** Traitez les données et les gens comme le projet principal, avec l'outil comme une partie de celui-ci, et non l'inverse. Passez du vrai temps à nettoyer et vérifier les données. Passez du vrai temps à former, communiquer et soutenir les gens. Ce n'est pas une charge ; c'est le travail.

### 24.3 Faire trop confiance à l'IA

L'IA moderne produit des résultats fluides, assurés, bien écrits. Cette fluidité nous trompe et nous fait lui faire plus confiance qu'elle ne le mérite. C'est le biais d'automatisation, et c'est l'erreur la plus dangereuse de la liste, parce qu'elle transforme un outil en décideur sans surveillance.

**Pourquoi ça arrive.** Une réponse assurée et bien écrite *semble* correcte. Notre cerveau confond « sonne bien » avec « est vrai ». Ajoutez l'effet Eliza — notre habitude d'accorder de la compréhension à une machine polie — et il est facile de cesser de vérifier. Si l'outil a raison 95 % du temps, les 5 % où il a tort passent à travers parce que personne ne regarde.

**Ce que ça coûte.** De fausses réponses qui atteignent les clients. De faux chiffres dans les rapports. De fausses décisions prises sur des résultats assurés mais faux. Les dégâts sont d'autant pires que le résultat avait l'air digne de confiance, alors personne ne l'a remis en question avant qu'il ne soit trop tard. Rappelez-vous la leçon du Chapitre 1 : la fluidité n'est pas la vérité.

**La solution : garder l'humain dans la boucle.** Ne laissez jamais un résultat de l'IA sortir sans vérification, surtout vers les clients ou dans des décisions qui comptent. Fixez une règle ferme : l'IA rédige, un humain vérifie et envoie. Apprenez aux gens *comment* vérifier — quoi chercher, à quoi ressemble une mauvaise réponse — pas seulement à appuyer sur un bouton. La compétence de vérification est plus importante que l'outil.

**Méfiez-vous des absurdités assurées.** L'IA peut être fausse avec assurance. Plus le résultat est assuré et fluide, plus vous devez le vérifier soigneusement, et non moins. Entraînez votre instinct à vous méfier des réponses lisses sur ce qui compte. L'état d'esprit sans-confiance du [Chapitre 7 — Sans-confiance : faire confiance sans se fier](ch07-trustless-trust-without-trusting.md) est le bon cadre : vérifiez, ne faites pas confiance par défaut.

**Fixez des règles d'escalade.** Décidez ce que l'IA peut faire seule et ce qui doit remonter à un humain. Les cas à enjeu élevé, inhabituels ou ambigus vont à une personne. L'IA gère la routine ; l'humain gère l'important et l'étrange.

### 24.4 Démarrer trop gros

Le déploiement big-bang — tout changer d'un coup selon un grand plan — est un échec classique. Il est tentant parce qu'il semble ambitieux, mais c'est la façon la plus sûre de perdre le contrôle.

**Pourquoi ça arrive.** L'ambition et l'impatience. Vous voulez la grande transformation maintenant, alors vous partez large et vite. Ou vous voulez impressionner, alors vous choisissez le plus grand périmètre possible. Le gros semble audacieux ; en pratique, il est fragile.

**Ce que ça coûte.** Les gros projets sont difficiles à contrôler, coûteux à réparer quand ils déraillent, et lents à montrer de la valeur. Un défaut qui serait petit dans un pilote devient une crise quand il est multiplié dans toute l'entreprise avant que vous ne le voyiez. Les projets big-bang dépassent souvent le budget et les délais, et beaucoup échouent carrément.

**La solution : commencer petit et prouver la valeur.** Choisissez une seule tâche étroite, une seule équipe, un seul objectif clair. Lancez un pilote. Mesurez-le. Si ça marche, montez par étapes (Chapitre 23). Petit n'est pas timide ; petit est la façon d'apprendre à bon marché et de garder le contrôle. Chaque petite victoire construit la compétence et la preuve pour l'étape suivante. L'approche des victoires étroites est la même que celle que le Chapitre 1 recommande à partir de l'histoire : l'IA gagne une chose précise à la fois, et vous aussi.

**L'ambition est bonne ; la séquence est la discipline.** Vous pouvez avoir une grande vision. Atteignez-la juste par une chaîne de petites étapes prouvées, pas un seul bond géant. La destination peut être grande ; la première étape doit être petite.

### 24.5 Ignorer les règles et la sécurité

L'IA touche vos données, les données de vos clients et vos décisions. Cela veut dire qu'elle touche la loi et votre sécurité. Ignorer les deux n'est pas un raccourci ; c'est une responsabilité chargée.

**Pourquoi ça arrive.** Les règles et la sécurité semblent lentes, complexes et loin — jusqu'à ce qu'elles ne le soient plus. Il est tentant d'aller vite et de traiter la conformité « plus tard ». Plus tard arrive souvent sous forme d'amende, de fuite ou de procès.

**Ce que ça coûte.** De lourdes amendes pour violation des règles de confidentialité. Une fuite de données qui expose les informations clients et détruit la confiance. Une responsabilité juridique pour des décisions prises par l'IA qui ont enfreint une règle. Le coût de l'ignorance est bien plus grand que celui d'un traitement correct, et il s'abat d'un coup.

**La solution : connaître les règles qui vous concernent.** Si vous traitez des données personnelles en Europe ou à son sujet, le RGPD s'applique — traité dans le [Chapitre 10 — Confidentialité et RGPD](ch10-privacy-and-gdpr.md). Si votre usage de l'IA relève de l'AI Act européen, ses obligations s'appliquent — traité dans le [Chapitre 5 — Règles et responsabilité juridique](ch05-rules-and-legal-responsibility.md). Vous n'avez pas besoin d'être avocat, mais vous devez savoir quelles règles vous touchent et les suivre. Prenez conseil là où c'est important.

**Prenez la sécurité au sérieux dès le premier jour.** Les outils d'IA manipulent souvent des données sensibles. Traitez ces données avec le même soin que vous traiteriez du cash dans un coffre. Les menaces de sécurité propres à l'ère de l'IA — fuites de données, injection de prompt, exposition au fournisseur — sont traitées dans le [Chapitre 6 — Cybersécurité à l'ère de l'IA](ch06-cybersecurity-in-the-ai-era.md). Ne greffez pas la sécurité plus tard ; intégrez-la dès le départ.

**La conformité n'est ni facultative ni une ligne d'arrivée.** Les règles changent, et votre usage de l'IA change. La conformité est continue, comme l'entretien. Intégrez-la à votre façon de fonctionner, pas à un contrôle ponctuel que vous sautez.

### 24.6 Ne pas mesurer les résultats

Si vous ne mesurez pas, vous ne pouvez pas dire si l'IA a aidé, nui, ou n'a rien fait. Vous conduisez à l'aveugle, et vous continuerez à dépenser de l'argent pour quelque chose que vous ne pouvez pas évaluer.

**Pourquoi ça arrive.** Mesurer semble être du travail en plus, et cela peut montrer de mauvaises nouvelles. Il est plus facile de supposer que ça marche que de vérifier. Beaucoup de projets se lancent dans l'enthousiasme et ne regardent plus jamais un chiffre.

**Ce que ça coûte.** Vous ne pouvez pas prouver la valeur, alors vous ne pouvez pas prendre de bonnes décisions pour étendre ou arrêter. Vous continuez à dépenser pour des choses qui peuvent ne pas marcher. Vous perdez la leçon qui rendrait le projet suivant meilleur. Un projet que vous n'avez jamais mesuré est un projet dont le résultat était aléatoire.

**La solution : mesurer dès le départ.** Fixez une référence avant de lancer, suivez quelques indicateurs honnêtes, et passez-les en revue régulièrement. La méthode complète est dans le [Chapitre 16 — Objectifs, coûts et retour sur investissement](ch16-goals-costs-and-return-on-investment.md) et la pratique du tableau de bord est dans le [Chapitre 22 — Mesurer les résultats et le ROI](ch22-measuring-results-and-roi.md). Ne la réapprenez pas ici ; engagez-vous juste à la faire. Mesurez la vérité, y compris les mauvaises semaines, et servez-vous-en pour décider de garder, corriger ou arrêter.

**Mesurez ce qui compte, pas ce qui vous flatte.** Évitez les indicateurs de vanité comme les comptes d'usage. Mesurez le temps, les erreurs, le coût et la satisfaction. Un chiffre qui ne montre que le bon côté est un chiffre qui vous ment.

## Éthique et responsabilité

Chaque erreur de cette liste a un tranchant éthique, parce que chacune peut blesser de vraies personnes — clients, employés, ou l'entreprise elle-même.

**Faire trop confiance à l'IA est une faute éthique, pas seulement pratique.** Quand un résultat de l'IA non vérifié atteint un client et est faux, vous avez blessé quelqu'un. Vous restez responsable de ce que votre IA envoie, aussi assuré que cela ait pu sonner. Garder l'humain dans la boucle est un devoir, pas une préférence.

**Ignorer les règles est un devoir que vous devez aux gens, pas une case à cocher.** Les règles de confidentialité existent pour protéger les informations de vraies personnes. Les suivre, c'est respecter ces personnes, pas éviter une amende. L'amende est le moindre du problème ; le tort causé à la personne dont vous avez mal traité les données est le vrai enjeu.

**Ne pas mesurer est un manque d'honnêteté.** Si vous ne pouvez pas dire si votre IA fonctionne, vous ne pouvez pas honnêtement dire à vos clients, votre personnel ou vos partenaires ce que vous faites. La mesure fait partie du fait d'être véridique sur votre propre entreprise.

**Démarrer trop gros peut blesser vos propres gens.** Un projet big-bang raté gaspille l'argent de l'entreprise et la confiance et l'effort de l'équipe. Une ambition qui ignore le chemin sûr peut abîmer les très personnes que vous essayez d'aider. Protégez-les en avançant par étapes sûres.

**Le fil commun : restez éveillé et restez responsable.** Chaque erreur ici est une forme de somnambulisme — faire la chose facile au lieu de la chose prudente. La posture éthique est la posture éveillée : choisissez le processus délibérément, respectez les données et les gens, vérifiez le résultat, avancez par étapes sûres, suivez les règles, et mesurez la vérité.

## Erreurs à éviter

Ce chapitre *est* la liste des erreurs, alors au lieu de la répéter, voici la méta-erreur qui cache toutes les autres :

**La méta-erreur : traiter l'IA comme un produit que vous achetez au lieu d'un changement que vous gérez.** Les six erreurs viennent de la même racine — traiter l'IA comme un achat qui fonctionne tout seul, plutôt que comme un changement qui demande de choisir, préparer, superviser et mesurer. Quand vous achetez un outil et attendez qu'il livre par lui-même, vous glissez dans tous les pièges à la fois : mauvais processus, mauvaises données, confiance aveugle, trop gros, pas de règles, pas de mesure.

**La solution à la méta-erreur : traiter l'IA comme un changement géré.** Choisissez la cible exprés. Préparez les données et les gens. Supervisez le résultat. Commencez petit et montez avec un plan. Suivez les règles. Mesurez le résultat. C'est tout le livre en une phrase, et c'est l'opposé du somnambulisme qui cause chaque échec ici.

Une seconde méta-erreur qui vaut d'être nommée : **conclure « l'IA ne marche pas » à partir d'un projet raté.** Quand un projet échoue, la cause était presque toujours l'une des six erreurs, pas la technologie. Ne jetez pas l'opportunité parce que vous avez marché sur une mine. Apprenez laquelle c'était, évitez-la la prochaine fois, et réessayez avec discipline. Les outils marchent quand vous évitez les erreurs.

## Exercice pratique

### 24.8 Exercice : auditez votre plan face aux six erreurs

Prenez n'importe quel projet d'IA que vous planifiez ou menez, et auditez-le face aux six erreurs. Pour chacune, répondez honnêtement par oui ou non et une ligne de preuve.

**1. Mauvais processus ?** « Ai-je choisi cette cible par impact et adéquation, pas seulement par enthousiasme ? » Si non, revenez et utilisez le test impact-vers-facilité (Chapitre 12).

**2. Données et gens sous-estimés ?** « Mes données sont-elles assez propres, et ai-je budgété du vrai temps pour la formation et le changement ? » Si non, corrigez les données et planifiez le travail humain avant d'aller plus loin.

**3. Trop confiance à l'IA ?** « Y a-t-il une vérification humaine sur tout ce qui compte, et les gens savent-ils à quoi ressemble une mauvaise réponse ? » Si non, ajoutez la règle de vérification maintenant, avant que d'autres résultats ne sortent.

**4. Démarré trop gros ?** « Est-ce que je commence par une seule tâche étroite et une seule équipe, ou je pars large ? » Si large, réduisez à un pilote et prouvez la valeur d'abord.

**5. Règles et sécurité ignorés ?** « Sais-je quelles règles s'appliquent à moi, et les données sont-elles protégées ? » Si vous n'êtes pas sûr, renseignez-vous et corrigez avant de manipuler plus de données sensibles.

**6. Pas de mesure ?** « Ai-je une référence et quelques indicateurs honnêtes que je surveille vraiment ? » Si non, mettez-les en place maintenant, même si vous devez reconstruire la référence.

Pour chaque « non », écrivez une action concrète pour corriger, avec une date. N'avancez pas sur le projet tant que les réponses « non » ne sont pas corrigées. Cet audit de dix minutes attrape la plupart des erreurs coûteuses avant qu'elles ne vous coûtent. Gardez les réponses et revérifiez-les à votre date de revue.

## Liste de contrôle

### 24.9 Liste de contrôle anti-erreurs

Passez ceci sur n'importe quel projet d'IA avant et pendant.

- [ ] **Vous avez choisi la cible par impact et adéquation**, pas par enthousiasme ou habitude.
- [ ] **Vous avez réparé ou simplifié le processus avant de l'automatiser.**
- [ ] **Vous avez vérifié la qualité des données** et corrigé les données avant d'attendre de bons résultats.
- [ ] **Vous avez budgété du vrai temps et de l'argent pour le côté humain** — formation, communication, changement.
- [ ] **Vous gardez une vérification humaine sur tout ce qui compte** — l'IA rédige, un humain envoie.
- [ ] **Vous avez formé les gens à repérer les mauvais résultats**, pas seulement à appuyer sur des boutons.
- [ ] **Vous traitez les résultats assurés et fluides avec méfiance** et vous vérifiez ce qui compte.
- [ ] **Vous avez fixé des règles d'escalade** — la routine à l'IA, l'important et l'étrange à un humain.
- [ ] **Vous avez commencé petit** — une seule tâche étroite, une seule équipe, un seul objectif clair.
- [ ] **Vous montez par étapes** avec un plan, pas un seul déploiement big-bang.
- [ ] **Vous savez quelles réglementations s'appliquent à vous** (RGPD, AI Act) et vous les suivez.
- [ ] **Vous protégez les données sensibles** avec une vraie sécurité dès le premier jour, pas greffée plus tard.
- [ ] **Vous traitez la conformité comme continue**, pas un contrôle ponctuel.
- [ ] **Vous avez mesuré une référence** avant le lancement.
- [ ] **Vous suivez des indicateurs honnêtes** (temps, erreurs, coût, satisfaction), pas des indicateurs de vanité.
- [ ] **Vous passez les chiffres en revue régulièrement** et vous en servez pour décider garder / corriger / arrêter.
- [ ] **Vous traitez l'IA comme un changement géré**, pas un produit qui livre tout seul.
- [ ] **Vous n'avez pas conclu « l'IA ne marche pas »** à partir d'une erreur qu'il vous incombait d'éviter.

Si une case est vide, vous êtes debout sur une mine. Contournez-la avant de dépenser plus d'argent ou de confiance. Chaque erreur de cette liste est vieille, courante et évitable — une fois que vous savez qu'elle est là.

## Points à retenir

- La plupart des échecs de l'IA viennent de six erreurs vieilles et prévisibles — mauvais processus, données et gens faibles, trop de confiance, trop gros, règles et sécurité ignorées, pas de mesure — et toutes sont évitables une fois qu'on les connaît.
- L'erreur la plus dangereuse est de faire trop confiance aux résultats fluides de l'IA ; gardez une vérification humaine sur tout ce qui compte, parce que la fluidité n'est pas la vérité.
- La racine de chaque erreur est de traiter l'IA comme un produit que vous achetez au lieu d'un changement que vous gérez — choisir, préparer, superviser, monter par étapes, suivre les règles, et mesurer.
- Commencez petit et prouvez la valeur avant de partir large ; une victoire étroite que vous pouvez contrôler bat un grand déploiement que vous ne pouvez pas.
- Ne concluez pas « l'IA ne marche pas » à partir d'un projet raté — nommez quelle erreur l'a causée, corrigez-la, et réessayez avec discipline.
