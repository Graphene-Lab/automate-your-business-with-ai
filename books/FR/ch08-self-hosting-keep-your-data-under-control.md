# Chapitre 8 — L'auto-hébergement : gardez vos données sous contrôle

## En mots simples

L'auto-hébergement signifie faire tourner un logiciel sur des ordinateurs que vous possédez ou contrôlez, au lieu de le louer sur les ordinateurs de quelqu'un d'autre.

Vous connaissez déjà les deux côtés de ceci. Louer une chambre d'hôtel, c'est le cloud : quelqu'un d'autre nettoie, répare, et garde un double des clés. Posséder une maison, c'est l'auto-hébergement : vous réparez la chaudière vous-même, mais personne d'autre n'a de clé.

Appliqué à l'IA, l'auto-hébergement signifie que le modèle — le logiciel qui fait le raisonnement — tourne sur une machine dans votre bureau ou sur un serveur que vous contrôlez. Vos questions entrent là-dedans. Les réponses sortent de là. Rien ne voyage sur internet vers une entreprise que vous n'avez pas choisie.

Ce n'était pas possible pour une petite entreprise jusqu'à récemment. Jusqu'en 2022, les meilleurs modèles de langage vivaient uniquement dans des centres de données géants, et on ne pouvait les atteindre que par une porte louée appelée API — une interface standard qu'une entreprise ouvre pour que d'autres logiciels puissent poser des questions à ses systèmes. Chaque question que vous tapiez passait par cette porte et atterrissait sur leurs machines.

Puis deux choses ont changé. D'abord, des modèles ouverts sont apparus : des modèles dont les fichiers entraînés peuvent être téléchargés et exécutés par n'importe qui. Ensuite, les techniques de compression sont devenues assez bonnes pour qu'un modèle compressé tourne sur un ordinateur de bureau ordinaire mais puissant, avec seulement une petite perte de qualité.

L'échange est un triangle, et vous ne pouvez pas avoir les trois coins à la fois.

- **Le contrôle.** Vous décidez ce qui arrive à vos données, quel modèle vous utilisez, quand il change, et qui peut le voir.
- **La capacité.** À quel point l'IA est réellement bonne sur les tâches difficiles.
- **Le coût.** Ce que vous payez, en argent, temps et attention.

L'IA dans le cloud donne une grande capacité pour un faible effort et un faible contrôle. L'auto-hébergement donne un grand contrôle, une capacité modérée, et un coût que vous payez d'avance en matériel puis encore en temps continu. La bonne réponse dépend de ce que vous faites.

Deux phrases honnêtes avant d'aller plus loin. L'auto-hébergement n'est pas automatiquement plus sûr — un serveur local mal configuré est pire qu'un service cloud bien géré. Et l'auto-hébergement n'est pas automatiquement moins cher — à petite échelle, la location gagne en général. Ce que l'auto-hébergement achète est une chose précise et précieuse : vos données ne partent pas, et personne ne peut changer votre système sans que vous le sachiez.

Sujets liés ailleurs : le [Chapitre 11](ch11-digital-sovereignty.md) couvre l'idée plus large de contrôler vos propres outils numériques, le [Chapitre 9](ch09-third-party-services-and-shadow-ai.md) couvre le schéma opposé des services tiers non gérés, et le [Chapitre 6](ch06-cybersecurity-in-the-ai-era.md) couvre les bases de sécurité qui s'appliquent toujours à une machine dans votre propre bureau.

## Un peu d'histoire

**Années 1990 à 2000 : tout à la maison.** Une petite entreprise avait un serveur dans un placard. Email, fichiers et comptes étaient tous sur place. Vous possédiez la machine et tous ses problèmes.

**Années 2000 à 2018 : le départ.** Le haut débit est devenu rapide, et louer est devenu plus facile que posséder. L'email est parti en premier, puis les fichiers, puis la comptabilité et les dossiers clients. « Le cloud » est devenu la réponse par défaut. La blague chez les ingénieurs était exacte : il n'y a pas de cloud, c'est juste l'ordinateur de quelqu'un d'autre.

**2013 : les conteneurs.** Docker est arrivé et a empaqueté les logiciels pour qu'ils tournent de la même façon partout. Cela a discrètement rendu l'auto-hébergement facile de nouveau, parce que vous n'aviez plus besoin d'un spécialiste pour reconstruire une application sur chaque nouvelle machine.

**2022 : l'IA n'était qu'une location.** Les meilleurs modèles de langage n'existaient que dans une poignée de grandes entreprises. Si vous vouliez de l'IA, vous leur envoyiez votre texte. Il n'y avait pas d'alternative qui vaille la peine d'être utilisée.

**2023 : l'année des modèles ouverts.** Meta a publié Llama comme modèle de recherche en février, puis Llama 2 avec des poids ouverts en juillet. Mistral AI a publié un puissant modèle de sept milliards de paramètres en août. « Poids ouverts » signifie que les fichiers entraînés sont publiés, donc n'importe qui peut les télécharger et les exécuter. La même année, la quantification — compresser un modèle pour qu'il ait besoin de beaucoup moins de mémoire — est devenue assez bonne pour un usage quotidien. D'un coup, une IA capable n'était plus seulement dans un centre de données.

**8 juillet 2023 : Ollama.** Un outil appelé Ollama a été publié, open source sous licence MIT, écrit principalement en Go avec un peu de C et de TypeScript, par Jeffrey Morgan et Michael Chiang. Son travail était de supprimer toute la friction. Une seule commande télécharge un modèle et le fait tourner localement, avec une interface simple et un service local auquel d'autres programmes peuvent parler. Il utilisait le moteur llama.cpp pour le travail réel sur votre matériel.

**2024 : « souverain » devient un critère d'achat.** Des entreprises de secteurs régulés, et plusieurs gouvernements européens, ont commencé à demander une IA qui reste dans un pays et dans leurs propres murs. Les fournisseurs cloud ont répondu avec des options de cloud souverain, et un marché pour l'IA sur site a grandi rapidement.

**2026 : un client open source d'entreprise.** En avril 2026, MZLA Technologies, une filiale de Mozilla, a annoncé Thunderbolt, un client IA open source conçu pour être auto-hébergé. La section Curiosité le couvre.

La forme de cette histoire est une boucle. Nous avons commencé en auto-hébergement, sommes partis pour la commodité, et revenons maintenant pour le contrôle — avec des outils bien meilleurs que la première fois.

## Curiosité

### 8.7 Le client IA open source de Mozilla pour « une IA que vous contrôlez »

En avril 2026, MZLA Technologies Corporation — une filiale à part entière de Mozilla, l'organisation à but non lucratif derrière Firefox — a annoncé **Thunderbolt**. C'est un client IA open source, multiplateforme, conçu pour les organisations qui veulent faire tourner l'IA selon leurs propres conditions.

Les détails qui comptent pour ce chapitre :

- **Auto-hébergeable.** Il tourne sur la propre infrastructure du client. Le projet décrit la prise en charge de configurations sur site, cloud souverain et isolées (air-gapped) — ce qui signifie un réseau physiquement déconnecté d'internet.
- **Agnostique au modèle.** Il fonctionne avec tout agent qui parle l'Agent Client Protocol, et avec tout modèle qui offre une API compatible OpenAI. En pratique, cela signifie que vous pouvez le diriger vers un modèle local, votre propre serveur, ou un fournisseur commercial, et changer sans changer vos outils.
- **Partout.** Web, Windows, macOS, Linux, iOS et Android.
- **Connecté à vos systèmes.** Il s'intègre aux systèmes d'entreprise via le Model Context Protocol — une façon standard de laisser un outil IA atteindre vos données et actions internes — et prend en charge des automatisations réutilisables et une API extensible.
- **Auditable.** Parce que le code est ouvert, vous ou un tiers pouvez le lire et vérifier ce qu'il fait réellement. Le projet a dit qu'il passe par un audit de sécurité.
- **Un partenaire pour la souveraineté européenne.** Il s'associe à Haystack de deepset, une plateforme d'orchestration open source, pour des déploiements souverains en Europe.
- **Assistance incluse.** Le support d'entreprise et l'ingénierie déployée en amont sont offerts, ce qui est la partie que la plupart des projets open source vous laissent résoudre seul.

Le positionnement vaut d'être remarqué. Le cadre est « une IA que vous contrôlez », et l'argument est que l'IA est trop importante pour être entièrement externalisée. C'est le même argument qu'un petit patron d'entreprise fait quand il décide de garder les fichiers de paie sur sa propre machine plutôt que dans un service qu'il n'a jamais inspecté.

Un exemple plus petit et plus ancien de la même idée se trouve dans une application email que beaucoup utilisent déjà. L'add-on ThunderAI pour Thunderbird a ajouté la prise en charge des modèles locaux via Ollama dans la version 2.1.1, publiée en août 2024. Avec cette configuration, le modèle tourne sur votre propre ordinateur, donc le texte de l'email ne quitte jamais la machine, et aucun compte cloud ni clé API n'est nécessaire. C'est une petite fonctionnalité, et elle fait le point clairement : l'IA locale n'est plus un projet de recherche. C'est une option dans un client email gratuit.

## Un exemple d'entreprise réel

### Même Apple a construit son propre cloud

Apple est une entreprise qui pourrait louer presque n'importe quoi. En juin 2024, elle a annoncé un système appelé Private Cloud Compute, construit pour les fonctionnalités IA de ses appareils quand une tâche est trop grosse pour le téléphone lui-même. Ce qu'elle a choisi de faire de ce système est la leçon.

Apple a construit ses propres serveurs autour de ses propres puces avec un système d'exploitation durci. Elle a conçu le système pour une inférence sans état — traiter la requête, renvoyer la réponse, ne rien garder. Et elle a fait une promesse inhabituelle : elle publierait l'image logicielle de chaque version de production pour que des chercheurs en sécurité extérieurs puissent inspecter exactement ce qui tourne, et vérifier que la machine à qui ils parlent est vraiment ce qu'elle prétend être. En octobre 2024, Apple a publié un guide de sécurité et invité les chercheurs à attaquer le système.

Trois choses en découlent pour une petite entreprise.

D'abord, remarquez le raisonnement. Apple n'a pas construit un cloud parce qu'il ne pouvait pas en louer un. Il en a construit un parce que louer aurait signifié garder les données des utilisateurs selon les conditions de quelqu'un d'autre, et toute sa marque est de ne pas le faire. Le contrôle de la machine valait de l'argent réel pour eux.

Ensuite, remarquez l'idée de vérification. Publier le logiciel pour que des extérieurs puissent le vérifier est le même instinct que l'audit open source. La confiance est réduite en rendant le système inspectable, pas en promettant d'être bon.

Enfin, remarquez la taille de l'écart. Apple a dépensé une fortune pour atteindre « nous ne gardons rien ». La plupart des petites entreprises ne peuvent pas copier cela. Mais vous pouvez copier la question : *qui dirige la machine où vont mes données, que gardent-ils, et quelqu'un peut-il vérifier ?* Si vous ne pouvez pas répondre à ces trois questions sur un outil, vous ne devriez pas y mettre de données sensibles. Et si la réponse honnête est « nous ne pouvons pas vérifier », un modèle tournant sur votre propre machine devient une sérieuse option.

## Comment faire

### 8.5 Comment commencer : des outils open source comme Ollama aux modèles locaux

**Étape 1 : Choisissez une tâche et une personne.**
N'achetez pas du matériel d'abord. Choisissez une tâche répétée qui implique des données sensibles — résumer des contrats, rédiger des réponses aux demandes courantes, transformer des notes de réunion en listes d'actions. Donnez-la à une personne curieuse avec un bon ordinateur.

**Étape 2 : Installez Ollama.**
Ollama tourne sur Windows, macOS et Linux. Après l'installation, une seule commande tire un modèle et démarre un chat dans votre terminal. Sous le capot, il démarre un petit service sur votre propre machine, sur le port 11434, auquel d'autres programmes peuvent parler. C'est ce service local qui vous permet de connecter le modèle à vos propres outils plus tard.

**Étape 3 : Choisissez le modèle par taille, pas par nom.**
Les tailles de modèles se comptent en paramètres, une mesure approximative de la grosseur et de la capacité du modèle. Comme règle empirique :

- **1 à 3 milliards** — rapide et léger, tourne sur un ordinateur portable ordinaire. Bon pour de courts résumés et une rédaction simple.
- **7 à 9 milliards** — le milieu pratique. Bonne qualité générale, a besoin d'une machine correcte avec assez de mémoire.
- **70 milliards et plus** — beaucoup plus fort, mais a besoin d'un matériel sérieux et de beaucoup de mémoire. Habituellement pas un point de départ de petite entreprise.

Cherchez les versions **quantifiées**. La quantification compresse les nombres à l'intérieur du modèle pour qu'il ait besoin de beaucoup moins de mémoire et tourne plus vite, au prix d'une petite baisse de qualité. Pour la plupart des tâches de bureau, cette baisse est acceptable.

**Étape 4 : Ajoutez une interface conviviale.**
Le terminal va bien pour tester. Pour un usage quotidien, ajoutez une interface de chat qui tourne localement, ou branchez le modèle dans une application que les gens utilisent déjà — l'add-on Thunderbird mentionné plus haut en est un exemple. Le but est qu'un collègue non technique puisse l'utiliser sans aide. Si une seule personne peut le piloter, il ne sera jamais adopté.

**Étape 5 : Gardez-le réellement local.**
C'est là que les gens échouent. Le service local doit écouter seulement sur votre propre machine, pas sur tout le réseau. Des chercheurs en sécurité ont trouvé beaucoup de serveurs Ollama exposés à l'internet public parce qu'ils étaient configurés pour accepter des connexions de n'importe quelle adresse. Donc : gardez la liaison locale par défaut, mettez un pare-feu devant, n'ouvrez jamais le port 11434 sur internet, et ne le faites pas tourner avec des droits d'administrateur. Un outil local n'est pas automatiquement un outil sûr.

**Étape 6 : Laissez-le lire vos propres fichiers.**
La prochaine étape la plus utile est la récupération (retrieval), souvent appelée RAG. En mots simples : au lieu de réentraîner le modèle, vous mettez vos documents dans un index consultable. Quand quelqu'un pose une question, le système trouve les passages pertinents et les remet au modèle avec la question. Le modèle répond à partir de vos documents. Rien n'est entraîné sur vos données, et tout cela peut tourner sur votre propre machine. C'est ainsi qu'on obtient « demande à notre manuel » sans envoyer le manuel nulle part.

**Étape 7 : Ne passez à l'échelle que si le test a fonctionné.**
Si le pilote est utile, alors achetez du matériel. Une station de travail avec une carte graphique puissante est la réponse habituelle, parce que la mémoire graphique est ce qui limite la taille du modèle que vous pouvez faire tourner. Les machines Apple avec mémoire unifiée sont un choix courant pour la même raison. Un petit serveur a du sens quand plusieurs personnes en ont besoin en même temps.

**Étape 8 : Décidez de la répartition.**
La plupart des entreprises finissent hybrides. Les données sensibles et les tâches répétitives à gros volume tournent localement. Le raisonnement difficile, les très longs documents et les fonctionnalités spécialisées utilisent un service cloud sous un contrat approprié. Écrivez la règle : quelles données vont où, et qui décide.

### 8.6 Cas d'usage idéaux

**Données personnelles sensibles.** Dossiers de santé, dossiers RH, paie, CV de candidats, détails financiers des clients. Si les données ne doivent pas partir, le traitement local supprime entièrement la question.

**Informations propriétaires.** Designs, dessins, code source, documents d'appel d'offres et de soumission, modèles de prix, plans stratégiques. Ce sont les fichiers qui feraient le plus mal si un fournisseur les gardait ou les fuitait.

**Secteurs régulés.** Santé, cabinets juridiques, banque et assurance, gouvernement et défense, et toute entreprise sous des règles de résidence des données qui exigent que les données restent dans un pays ou une région. L'auto-hébergement transforme une dure conversation de conformité en une conversation simple.

**Connectivité faible ou nulle.** Champs de travail, usines, navires, mines, bureaux éloignés, intervention d'urgence. Un modèle local fonctionne quand internet ne le fait pas.

**Travail répétitif à gros volume.** Des milliers de tickets, factures ou documents. Un prix par requête fait mal en volume ; une machine fixe ne grossit pas.

**Expérimentation bon marché.** Essayer des idées sans compteur qui tourne. Utile avant d'engager un budget.

**Où cela colle mal :** raisonnement de pointe, très longs documents, génération d'images avancée, et toute équipe sans aucun support technique. Si personne ne peut le maintenir, ne commencez pas.

## Éthique et responsabilité

L'auto-hébergement résout un problème éthique et en crée d'autres. Soyez clair sur lequel est lequel.

**Ce qu'il résout.** Vos données clients cessent de voyager vers des entreprises que vous n'avez pas choisies, et ne peuvent pas être utilisées pour entraîner le produit de quelqu'un d'autre à votre insu. C'est un vrai gain de respect pour les personnes dont vous détenez les données.

**Ce qu'il ne résout pas.** Le modèle peut encore être faux, biaisé ou trompeur avec assurance. Faire tourner un modèle biaisé sur votre propre matériel ne le rend pas juste. Les devoirs du [Chapitre 4](ch04-ethical-ai-doing-the-right-thing.md) s'appliquent toujours, et les règles de divulgation du [Chapitre 5](ch05-rules-and-legal-responsibility.md) aussi.

**Ce qu'il ajoute.** Vous êtes maintenant l'opérateur. Les correctifs, le contrôle d'accès, la journalisation et les sauvegardes sont votre travail. Si un serveur local non corrigé fuit des données, c'est sur vous d'une façon nouvelle et très directe.

**Surveillance des employés.** Si vous journalisez les invites dans un système local, vous détenez maintenant un dossier détaillé de ce que votre personnel a demandé. Ayez une politique écrite sur ce qui est gardé, pourquoi, qui le lit, et pour combien de temps. Restez proportionné, et dites-le aux gens.

**Ne survendez pas la souveraineté.** « Souverain » est un mot de marketing autant qu'un mot technique. Si vous prétendez au contrôle mais ne pouvez pas corriger, sauvegarder ou auditer, la prétention est vide. Dites ce que vous avez réellement, et dites clairement ce que vous n'avez pas.

**Énergie.** Une machine qui fait tourner des modèles toute la journée consomme de l'électricité. Le local n'est pas automatiquement plus écologique qu'un grand centre de données efficace. Si vous revendiquez un bénéfice environnemental, vérifiez-le d'abord.

## Erreurs à éviter

1. **Acheter du matériel avant de tester une tâche.** Testez d'abord avec une configuration louée ou empruntée. Le matériel acheté sur l'espoir reste inutilisé.
2. **Exposer le service IA local à internet.** C'est l'erreur d'auto-hébergement la plus courante et la plus grave. Gardez-le local, pare-feu, n'ouvrez pas le port.
3. **Supposer que local égale sécurisé.** Vous possédez maintenant la sécurité de cette machine, y compris les parties auxquelles vous n'avez jamais pensé.
4. **Pas de sauvegardes.** La machine, les modèles, la configuration et l'index de documents ont tous besoin d'être sauvegardés.
5. **Choisir le plus gros modèle.** Plus gros est plus lent, plus gourmand, et souvent pas meilleur pour votre tâche réelle.
6. **Ignorer les licences des modèles.** Les modèles à poids ouverts viennent avec des conditions différentes, y compris des règles sur l'usage commercial et sur la façon dont vous pouvez décrire votre usage. Lisez la licence avant de construire dessus.
7. **Dépendance à une seule personne.** Si une seule personne sait comment ça marche et part, le système s'arrête. Écrivez la configuration, le redémarrage et les étapes de restauration.
8. **Auto-héberger la mauvaise charge de travail.** Si la tâche a besoin d'une qualité de pointe, le local décevra, et vous conclurez à tort que la technologie est inutile.
9. **Ne jamais mettre à jour, ou mettre à jour sans tester.** Une nouvelle version de modèle change les réponses. Réexécutez vos tâches d'échantillon après chaque changement.
10. **Le traiter en tout ou rien.** Une configuration hybride est habituellement la bonne réponse, pas un basculement total dans une direction ou l'autre.

## Exercice pratique

### 8.8 Évaluer si l'auto-hébergement convient à votre entreprise

Notez chaque ligne 0, 1 ou 2. Soyez honnête.

| Question | 0 | 1 | 2 |
|---|---|---|---|
| À quel point les données sont-elles sensibles ? | Public | Interne | Confidentiel client ou régulé |
| Support technique disponible | Aucun | Aide informatique à temps partiel | Quelqu'un qui peut maintenir un serveur |
| Budget matériel | Aucun | Une bonne station de travail | Station de travail plus un petit serveur |
| Complexité de la tâche | Résumés et rédaction | Questions sur des documents | Raisonnement complexe, très longs documents |
| Connectivité | Non fiable | Correcte | Correcte |
| Volume | Occasionnel | Quotidien | Élevé et croissant |

Lisez le score ligne par ligne, parce que les lignes ne poussent pas toutes dans le même sens.

- **Sensibilité 2** et **Volume 2** poussent tous deux vers l'auto-hébergement.
- **Support technique 0** pousse fortement contre, quels que soient les autres scores.
- **Complexité de la tâche 2** pousse contre, parce que les modèles locaux sont en retard sur le raisonnement difficile.

Maintenez faites un test d'une journée avant de dépenser quoi que ce soit. Prenez vingt tâches réelles de votre liste. Faites-en dix avec un modèle local de taille moyenne et dix avec un service cloud. Comparez trois choses : la réponse était-elle assez bonne pour être utilisée telle quelle, combien de temps a-t-elle pris, et qu'aurait coûté l'autre façon. Écrivez les résultats.

Si la réponse locale était utilisable pour la plupart des tâches, l'auto-hébergement vaut l'investissement. Si elle n'était utilisable que pour quelques-unes, gardez celles-là en local et laissez le reste dans le cloud sous contrat. Dans les deux cas, vous avez maintenant des preuves au lieu d'une opinion.

## Liste de contrôle

### 8.9 Ce qu'il vous faut pour commencer

- [ ] **Une tâche nommée** qui implique des données sensibles et se répète souvent.
- [ ] **Une personne nommée** qui peut installer, redémarrer, sauvegarder et mettre à jour le système — ou un plan pour en embaucher une.
- [ ] **Une machine avec assez de mémoire**, choisie après un test, pas avant.
- [ ] **Un modèle choisi par taille et quantification**, adapté à la tâche plutôt qu'au plus grand disponible.
- [ ] **Une interface locale** qu'un collègue non technique peut utiliser sans aide.
- [ ] **Le service lié à la machine locale uniquement**, pare-feu, sans port ouvert sur internet.
- [ ] **Une vérification écrite de la licence** pour le modèle que vous choisissez, y compris les conditions d'usage commercial.
- [ ] **Un plan de sauvegarde** pour la machine, les modèles, la configuration et l'index de documents.
- [ ] **Une routine de correctifs** avec une date fixe, et un re-test des tâches d'échantillon après chaque changement.
- [ ] **Une règle de répartition écrite** indiquant quelles données restent locales et lesquelles peuvent utiliser un service cloud, et qui décide.

## Points à retenir

- L'auto-hébergement signifie que l'IA tourne sur des machines que vous contrôlez, donc vos données ne les quittent pas.
- Elle est devenue pratique pour les petites entreprises quand les modèles à poids ouverts et une bonne compression sont arrivés en 2023, et des outils comme Ollama ont supprimé la friction de configuration.
- Vous échangez la capacité et la commodité contre le contrôle : le triangle est contrôle, capacité et coût, et vous ne pouvez pas avoir les trois.
- Le local n'est pas automatiquement sûr ou bon marché ; un serveur local mal configuré est un risque réel, et la maintenance est maintenant votre travail.
- Commencez par une tâche, une personne, et un test d'une journée avant d'acheter le moindre matériel.
