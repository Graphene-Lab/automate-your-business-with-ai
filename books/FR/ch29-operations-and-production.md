# Chapitre 29 — Opérations et production

## En mots simples

Les opérations sont le moteur d'une entreprise. C'est tout ce qui transforme des entrées en sorties : fabriquer un produit, le déplacer, faire tourner les machines, vérifier la qualité et garder les gens en sécurité. La production est la partie des opérations qui fabrique réellement la chose. Quand le moteur tourne bien, les clients reçoivent ce qu'ils ont commandé, à l'heure, sans défaut. Quand il tousse, tout ce qui vient après le ressent.

Pensez à vos opérations comme à un atelier, que vous fabriquiez des objets ou rendiez des services. Les machines tournent, les marchandises circulent, les gens travaillent, et quelque chose peut toujours légèrement déraper — une machine sur le point de lâcher, un lot avec un défaut, une livraison qui sera en retard, un travailleur à un endroit dangereux. Un bon opérateur voit ces choses tôt. L'IA aide en surveillant tout à la fois et en signalant les petits signaux qu'un œil humain fatigué rate.

Ce chapitre couvre quatre métiers : la maintenance prédictive (réparer les machines avant qu'elles ne cassent), le contrôle qualité (repérer les défauts automatiquement), la logistique (déplacer les marchandises et les informations efficacement) et la sécurité au travail (garder les gens hors de danger). Chacun est un endroit où une petite entreprise peut réduire le gaspillage, améliorer la qualité et protéger son personnel.

Une idée honnête d'abord : l'IA dans les opérations est une *sentinelle et une aide*, pas un pilote automatique qui gère l'atelier tout seul. Elle perçoit, prédit et suggère. Une personne décide encore quand arrêter une ligne, quand rejeter un lot, et quand renvoyer quelqu'un chez lui parce que ce n'est pas sûr. La méthode pour juger si tout cela rapporte se trouve dans le [Chapitre 16 — Objectifs, coûts et retour sur investissement](ch16-goals-costs-and-return-on-investment.md) ; ce chapitre vous montre quoi automatiser et comment. Pour voir où se situent les opérations sur la carte impact-effort de toute votre entreprise, regardez le [Chapitre 12 — Où l'IA peut aider votre entreprise](ch12-where-ai-can-help-your-business.md).

## Un peu d'histoire

**Années 1900-1950 : la chaîne de montage et la maintenance préventive.** La production moderne a commencé avec la chaîne de montage mobile, qui découpait le travail en petites étapes répétibles. Avec elle est venue la maintenance *préventive* — l'habitude de réviser une machine selon un calendrier fixe, comme changer l'huile d'une voiture tous les quelques milliers de kilomètres, qu'elle en ait besoin ou non. Cela réduisait les pannes, mais gaspillait de la révision sur des machines qui allaient bien.

**Années 1960-1980 : l'automatisation et le contrôle qualité.** Les usines ont ajouté des machines automatisées et un contrôle qualité formalisé — inspecter les produits par rapport à une norme et trier le bon du mauvais. Les méthodes statistiques de qualité repéraient les défauts dans les lots. Cela a élevé la qualité, mais reposait encore sur des humains pour inspecter et sur des règles fixes pour réviser les machines.

**Années 1990 : les capteurs et la chaîne d'approvisionnement numérique.** Des capteurs bon marché ont permis aux machines de signaler leur propre état — température, vibration, heures de fonctionnement. Les chaînes d'approvisionnement sont devenues numériques, avec des logiciels suivant les marchandises du fournisseur au client. Pour la première fois, un opérateur pouvait voir, sur un écran, ce qui se passait dans tout l'atelier et dans toute la chaîne d'approvisionnement. Mais les données étaient surtout lues à la main.

**Années 2000 : l'apprentissage automatique prédit la panne.** L'apprentissage automatique — un logiciel qui apprend des modèles à partir de nombreux exemples — a changé la maintenance. Au lieu de réviser selon un calendrier fixe, on pouvait apprendre à partir des données des capteurs quand une machine était *réellement* sur le point de lâcher. Un motif de vibration en hausse lente qu'un humain ne pouvait pas sentir devenait un signal d'alarme clair plusieurs jours à l'avance. C'est la naissance de la maintenance *prédictive*.

**Années 2010 : la vision par ordinateur inspecte la qualité.** La vision par ordinateur — une IA qui lit ce qu'une caméra voit — a commencé à inspecter les produits automatiquement. Une caméra pouvait repérer une fissure, une rayure ou une pièce manquante plus vite et plus régulièrement qu'un inspecteur humain, et sans se fatiguer. Le contrôle qualité est passé de l'échantillonnage à la vérification de chaque unité.

**Années 2020 : les agents exécutent le flux de travail.** Les grands modèles de langage et les agents IA — un logiciel qui prend une tâche entière et la mène à travers plusieurs étapes — exécutent maintenant des parties du flux de travail opérationnel lui-même : lire une demande, tirer des données des systèmes de back-end et exécuter l'étape suivante. L'exemple SOK Finance ci-dessous est exactement cela : des agents IA gérant les opérations de service quotidiennes d'un centre de services financiers, avec des humains supervisant.

L'arc : des calendriers fixes, à l'inspection manuelle, aux données des capteurs, à une IA qui prédit et voit, à des agents qui agissent. Chaque étape a déplacé la surveillance et le travail de routine vers le logiciel et a laissé aux humains la décision et l'intervention.

## Curiosité

### 29.5 Le centre de services qui a mis des agents IA en première ligne

Quand on entend « opérations et production », on imagine une usine. Mais les opérations, c'est aussi le centre de services qui garde une entreprise en marche — l'endroit où les demandes arrivent et où quelqu'un doit agir vite.

SOK Finance, en Finlande, gère un centre de services appelé Palveluässä qui fournit des services de gestion financière et de paie au S Group — un réseau finlandais de commerces et de sociétés de services détenu par ses clients, avec environ 2 000 points de vente. Chaque jour, des demandes arrivent : « Envoyez-moi une copie de cette facture », « Changez la date d'échéance de ce paiement ». De routine, en gros volume, et sensibles au temps.

La curiosité, c'est ce que l'entreprise en a fait. Au lieu d'embaucher plus de gens pour répondre aux mêmes demandes, ils ont mis des *agents* IA en première ligne pour traiter ceux de routine, afin que le personnel humain puisse se concentrer sur les cas qui demandent du jugement. Ce changement — passer de humains faisant chaque demande à des agents faisant la routine et des humains supervisant — est la même révolution silencieuse qui s'est produite dans l'atelier, appliquée cette fois à un centre de services. L'histoire complète, avec la vraie source, est ci-dessous.

## Un exemple réel d'entreprise

**SOK Finance : des agents IA exécutant le flux de travail du centre de services.**

SOK Finance exploite le centre de services Palveluässä, qui fournit des services de gestion financière et de paie au S Group, un réseau finlandais de commerces et de sociétés de services détenu par ses clients, avec environ 2 000 points de vente. Le centre de services traite un flux régulier de demandes de routine provenant de tout ce réseau — des choses comme demander une copie d'une facture ou changer une date d'échéance de paiement. Chaque demande est petite, mais ensemble elles forment une charge de travail large et répétitive qui doit être traitée vite et de façon cohérente.

D'après un communiqué de presse de CGI (Helsinki, 23 avril 2026), CGI a conçu, mis en œuvre et déployé une **solution IA multi-agents construite sur AWS Bedrock** pour SOK Finance, faisant entrer l'IA dans un usage de production en direct dans l'administration financière et le service client. Une solution « multi-agents » signifie que plusieurs agents IA travaillent ensemble sur une tâche, chacun traitant une étape. Dans ce cas, les agents traitent les messages entrants du service client, récupèrent les données nécessaires dans les systèmes de back-end, et exécutent automatiquement des parties du processus.

Le communiqué décrit la solution comme accélérant de façon significative les processus de routine tels que **les demandes de copie de facture et les changements de date d'échéance**, et comme améliorant l'efficacité et la cohérence par rapport au traitement manuel précédent. CGI était responsable de la conception, de la mise en œuvre, du déploiement et de l'intégration avec les systèmes clés de SOK Finance.

Deux choses méritent d'être remarquées. D'abord, le rôle humain passe de *faire chaque demande* à *superviser les agents et traiter les exceptions*. Les agents prennent la routine ; les gens prennent l'inhabituel et le sensible. Ensuite, la victoire est la cohérence autant que la vitesse — un agent suit les mêmes étapes soigneuses à chaque fois, là où une personne fatiguée un après-midi chargé pourrait glisser.

Une note sur la source et les chiffres : les chiffres ci-dessus viennent de l'annonce publiée par CGI. Le communiqué décrit les résultats en termes qualitatifs — des processus plus rapides, une meilleure cohérence — et ne publie pas de pourcentage précis pour le temps économisé ou le coût réduit. Considérez le résultat comme l'expérience rapportée par l'entreprise, et rappelez-vous que vos propres chiffres dépendront de votre volume et de vos systèmes. L'intérêt du cas est le *motif* : des agents IA exécutant un flux de travail de service de routine en production, avec des humains supervisant, à l'échelle d'un réseau de 2 000 points de vente.

## Comment faire

### 29.1 Maintenance prédictive

La maintenance prédictive signifie réparer une machine *avant* qu'elle ne casse, en prédisant la panne à partir de données au lieu d'attendre qu'elle arrive ou de réviser selon un calendrier fixe.

**L'ancienne méthode et son coût.** Traditionnellement, vous aviez deux choix : faire tourner une machine jusqu'à ce qu'elle lâche (et payer un arrêt imprévu), ou la réviser selon un calendrier fixe (et gaspiller de l'argent à réviser des machines qui allaient bien). Les deux perdent. Une panne imprévue arrête la production au pire moment et coûte bien plus qu'une réparation planifiée.

**Comment l'IA prédit.** Vous mettez des capteurs sur la machine pour mesurer des choses comme la vibration, la température, le son et les heures de fonctionnement. L'IA apprend le motif normal et repère les premiers signes de problème — une vibration qui monte lentement, une température qui tourne un peu chaude. Ces petits changements apparaissent souvent plusieurs jours avant une panne. L'IA vous avertit à temps pour réparer la machine pendant un arrêt planifié, pas en pleine production.

**Ce que cela économise.** La grande économie est d'éviter les temps d'arrêt imprévus — la panne surprise qui bloque tout. Une réparation planifiée un mardi après-midi est bon marché ; une panne pendant votre plus grosse commande du mois coûte cher. La maintenance prédictive transforme la seconde en première.

**Commencez petit.** Vous n'avez pas besoin de capteurs sur chaque machine. Commencez par la ou les deux machines dont la panne fait le plus mal — le goulot d'étranglement, celle avec le long temps de réparation, celle qui arrête toute la ligne. Mettez quelques capteurs dessus et observez. Prouvez la valeur là avant de vous étendre.

**L'humain décide l'arrêt.** L'IA signale le risque ; une personne décide quand faire descendre la machine. Ne laissez pas le système arrêter la production tout seul sans qu'un humain confirme la décision. L'avertissement est la valeur ; la décision reste humaine.

### 29.2 Contrôle qualité

Le contrôle qualité signifie vérifier qu'un produit respecte sa norme et repérer les défauts avant que le produit n'atteigne le client. L'IA change le contrôle qualité de *l'échantillonnage* à *la vérification de chaque unité*, et des *yeux fatigués* à des *yeux cohérents*.

**La vision par ordinateur inspecte.** Une caméra plus une IA peuvent regarder chaque produit sur la ligne et repérer une fissure, une rayure, une pièce manquante, une mauvaise étiquette ou une mauvaise couture. Elle vérifie chaque unité, pas seulement un échantillon, et elle ne se fatigue ni ne s'ennuie. Un inspecteur humain vérifiant des milliers d'unités par jour en ratera ; la caméra non.

**La cohérence est la victoire.** Les humains varient. Une personne est plus vive le matin, plus lente après le déjeuner, et facilement influencée par ce qu'elle a vu en dernier. L'IA applique la même norme à chaque unité, toute la journée. Cette cohérence vaut beaucoup dans une entreprise où un défaut atteignant un client coûte un retour, une réclamation ou une réputation.

**Repérez-le tôt.** Plus vous repérez un défaut tôt, moins il coûte. Un défaut repéré à la machine qui l'a fabriqué coûte une pièce. Le même défaut repéré à l'assemblage final coûte une retouche. Repéré par le client, il coûte un retour et de la confiance. L'IA à chaque poste repère les problèmes à la source, pas à la fin.

**Commencez par le défaut coûteux.** N'essayez pas de tout inspecter au début. Trouvez le défaut qui vous coûte le plus — celui qui cause le plus de retours ou de réclamations — et mettez une vérification par vision dessus. Prouvez qu'il repère le problème coûteux, puis ajoutez d'autres vérifications.

**Gardez un humain pour la décision délicate.** L'IA peut signaler une unité suspecte ; une personne décide si elle est vraiment défectueuse, surtout pour les cas limites. Ne laissez pas un système de vision jeter du bon produit parce qu'il est trop strict. Passez les rejets en revue et réglez le seuil.

### 29.3 Logistique

La logistique est le mouvement des marchandises et des informations : faire arriver la bonne chose au bon endroit au bon moment, au coût le plus bas. C'est un puzzle de routes, de stock, de minutage et de fournisseurs, et l'IA est très douée pour les puzzles de ce type.

**Optimisation des routes et des livraisons.** L'IA peut planifier des routes de livraison qui économisent des kilomètres, du carburant et du temps, en tenant compte du trafic, des créneaux de livraison et de la charge. Pour une entreprise avec une flotte, même une petite économie par route s'accumule vite sur une année.

**Stock et prévision de la demande.** L'IA regarde votre historique de ventes et prédit ce dont vous aurez besoin et quand, pour que vous stockiez assez sans suracheter. Trop peu de stock signifie une vente manquée ; trop signifie de la trésorerie immobilisée et du gaspillage. L'IA équilibre les deux en apprenant vos motifs et votre saisonnalité.

**Repérez le goulot d'étranglement.** L'IA peut voir où les marchandises ralentissent — un fournisseur toujours en retard, une étape d'entrepôt qui s'engorge, une route qui déborde toujours. Voir le goulot d'étranglement est la première étape pour le corriger. Toute la valeur est de rendre visible le retard invisible.

**Connectez les systèmes.** L'IA logistique fonctionne mieux quand elle peut voir vos commandes, votre stock et vos livraisons ensemble. Connecter l'IA aux systèmes que vous utilisez déjà — vos commandes, votre inventaire, votre suivi — est ce qui rend le tableau complet. Le mode d'emploi de cette connexion est dans le [Chapitre 19 — Connecter l'IA aux systèmes que vous utilisez déjà](ch19-connecting-ai-to-systems-you-already-use.md).

**Gardez un humain pour l'exception.** L'IA planifie la routine ; une personne gère la surprise — la grève, la tempête, le fournisseur qui flanche. Ne laissez pas un plan optimisé foncer dans une perturbation du monde réel sans un humain prêt à le court-circuiter. Le plan est un point de départ, pas une camisole.

### 29.4 Sécurité au travail

La sécurité au travail signifie garder les gens hors de danger. L'IA peut surveiller les conditions dangereuses et les comportements à risque et avertir avant qu'un accident n'arrive. C'est l'un des usages les plus précieux de l'IA, parce que ce qu'elle protège est une personne.

**La vision par ordinateur guette les dangers.** Des caméras plus une IA peuvent repérer un travailleur sans l'équipement de protection adéquat, une personne debout dans une zone dangereuse, une flaque par terre, ou une sortie de secours bloquée. Quand elle en voit un, elle déclenche une alerte pour que le danger soit corrigé avant que quelqu'un ne soit blessé.

**Prédisez le moment à risque.** L'IA peut apprendre quand les accidents sont les plus probables — une certaine équipe, une certaine machine, une certaine heure de la journée où les gens sont fatigués — et renforcer la surveillance à ce moment-là. C'est comme avoir un responsable sécurité qui ne cligne jamais des yeux et voit tout l'atelier à la fois.

**Une ligne juridique sérieuse : ne lisez pas les émotions.** Une IA qui déduit les *émotions* d'un travailleur depuis son visage ou sa voix est interdite sur le lieu de travail selon le règlement européen sur l'IA. La vision de sécurité porte sur les *dangers et l'équipement*, pas sur ce qu'un travailleur *ressent*. Gardez la caméra sur l'atelier et la machine, pas sur l'humeur de la personne. La liste complète des pratiques interdites est dans le [Chapitre 5 — Règles et responsabilité juridique](ch05-rules-and-legal-responsibility.md).

**Prévenez vos travailleurs.** Si vous utilisez une surveillance de sécurité basée sur l'IA qui affecte les travailleurs, vous devez informer vos travailleurs et leurs représentants avant de commencer, comme la loi l'exige pour l'IA à haut risque sur le lieu de travail. Soyez ouverts sur ce que les caméras surveillent et pourquoi. Le secret brise la confiance. La règle d'avis aux travailleurs est couverte dans la Curiosité de ce chapitre et dans le [Chapitre 5](ch05-rules-and-legal-responsibility.md).

**Utilisez-la pour protéger, pas pour punir.** Les données de sécurité doivent rendre le lieu de travail plus sûr — corriger le danger, changer le processus, former l'équipe. Elles ne doivent pas devenir un outil pour discipliner des individus pour chaque petite erreur. Utilisez-les pour trouver et supprimer le danger, pas pour monter un dossier contre un travailleur.

## Éthique et responsabilité

Les opérations touchent la sécurité et l'environnement, donc les enjeux éthiques sont réels et concrets.

**Les décisions de sécurité restent humaines.** L'IA peut avertir d'un danger, mais une personne décide quand arrêter une ligne ou renvoyer quelqu'un chez lui. Ne laissez jamais un système prendre une décision critique pour la sécurité sans humain dans la boucle. Un faux « tout va bien » peut blesser quelqu'un.

**Respectez la vie privée et les droits des travailleurs.** Les caméras et les capteurs sur le lieu de travail veillent sur des personnes. Utilisez-les pour la sécurité et les opérations, pas pour la surveillance. Dites aux travailleurs ce qui est surveillé et pourquoi, et suivez les règles de vie privée du [Chapitre 10 — Vie privée et RGPD](ch10-privacy-and-gdpr.md).

**Ne lisez jamais les émotions.** La reconnaissance des émotions sur le lieu de travail est interdite. Gardez la surveillance sur les dangers et l'équipement, jamais sur les sentiments d'un travailleur.

**Protégez les données opérationnelles.** Les données des capteurs, les calendriers de production et les registres de la chaîne d'approvisionnement sont sensibles et précieux. Gardez-les sécurisés et, quand c'est important, dans votre propre environnement. Les bases de sécurité sont dans le [Chapitre 6 — Cybersécurité à l'ère de l'IA](ch06-cybersecurity-in-the-ai-era.md), et l'option d'auto-hébergement dans le [Chapitre 8 — Auto-hébergement : gardez vos données sous contrôle](ch08-self-hosting-keep-your-data-under-control.md).

**Soyez honnête sur les résultats.** Un chiffre de qualité ou d'efficacité qui semble trop beau devrait être vérifié avant que vous le rapportiez. Rapportez les vrais chiffres, y compris les ratés, pour que vous puissiez corriger ce qui est encore cassé.

**Utilisez les données pour améliorer, pas pour punir.** Les données opérationnelles et de sécurité doivent rendre le travail meilleur et plus sûr pour tout le monde. Quand elles deviennent un bâton pour frapper des individus, elles empoisonnent le lieu de travail et cachent les vrais problèmes.

## Erreurs à éviter

**Attendre la panne.** Rester au « faire tourner jusqu'à la casse » quand une réparation planifiée était bon marché et prévisible. Prédisez et agissez tôt.

**Des capteurs sans plan.** Collecter des données sur lesquelles vous n'agissez jamais. Commencez par la machine qui fait le plus mal et reliez chaque capteur à une décision.

**Laisser l'IA arrêter ou jeter toute seule.** Pas de vérification humaine sur un arrêt de ligne ou un rejet de produit. Gardez la décision humaine.

**Des vérifications de vision trop strictes.** Un système qualité qui jette du bon produit parce que le seuil est trop serré. Passez les rejets en revue et réglez-le.

**Inspecter le mauvais défaut.** Mettre de la vision sur un problème bon marché pendant que le coûteux passe au travers. Ciblez d'abord le défaut coûteux.

**Un plan qui ignore le monde réel.** Laisser un plan logistique optimisé foncer dans une perturbation sans court-circuit humain. Gardez une personne prête.

**La reconnaissance des émotions au travail.** Utiliser l'IA pour lire les sentiments des travailleurs. C'est interdit et mal.

**La surveillance secrète.** Ne pas dire aux travailleurs avant qu'une surveillance de sécurité ou d'opérations basée sur l'IA ne commence. Cela enfreint la loi et la confiance.

**La dérive de surveillance.** Utiliser les données de sécurité et d'opérations pour surveiller et punir des individus au lieu de supprimer les dangers.

**Automatiser un processus cassé.** Si la ligne ou la chaîne d'approvisionnement est un désordre, l'IA fait un désordre plus rapide. Réparez d'abord le processus.

**Pas de référence de départ.** Ne pas mesurer le temps d'arrêt, le taux de défauts ou le délai de livraison avant, donc vous ne pouvez pas prouver le gain. Mesurez d'abord (voir le [Chapitre 22 — Mesurer les résultats et le ROI](ch22-measuring-results-and-roi.md)).

**Trop promettre sur les chiffres.** Citer le chiffre du meilleur cas d'un fournisseur comme votre résultat. Utilisez vos propres chiffres mesurés.

## Exercice pratique

### 29.7 Exercice : planifier une automatisation des opérations

Choisissez un métier des opérations et planifiez son assistance IA de bout en bout, avec la sécurité et la décision humaine intégrées.

**Étape 1 — Choisissez le métier.** Choisissez-en un : maintenance prédictive, contrôle qualité, logistique ou sécurité au travail. Faites-en un, pas tous.

**Étape 2 — Définissez l'objectif et la métrique.** Moins de temps d'arrêt ? Moins de défauts ? Livraison plus rapide ? Moins d'incidents de sécurité ? Choisissez un chiffre à mesurer.

**Étape 3 — Mesurez la référence de départ.** Quelle est ce chiffre maintenant ? Heures de temps d'arrêt imprévu, taux de défauts, livraisons à l'heure, incidents par mois. Écrivez-le.

**Étape 4 — Trouvez la cible coûteuse.** Identifiez le seul échec le plus coûteux dans ce métier — la machine dont la panne fait le plus mal, le défaut qui coûte le plus, la route toujours en retard, le danger qui cause le plus de tort. Ciblez celui-là d'abord.

**Étape 5 — Marquez chaque étape.** Pour chaque étape, marquez-la : **l'IA la fait** (percevoir, prédire, inspecter, planifier), **un humain la passe en revue** (confirmer l'avertissement, vérifier le rejet), ou **un humain la décide** (arrêter la ligne, jeter le lot, renvoyer quelqu'un chez lui). Chaque décision critique pour la sécurité doit être humaine.

**Étape 6 — Vérifiez la ligne juridique.** Si le métier implique de surveiller des travailleurs, confirmez que vous regardez les dangers et l'équipement, pas les émotions, et planifiez comment vous informerez les travailleurs et leurs représentants avant de commencer.

**Étape 7 — Connectez les données.** Décidez quels systèmes l'IA a besoin de voir — capteurs, inventaire, suivi — et comment vous les connecterez (voir le [Chapitre 19](ch19-connecting-ai-to-systems-you-already-use.md)).

**Étape 8 — Lancez petit et mesurez.** Faites-le tourner sur une machine, une ligne ou une route d'abord. Comparez la métrique à la référence de départ. Étendez seulement ce qui prouve que ça marche.

Faites un métier bien. L'analyse de la cible coûteuse à l'étape 4 a de la valeur à elle seule — elle vous montre où votre opération perd réellement le plus d'argent ou cause le plus de tort, ce qui est utile même avant d'acheter un outil.

## Liste de contrôle

### 29.8 Liste de contrôle des opérations et de la production

Avant d'automatiser toute tâche opérationnelle, vérifiez ceci.

- [ ] **Vous avez mesuré la référence de départ** — temps d'arrêt, taux de défauts, délai de livraison, incidents de sécurité.
- [ ] **Vous avez ciblé l'échec le plus coûteux d'abord**, pas le plus facile.
- [ ] **Un humain prend chaque décision critique pour la sécurité** — arrêter une ligne, jeter un lot.
- [ ] **La maintenance prédictive est reliée à une action réelle**, pas seulement à des données collectées.
- [ ] **Les vérifications qualité sont réglées** pour ne pas jeter du bon produit.
- [ ] **L'IA logistique peut voir vos commandes, votre stock et vos livraisons ensemble.**
- [ ] **Un humain peut court-circuiter le plan optimisé** quand le monde réel le perturbe.
- [ ] **La surveillance de sécurité guette les dangers et l'équipement, jamais les émotions** (la reconnaissance des émotions est interdite).
- [ ] **Vous avez informé les travailleurs et leurs représentants** avant toute surveillance IA qui les affecte.
- [ ] **Les données opérationnelles sont gardées sécurisées**, pas envoyées à des services d'IA publics.
- [ ] **Vous utilisez les données pour supprimer les dangers et améliorer le processus**, pas pour punir des individus.
- [ ] **Vous réparez le processus cassé avant de l'automatiser.**
- [ ] **Vous rapportez vos propres chiffres mesurés**, pas le meilleur cas du fournisseur.

Si une case est vide, le risque — pour votre produit, votre personnel ou votre confiance — reste le vôtre. Remplissez-la avant de laisser l'IA près de l'atelier.

## Points à retenir

- L'IA dans les opérations est une sentinelle et une aide : elle perçoit, prédit, inspecte et planifie, tandis qu'un humain garde chaque décision critique pour la sécurité.
- Le cas SOK Finance (une annonce de CGI) a mis une IA multi-agents sur AWS Bedrock en production en direct dans un centre de services desservant un réseau d'environ 2 000 points de vente, accélérant les demandes de routine comme les copies de facture et les changements de date d'échéance, avec des humains supervisant les exceptions.
- La maintenance prédictive transforme une panne surprise en une réparation planifiée bon marché ; le contrôle qualité par vision par ordinateur vérifie chaque unité de façon cohérente au lieu d'échantillonner avec des yeux fatigués.
- Dans la sécurité au travail, surveillez les dangers et l'équipement de protection — jamais les émotions des travailleurs, que le règlement européen sur l'IA interdit — et prévenez les travailleurs avant toute surveillance qui les affecte.
- Ciblez l'échec le plus coûteux d'abord, gardez un court-circuit humain pour les perturbations du monde réel, et mesurez votre propre référence de départ avant de faire confiance au chiffre d'un fournisseur.

<!-- BEGIN agentbridge-examples -->

## Essayez avec AgentBridge

Voici à quoi ressemble le même travail avec AgentBridge. Chaque encadré montre le résultat fini et la seule ligne que vous tapez pour l'obtenir.

### Garder le stock en ordre

![Une feuille d'inventaire avec les articles en stock bas surlignés](../../assets/examples/inventory-list.png)
*Une feuille d'inventaire avec les articles en stock bas surlignés*

**Ce que vous demandez :** `Fais un tableur d'inventaire avec article, quantité, seuil de réapprovisionnement et fournisseur, et surligne ce qui est sous le seuil de réapprovisionnement.`

L'agent met en place la feuille d'inventaire et marque les articles à réapprovisionner. Mettez à jour les quantités et demandez-lui de revérifier à tout moment.

*Conseil : Une vérification hebdomadaire planifiée peut vous dire quoi réapprovisionner avant que vous n'ayez plus de stock.*

---

### Planifier une tournée de livraison

![Une tournée de livraison tracée sur la carte entre les arrêts](../../assets/examples/delivery-route.png)
*Une tournée de livraison tracée sur la carte entre les arrêts*

**Ce que vous demandez :** `Planifie le meilleur itinéraire pour ces cinq adresses de livraison et montre-le sur une carte.`

L'agent place les arrêts sur une carte dans un ordre efficace et vous donne la distance et le temps estimé. Vous suivez la tournée et économisez du carburant.

*Conseil : Ajoutez des créneaux horaires (« arrêt B avant midi ») et l'agent en tient compte.*

---

### Est-ce en stock ?

![Une vérification de stock en direct répondue en quelques secondes](../../assets/examples/stock-check.png)
*Une vérification de stock en direct répondue en quelques secondes*

**Ce que vous demandez :** `Avons-nous l'article SKU 3391 en stock, et combien ?`

L'agent vérifie le stock dans votre système et répond avec la quantité, pour que vous puissiez promettre ou promettre prudemment en toute confiance.

*Conseil : Associez-le à une alerte de stock bas planifiée chaque jour pour éviter les surprises.*

<!-- END agentbridge-examples -->
