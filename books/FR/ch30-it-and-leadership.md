# Chapitre 30 — Informatique et direction

## En mots simples

L'informatique et la direction sont deux moitiés d'un seul métier : garder l'entreprise qui tourne et la piloter dans la bonne direction. L'informatique garde les systèmes, les données et le réseau fonctionnels et sûrs. La direction transforme tout cela en décisions — où investir, quoi réparer en premier, quel risque prendre. L'IA aide les deux moitiés. Elle répond aux questions informatiques de routine, surveille les menaces, construit les rapports et expose les options pour qu'un dirigeant puisse bien choisir.

Pensez à l'informatique comme la plomberie et la sécurité d'un bâtiment, et à la direction comme les gens qui décident où le bâtiment va ensuite. Quand la plomberie fuit, tout le monde le sent. Quand la barrière de sécurité est laissée ouverte, tout le monde est exposé. Et quand les dirigeants doivent décider sans image claire, ils devinent. L'IA répare les fuites plus vite, surveille les barrières, et donne aux dirigeants une image claire pour décider.

Ce chapitre couvre quatre métiers : le support interne (aider le personnel avec sa technologie), la cybersécurité (défendre contre l'attaque), les rapports de gestion (transformer les données en une image claire), et l'aide à la décision (exposer les options pour un dirigeant). Chacun est un endroit où une petite entreprise peut tourner plus smoothly, rester plus sûre, et mieux décider.

Une idée honnête d'abord : l'IA en informatique et direction est un *copilote*, pas le *capitaine*. Elle répond, surveille, résume et suggère. Une personne prend encore la décision — que ce soit arrêter un système, à quel fournisseur se fier, quel risque accepter. Plus la décision est grosse, plus le jugement humain compte. La méthode pour juger si tout cela rapporte vit au [Chapitre 16 — Objectifs, coûts et retour sur investissement](ch16-goals-costs-and-return-on-investment.md) ; ce chapitre vous montre quoi automatiser et comment. Pour voir où l'informatique et la direction se situent sur la carte impact-effort de toute votre entreprise, regardez le [Chapitre 12 — Où l'IA peut aider votre entreprise](ch12-where-ai-can-help-your-business.md).

## Un peu d'histoire

**Années 1980-1990 : le help desk.** Le support informatique a commencé comme le help desk — un numéro de téléphone que le personnel appelait quand quelque chose cassait. Une personne journalisait le problème, réparait ce qu'elle pouvait, et escaladait le reste. Cela marchait, mais c'était lent, et les mêmes questions simples — mots de passe oubliés, ennuis d'imprimante — mangeaient la majeure partie de la journée.

**Années 1990-2000 : tableaux de bord et business intelligence.** Les entreprises ont commencé à rassembler les données dans des tableaux de bord et des outils de business intelligence — des logiciels qui transforment les nombres bruts en graphiques et résumés. Pour la première fois, un manager pouvait voir ventes, coûts et performance sur un seul écran. Mais construire ces rapports prenait encore un analyste, et vous ne pouviez voir que ce que le rapport était construit pour montrer.

**Années 2000 : surveillance de sécurité automatisée.** À mesure que les attaques croissaient, l'informatique a ajouté des outils de sécurité automatisés — pare-feu, détection d'intrusion et systèmes d'alerte qui surveillent le réseau pour une activité suspecte. Ceux-ci repéraient plus qu'un humain, mais produisaient aussi un déluge d'alertes, la plupart inoffensives, et un analyste fatigué devait trier la vraie menace du bruit.

**Années 2010 : l'apprentissage automatique lit la menace.** L'apprentissage automatique — un logiciel qui apprend des motifs à partir de nombreux exemples — a changé la sécurité. Au lieu de faire correspondre des signatures d'attaque connues, l'IA apprenait à quoi ressemblait le « normal » sur le réseau et signalait l'inhabituel. Elle perçait le bruit d'alertes en repérant les rares signaux qui comptaient vraiment.

**Années 2020 : les grands modèles de langage répondent et conseillent.** Les grands modèles de langage — une IA entraînée sur d'énormes quantités de texte — peuvent désormais répondre à la question informatique d'un employé en langage simple, résumer un incident de sécurité, construire un rapport de gestion à partir de données brutes, et exposer les options et les compromis pour la décision d'un dirigeant. C'est la plus récente étape : une IA qui lit, explique et conseille sur les quatre métiers à la fois. L'exemple de risque fournisseur IBM ci-dessous montre la même idée appliquée à décider quels fournisseurs sont sûrs.

L'arc : d'un help desk par téléphone, aux tableaux de bord, aux alertes automatisées, à une IA qui lit la menace et répond à la question, à une IA qui conseille la décision. Chaque étape a déplacé le travail de routine vers le logiciel et laissé les humains décider et diriger.

## Curiosité

### 30.5 Le plus vieux problème du dirigeant : décider sans image claire

Aussi longtemps qu'il y a eu des managers, il y a eu la même plainte : « Je dois décider, mais je ne vois pas clairement. » Les données sont éparpillées dans les systèmes. Le rapport prend une semaine à construire. Le tableau de bord montre le mois dernier, pas aujourd'hui. Alors les dirigeants décident à l'instinct et espèrent.

L'IA change cela plus que presque tout autre chose dans ce livre. Elle peut rassembler les données éparpillées, construire l'image à la demande, et répondre à la question d'un dirigeant en mots simples en quelques secondes — « Quelle gamme de produits perd de l'argent ? », « Où est notre trésorerie le mois prochain ? », « Quel fournisseur est le plus gros risque ? ». Le dirigeant décide encore. Mais maintenant il décide avec une image claire au lieu d'un pari. C'est la révolution silencieuse en direction : non pas l'IA qui prend la décision, mais l'IA qui rend la décision *éclairée*. L'histoire de risque fournisseur IBM ci-dessous est exactement cela, appliquée à une décision difficile — à quels fournisseurs pouvons-nous nous fier ?

## Un exemple d'entreprise réel

**IBM : évaluation assistée par IA du risque tiers (fournisseur).**

Toute entreprise qui achète à des fournisseurs externes porte un *risque tiers* — le risque qu'un fournisseur dont vous dépendez se révèle peu fiable, peu sûr ou non conforme. Vérifier chaque fournisseur est un travail lent et soigneux. Une façon courante de vérifier est un questionnaire détaillé que le fournisseur remplit, qu'un évaluateur humain lit puis note. Quand vous avez des centaines de fournisseurs, ce travail devient un goulot d'étranglement.

L'ingénierie client d'IBM a publié un vrai projet là-dessus, appelé « Évaluer le risque tiers avec l'IA ». Le client était une institution financière qui menait **plus de 1 000 évaluations de fournisseurs par an**, et chaque évaluation prenait **environ 45 heures de travail** à compléter — lire le questionnaire, vérifier les preuves, et noter le risque. C'est une énorme quantité de temps qualifié passé sur la même tâche soigneuse, encore et encore.

IBM a utilisé sa plateforme watsonx.ai pour assister les évaluateurs. L'IA lisait les réponses du questionnaire fournisseur et les preuves à l'appui, et aidait l'évaluateur à comprendre la qualité de ce que le fournisseur avait fourni, pour que l'humain puisse se concentrer sur le jugement au lieu de tout lire depuis zéro. L'estimation publiée était **environ 20 % de réduction du temps d'évaluation**, ce qui sur cette charge de travail représentait **environ 10 000 heures de travail économisées** et **environ 800 000 $ de coût de main-d'œuvre par an**.

Une note sur le chiffre des « 50 % ». Vous pouvez voir ce genre de travail IBM sur le risque fournisseur cité comme « environ 50 % de réduction du temps ». Ce nombre n'est **pas** ce que le cas publié d'IBM rapporte. L'estimation publiée pour ce projet est d'environ 20 %, avec les économies exprimées comme ~10 000 heures et ~800 000 $ par an. Traitez les « 50 % » comme non vérifiés, et utilisez les chiffres publiés — ~20 % de réduction de temps, ~10 000 heures, ~800 000 $ — comme les vrais chiffres sourcés. (Source : IBM Client Engineering, « Evaluating Third Party Risk with AI ».)

Deux choses valent d'être remarquées. D'abord, l'évaluateur humain est resté aux commandes. L'IA n'a pas approuvé ni rejeté un fournisseur ; elle a aidé l'humain à lire plus vite et mieux juger. Ensuite, l'économie est venue de la partie *lecture et vérification* du travail — la lecture lente et soigneuse que l'IA fait bien — tandis que la *décision* sur le fournisseur est restée à la personne. C'est le schéma à copier dans vos propres travaux de risque : laissez l'IA faire la lecture, gardez l'humain pour le jugement.

## Comment faire

### 30.1 Support interne

Le support interne signifie aider votre propre personnel avec sa technologie — le mot de passe oublié, l'imprimante qui ne marche pas, le logiciel qui faut configurer. C'est le help desk, et il est plein des mêmes questions répétées. L'IA est très douée avec les questions répétées.

**L'assistant du help desk informatique.** Un chatbot entraîné sur votre propre base de connaissances informatique peut répondre aux questions du personnel instantanément : « Comment me connecter au VPN ? », « Comment réinitialiser mon mot de passe ? », « Comment installer cette application ? ». Cela enlève les tickets de routine qui mangent la journée d'une équipe de support, pour que l'équipe puisse se concentrer sur les vrais problèmes.

**Résolvez les simples automatiquement.** Certains tickets demandent une action simple — réinitialiser un mot de passe, déverrouiller un compte, réinstaller une application. L'IA peut faire cela automatiquement ou rédiger l'action pour qu'un humain l'approuve. Le travail de routine disparaît de la file.

**Acheminez les difficiles vite.** Quand le bot ne peut pas résoudre, il doit passer le ticket à la bonne personne avec le contexte intact — ce que l'employé a déjà dit et essayé — pour que l'humain ne reparte pas de zéro. Un passage de relais propre est la fonctionnalité la plus importante.

**Construisez à partir de vos propres tickets.** Tirez les derniers mois de tickets informatiques et trouvez les questions les plus courantes. Celles-ci deviennent la base de connaissances du bot. La même technologie de chatbot, appliquée aux clients plutôt qu'au personnel, est couverte au [Chapitre 27 — Service et support client](ch27-customer-care-and-support.md) ; ici elle est retournée vers l'intérieur pour servir votre propre équipe.

**Gardez un humain pour le problème difficile.** L'IA gère la routine ; une personne gère la panne, le bug étrange, l'incident de sécurité. Ne laissez jamais un bot être le seul chemin quand quelque chose est vraiment cassé. Le personnel doit toujours pouvoir joindre un humain.

### 30.2 Cybersécurité

La cybersécurité signifie défendre vos systèmes, vos données et votre réseau contre l'attaque. L'IA est désormais un outil central des deux côtés de ce combat — les défenseurs l'utilisent pour repérer les menaces, et les attaquants aussi — donc il compte que vous compreniez ce qu'elle peut et ne peut pas faire pour vous.

**L'IA repère l'inhabituel.** L'IA apprend à quoi ressemble le « normal » sur votre réseau — trafic normal, connexions normales, accès aux données normal — et signale ce qui cloche. Une connexion d'un pays étrange à 3 h du matin, un déluge soudain de téléchargements de fichiers, un appareil au comportement étrange. Ces petits signaux, vus d'un coup sur tout le réseau, sont ainsi que l'IA repère une menace qu'un humain manquerait.

**Percez le bruit d'alertes.** Les outils de sécurité produisent des milliers d'alertes, la plupart inoffensives. L'IA les classe pour que la vraie menace remonte en haut et le bruit retombe. C'est l'un de ses plus grands apports : pas plus d'alertes, mais *moins d'alertes, meilleures*, qu'une petite équipe peut réellement gérer.

**Répondez plus vite.** Quand l'IA signale une vraie menace, elle peut aussi suggérer ou prendre une première action rapide — isoler une machine infectée, bloquer une adresse suspecte — pour stopper la propagation pendant qu'un humain enquête. La vitesse compte dans une attaque ; les premières minutes décident de combien de dégâts sont faits.

**Le tableau complet de la sécurité est son propre sujet.** Les menaces, les défenses et les habitudes humaines qui comptent le plus sont couverts en profondeur au [Chapitre 6 — Cybersécurité à l'ère de l'IA](ch06-cybersecurity-in-the-ai-era.md), et le déploiement sécurisé au [Chapitre 20 — Déployer l'IA en sécurité](ch20-implementing-ai-securely.md). Lisez-les avant de vous reposer sur l'IA pour votre défense. L'IA est un outil puissant, pas un bouclier magique.

**Gardez un humain pour la grande décision.** L'IA peut isoler une machine, mais une personne décide s'il faut arrêter un système, payer ou refuser une rançon, appeler les autorités. Dans un vrai incident, le jugement humain est la dernière ligne de défense. Ne laissez jamais l'automatisation prendre seule les grandes décisions de sécurité.

### 30.3 Rapports de gestion

Un rapport de gestion transforme les données brutes en une image claire qu'un dirigeant peut lire et sur laquelle agir — compte de résultat, ventes par produit, coûts par catégorie, position de trésorerie. L'IA change qui construit le rapport et à quelle vitesse.

**Le rapport se construit tout seul.** Au lieu qu'un analyste tire des nombres dans un tableur chaque semaine, le rapport peut se générer selon un calendrier depuis vos systèmes en direct et atterrir dans la boîte du dirigeant. Les nombres sont toujours à jour, et personne n'a à se souvenir de le faire.

**Résumés en langage simple.** L'IA peut lire les nombres et écrire un court résumé en mots simples : « Le chiffre d'affaires a monté de 8 % ce mois-ci, porté par le produit X ; les coûts ont monté de 3 %, surtout en livraison. » Cela transforme une table de chiffres en une phrase qu'un dirigeant peut réellement lire et sur laquelle agir. C'est comme avoir un jeune analyste qui écrit le commentaire.

**Demandez en langage simple.** Certains outils laissent un dirigeant demander « Quelle gamme de produits a perdu de l'argent le trimestre dernier ? » et obtenir une réponse sans écrire de formule. C'est utile pour les questions ponctuelles qui voulaient dire « je regarderai ça plus tard » et ne se faisaient jamais. Le dirigeant obtient la réponse pendant que la question est encore fraîche.

**Ne sautez pas la lecture humaine.** Un rapport automatique est un point de départ, pas un document de décision fini. Lisez le résumé, vérifiez que les nombres ont du sens, et ajoutez votre propre jugement avant d'agir ou de partager. L'IA peut résumer avec assurance et avoir quand même tort si les données sous-jacentes sont désordonnées. Poubelle dedans, poubelle confiante dehors.

**Gardez le format stable.** Une fois que vous vous fixez sur une mise en page de rapport, gardez-la cohérente. Un format stable est plus facile à lire de mois en mois et plus facile pour repérer quand quelque chose cloche. Changez-le délibérément, pas à chaque fois. (Les mêmes idées de construction de rapport, appliquées à la finance, sont au [Chapitre 25 — Administration et Finance](ch25-administration-and-finance.md).)

### 30.4 Aide à la décision

L'aide à la décision signifie utiliser l'IA pour exposer les options, les preuves et les compromis d'une décision, pour qu'un dirigeant puisse bien choisir. Elle ne prend pas la décision. Elle rend la décision *éclairée*.

**Exposez les options.** Pour un choix comme « Devrions-nous ouvrir une nouvelle région ? » ou « Quel fournisseur devrions-nous choisir ? », l'IA peut rassembler les données pertinentes et présenter les options côte à côte, avec les avantages, les inconvénients et les chiffres derrière chacune. Le dirigeant voit le tableau entier, pas le favori d'une personne.

**Modélisez les compromis.** L'IA peut montrer ce qui se passe sous différentes hypothèses : « Si la demande monte de 10 %, cette option gagne ; si elle reste plate, celle-là est plus sûre. » Cela transforme un pari en une comparaison de scénarios, bien plus utile pour une grosse décision.

**Faites surface ce que vous avez manqué.** L'IA peut signaler un risque ou une occasion qu'un dirigeant occupé n'a pas vus, parce qu'elle a tout regardé à la fois. Le cas de risque fournisseur IBM ci-dessus est exactement cela : l'IA lisant les réponses de chaque fournisseur pour que l'évaluateur voie le risque clairement avant de décider.

**Gardez la décision au dirigeant.** L'IA conseille ; le dirigeant décide et assume le résultat. Un dirigeant qui suit le modèle aveuglément a cessé de diriger. Utilisez l'IA pour éclairer votre jugement, pas pour le remplacer. La stratégie derrière ces choix est au [Chapitre 13 — Définir une simple stratégie d'IA](ch13-defining-a-simple-ai-strategy.md).

**Méfiez-vous du non-sens confiant.** L'IA peut présenter une mauvaise option avec une totale assurance. Vérifiez les preuves derrière son conseil, surtout pour une décision grosse ou inhabituelle. Demandez au modèle de montrer son raisonnement, et testez-le contre ce que vous savez. Faites confiance, mais vérifiez.

## Éthique et responsabilité

L'informatique et la direction portent la confiance de toute l'entreprise, donc la responsabilité ici est large.

**Gardez l'humain dans la grande décision.** L'IA conseille sur la sécurité, les rapports et la stratégie. Une personne prend la décision d'arrêter un système, de faire confiance à un fournisseur, ou de prendre un risque. Plus la décision est grosse, plus l'humain l'assume.

**Protégez les données que vous donnez aux modèles.** Les données d'informatique et de direction — journaux réseau, données financières, dossiers fournisseurs — comptent parmi les plus sensibles qu'une entreprise détient. Gardez-les sécurisées et, là où c'est important, dans votre propre environnement. Ne donnez pas de données sensibles à des outils d'IA publics sans vérifier les implications de sécurité (voir [Chapitre 6](ch06-cybersecurity-in-the-ai-era.md) et [Chapitre 8 — Auto-hébergement : gardez vos données sous contrôle](ch08-self-hosting-keep-your-data-under-control.md)).

**Surveillez l'IA tierce et fantôme.** Les fournisseurs et le personnel peuvent amener des outils d'IA dans l'entreprise sans approbation — le risque d'« IA fantôme ». Sachez quelle IA tourne sur votre réseau et qui l'a approuvée. Ce risque est couvert au [Chapitre 9 — Services tiers et IA fantôme](ch09-third-party-services-and-shadow-ai.md).

**Soyez honnête dans les rapports et les conseils.** Un résumé IA peut faire sembler correct un mauvais trimestre, et un conseil IA peut être confiant et faux. Lisez les nombres, vérifiez le conseil, et rapportez la vérité, surtout quand elle est inconfortable. Le travail d'un dirigeant est de voir clairement, pas d'être réconforté.

**Gardez à l'esprit le plancher légal.** Certains usages de l'IA en informatique et RH touchent les règles de haut risque et de transparence de l'AI Act. Connaissez votre rôle et vos devoirs avant de déployer (voir [Chapitre 5 — Règles et responsabilité légale](ch05-rules-and-legal-responsibility.md)). La conformité est le plancher ; votre propre jugement fixe la norme au-dessus.

**Utilisez l'IA pour renforcer la confiance, pas pour contrôler les gens.** La surveillance et l'analytique devraient rendre l'entreprise plus sûre et mieux gérée, pas devenir un outil pour surveiller et faire pression sur le personnel. Utilisez-les pour protéger et améliorer, pas pour faire la police.

## Erreurs à éviter

**Un help desk tout-bot.** Du personnel avec un vrai problème bloqué derrière un bot sans chemin humain. Autorisez toujours un passage à un humain.

**Se fier aveuglément à une alerte de sécurité.** Agir sur un faux positif, ou pire, ignorer une vraie menace parce que l'alerte était enfouie. Réglez le système et gardez un enquêteur humain.

**Laisser l'automatisation prendre la grande décision de sécurité.** Arrêter, payer ou escalader sans un humain. Gardez la décision humaine dans un incident.

**Sauter la lecture humaine sur les rapports.** Agir sur un résumé IA sans vérifier les nombres. Lisez-le vous-même d'abord.

**Non-sens confiant dans les conseils.** Suivre un conseil IA qui est faux mais bien formulé. Vérifiez les preuves derrière.

**Foi aveugle dans le modèle pour les grosses décisions.** Un dirigeant qui cesse de diriger et suit juste le tableau de bord. Le dirigeant assume la décision.

**Donner des données sensibles à une IA publique.** Journaux réseau, données financières et dossiers fournisseurs dans des outils non sûrs. Vérifiez d'abord la sécurité et la vie privée.

**IA fantôme tournant sans contrôle.** Personnel et fournisseurs utilisant des outils d'IA non approuvés. Sachez ce qui tourne et qui l'a approuvé.

**Automatiser un processus cassé.** Si votre support informatique ou votre reporting est un désordre, l'IA fait un désordre plus rapide. Réparez d'abord le processus.

**Pas de référence.** Ne pas mesurer le temps de ticket, le taux d'incident ou le temps de rapport avant, donc vous ne pouvez pas prouver le gain. Mesurez d'abord (voir [Chapitre 22 — Mesurer les résultats et le ROI](ch22-measuring-results-and-roi.md)).

**Citer le chiffre du fournisseur comme le vôtre.** Utiliser le chiffre du meilleur cas d'un fournisseur au lieu de votre propre résultat mesuré. Utilisez vos propres chiffres.

## Exercice pratique

### 30.7 Exercice : planifiez une automatisation informatique ou de direction

Choisissez un métier et planifiez son assistance IA de bout en bout, avec la décision humaine intégrée.

**Étape 1 — Choisissez le métier.** Choisissez-en un : support interne, cybersécurité, rapports de gestion, ou aide à la décision. Faites-en un, pas tous.

**Étape 2 — Définissez l'objectif et la métrique.** Une résolution de tickets plus rapide ? Moins de menaces manquées ? Des rapports plus rapides ? De meilleures décisions ? Choisissez un nombre à mesurer.

**Étape 3 — Mesurez la référence.** Que vaut ce nombre maintenant ? Temps moyen de ticket, incidents manqués, jours pour construire un rapport, délai de décision. Écrivez-le.

**Étape 4 — Trouvez la cible coûteuse.** Identifiez le point le plus douloureux — le type de ticket qui mange le plus de temps, la menace qui passe au travers, le rapport toujours en retard, la décision que vous continuez à rater. Ciblez celui-là d'abord.

**Étape 5 — Marquez chaque étape.** Pour chaque étape, marquez-la : **l'IA la fait** (répondre, signaler, résumer, exposer les options), **l'humain la revoit** (vérifier l'alerte, lire le rapport), ou **l'humain la décide** (arrêter le système, choisir le fournisseur, prendre le risque). Chaque grande décision doit être humaine.

**Étape 6 — Vérifiez les données et la loi.** Décidez de quelles données l'IA a besoin, gardez-les sécurisées, et vérifiez si l'usage touche les règles de haut risque ou de transparence de l'AI Act (voir [Chapitre 5](ch05-rules-and-legal-responsibility.md)).

**Étape 7 — Connectez les systèmes.** Décidez quels systèmes l'IA doit voir — tickets, journaux, données financières, dossiers fournisseurs — et comment vous les connecterez (voir [Chapitre 19 — Connecter l'IA aux systèmes que vous utilisez déjà](ch19-connecting-ai-to-systems-you-already-use.md)).

**Étape 8 — Lancez petit et mesurez.** Faites-le sur une équipe, un système ou un rapport d'abord. Comparez la métrique à la référence. Ne passez à l'échelle que ce qui prouve que ça marche.

Faites un métier bien. L'analyse de la cible coûteuse à l'étape 4 est précieuse à elle seule — elle vous montre où votre travail d'informatique et de direction perd réellement le plus de temps ou porte le plus de risque, ce qui est utile même avant d'acheter un outil.

## Liste de contrôle

### 30.8 Liste de contrôle informatique et direction

Avant d'automatiser une tâche informatique ou de direction, vérifiez ceci.

- [ ] **Vous avez mesuré la référence** — temps de ticket, taux d'incident, temps de rapport, délai de décision.
- [ ] **Vous avez ciblé le point le plus coûteux d'abord**, pas le plus facile.
- [ ] **Un humain prend chaque grande décision** — arrêt de système, confiance fournisseur, acceptation de risque.
- [ ] **Le bot du help desk passe à un humain** avec le contexte complet.
- [ ] **Les alertes de sécurité sont réglées** pour que la vraie menace remonte et le bruit retombe.
- [ ] **Un humain enquête sur chaque vrai incident de sécurité.**
- [ ] **Les rapports de gestion sont lus par un humain** avant que vous agissiez ou les partagiez.
- [ ] **Vous vérifiez les preuves derrière le conseil IA**, surtout pour les grosses décisions.
- [ ] **Les données sensibles sont gardées sécurisées**, pas envoyées à des services d'IA publics.
- [ ] **Vous savez quelle IA tourne sur votre réseau** et qui l'a approuvée (pas d'IA fantôme).
- [ ] **Vous avez vérifié l'AI Act** pour d'éventuels devoirs de haut risque ou de transparence.
- [ ] **Vous réparez le processus cassé avant de l'automatiser.**
- [ ] **Vous rapportez vos propres chiffres mesurés**, pas le meilleur cas du fournisseur.

Si une case est vide, le risque — pour vos systèmes, vos données ou vos décisions — est encore à vous. Remplissez-la avant de laisser l'IA près des commandes.

## Points à retenir

- L'IA en informatique et direction est un copilote : elle répond aux questions de support, repère les menaces, construit des rapports et expose des options, tandis qu'un humain garde chaque grande décision.
- Le cas de risque fournisseur IBM (IBM Client Engineering, « Evaluating Third Party Risk with AI ») a aidé une institution financière avec plus de 1 000 évaluations par an à ~45 heures chacune, avec une estimation publiée d'environ 20 % de réduction de temps, ~10 000 heures et ~800 000 $ économisés par an — le chiffre des « environ 50 % » n'est pas ce que la source publiée rapporte.
- L'économie vient du fait de laisser l'IA faire la lecture et la vérification lentes tandis que l'humain garde le jugement ; le même schéma marche sur le support, la sécurité, les rapports et les décisions.
- Gardez les données sensibles sécurisées, sachez quelle IA tourne sur votre réseau, et vérifiez les règles de haut risque et de transparence de l'AI Act avant de déployer.
- Mesurez votre propre référence, gardez un humain dans chaque grande décision, et traitez la loi comme le plancher et votre propre jugement comme la norme au-dessus.

<!-- BEGIN agentbridge-examples -->

## Essayez avec AgentBridge

Voici à quoi ressemble le même travail avec AgentBridge. Chaque encadré montre le résultat fini et la seule ligne que vous tapez pour l'obtenir.

### Des notes de réunion propres

![Un compte rendu de réunion soigné avec décisions et actions](../../assets/examples/meeting-minutes.png)
*Un compte rendu de réunion soigné avec décisions et actions*

**Ce que vous demandez :** `Transforme ces notes brutes en un compte rendu de réunion propre avec une liste de décisions et des points d'action : [coller les notes]`

L'agent transforme vos notes désordonnées en un compte rendu structuré : ce qui a été discuté, ce qui a été décidé, et une liste d'actions avec des responsables. Vous pouvez les envoyer directement à l'équipe.

*Conseil : Collez vos notes telles quelles — l'agent remet de l'ordre dans la succession et le libellé.*

---

### Une revue trimestrielle du conseil

![Une diapositive de revue trimestrielle](../../assets/examples/board-review.png)
*Une diapositive de revue trimestrielle*

**Ce que vous demandez :** `Construis une présentation de revue trimestrielle : résultats, points forts, défis, et plan pour le trimestre prochain.`

L'agent assemble la présentation de revue avec les résultats, les victoires, les problèmes et le plan — disposés pour que la réunion avance vite.

*Conseil : Joignez votre feuille d'indicateurs et l'agent met les graphiques dans les diapositives.*

---

### Voyez tous vos agents d'un coup d'œil

![La vue OfficeManager de vos agents](../../assets/examples/officemanager-view.png)
*La vue OfficeManager de vos agents*

**Ce que vous demandez :** `(browser) Ouvre la vue OfficeManager.`

OfficeManager montre vos agents sur une seule page simple, pour que vous voyiez ce qui tourne et où en sont les choses.

*Conseil : Un moyen rapide de garder un œil sur plus d'un assistant à la fois.*

---

### Un briefing que vous pouvez écouter

![Un briefing audio prêt à être joué](../../assets/examples/audio-briefing.png)
*Un briefing audio prêt à être joué*

**Ce que vous demandez :** `Transforme le résumé de cette semaine en un court briefing audio que je peux écouter sur le chemin du travail.`

L'agent convertit le résumé écrit en un briefing audio clair, pour que votre trajet devienne du temps utile.

*Conseil : Planifiez le résumé hebdomadaire et sa version audio ensemble.*

<!-- END agentbridge-examples -->
