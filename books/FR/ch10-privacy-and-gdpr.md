# Chapitre 10 — Confidentialité et RGPD : ce que vous devez vraiment savoir

## En mots simples

RGPD signifie Règlement Général sur la Protection des Données. C'est le règlement de l'Union européenne pour traiter les données personnelles — toute information sur une personne vivante qui peut être identifiée. C'est l'une des lois sur la vie privée les plus strictes au monde, et elle touche bien plus d'entreprises que la plupart des patrons ne le pensent.

Toute la loi peut se réduire à une idée : **si vous détenez des informations sur une personne, vous devez les traiter équitablement, pour une raison claire, ne garder que ce dont vous avez besoin, les garder en sécurité, et respecter ce que cette personne vous demande d'en faire.**

Vous êtes concerné si vous êtes dans l'UE, et aussi si vous êtes hors de l'UE mais proposez des biens ou des services à des personnes dans l'UE, ou observez leur comportement. Une petite boutique en ligne dans un autre pays qui vend à des clients en France est dans le champ du RGPD. On appelle cela la portée extraterritoriale, et cela surprend beaucoup d'entreprises.

Pourquoi cela compte-t-il pour l'IA ? Parce que l'IA tourne sur des données, et une grande partie de ces données est personnelle. Noms de clients, emails de support, CV, dossiers d'employés, visiteurs du site web — tout cela est des données personnelles. Quand vous en envoyez une partie dans un outil d'IA, vous traitez des données personnelles, et les règles s'appliquent. Si vous envoyez ces données à un service tiers, les règles les suivent dehors. C'est le lien avec le [Chapitre 9](ch09-third-party-services-and-shadow-ai.md).

Ce chapitre est le foyer approfondi du RGPD dans ce livre. Il explique les principes, les types de données, les bases légales, vos obligations, et les droits que les personnes détiennent sur vous. L'AI Act européen — une loi distincte sur les systèmes d'IA eux-mêmes — est traité en entier au [Chapitre 5](ch05-rules-and-legal-responsibility.md) ; ici nous ne regardons que là où il touche la vie privée. Le volet sécurité pour protéger les données est au [Chapitre 6](ch06-cybersecurity-in-the-ai-era.md).

Une note honnête : ceci est un guide simple, pas un conseil juridique. Pour de vraies décisions, surtout au-delà des frontières, parlez à un professionnel de la protection des données.

## Un peu d'histoire

**1995 : la première règle européenne.** La directive sur la protection des données a fixé des normes précoces en Europe, mais chaque pays l'a mise en œuvre différemment, créant un patchwork.

**27 avril 2016 : le RGPD est adopté.** L'UE a remplacé le patchwork par un seul règlement, conçu pour s'appliquer de la même façon dans chaque État membre et moderniser les règles pour l'ère d'internet.

**25 mai 2018 : le RGPD s'applique.** C'est la date qui compte. À partir de ce jour, les règles étaient pleinement en vigueur, avec de lourdes amendes pour les violations graves. Les entreprises du monde entier devaient se conformer ou risquer ces amendes.

**2018 à 2023 : l'ère de l'application.** Les autorités nationales de protection des données ont infligé des amendes, certaines très importantes, pour des violations et de mauvaises pratiques. La confidentialité est devenue un sujet de conseil d'administration, pas seulement un problème d'avocat.

**2018 : le CEPD.** Le Comité européen de la protection des données a été créé pour coordonner les autorités nationales et publier des orientations afin que la loi soit appliquée de façon cohérente dans toute l'UE. Ses orientations sont l'endroit où regarder quand la loi est floue.

**1er août 2024 : l'AI Act européen entre en vigueur.** Une loi distincte, le règlement (UE) 2024/1689, a commencé son déploiement par étapes. Il réglemente les systèmes d'IA selon le risque. Il ne remplace pas le RGPD. Quand un système d'IA utilise des données personnelles, les deux lois s'appliquent à la fois.

## Curiosité

### 10.9 Ce que les régulateurs européens de la vie privée ont dit sur les modèles d'IA

En décembre 2024, le Comité européen de la protection des données (CEPD) — l'organe qui coordonne tous les régulateurs nationaux de la vie privée de l'UE — a adopté l'**Avis 28/2024**, sur la protection des données personnelles dans le contexte des modèles d'IA. C'est la déclaration sur la vie privée la plus importante à ce jour sur la façon dont l'IA s'articule avec le RGPD.

Quelques points comptent pour un patron d'entreprise :

**Un modèle peut être examiné en trois étapes.** Le CEPD sépare la vie d'un modèle d'IA en développement (l'entraîner), déploiement (le mettre au travail) et utilisation (les personnes qui interagissent avec lui). Chaque étape peut impliquer des données personnelles, et chacune a ses propres questions de confidentialité. C'est utile parce que cela vous dit de poser la question à chaque étape, pas seulement au début.

**L'intérêt légitime peut être une base légale, mais ce n'est pas un laissez-passer.** L'avis dit qu'une entreprise peut s'appuyer sur l'« intérêt légitime » pour développer ou utiliser un modèle d'IA, mais seulement si le traitement est réellement nécessaire et qu'un test de mise en balance montre qu'il ne l'emporte pas sur les droits des personnes. Vous ne pouvez pas simplement déclarer un intérêt et ignorer les personnes concernées.

**Un modèle n'est « anonyme » que si on ne peut pas en extraire de données personnelles.** C'est le point pointu. Le CEPD dit que pour qu'un modèle soit traité comme anonyme — et donc hors du RGPD —, il doit être très improbable que quelqu'un puisse extraire des données personnelles de lui en lui posant des questions. Si un modèle peut être piégé pour répéter des détails personnels qu'il a mémorisés pendant l'entraînement, il n'est pas vraiment anonyme, et les règles de protection des données s'appliquent toujours.

**De mauvaises données d'entraînement peuvent suivre le modèle.** L'avis avertit que si un modèle a été entraîné sur des données personnelles traitées illégalement, cela peut affecter la licéité de son déploiement plus tard, à moins que le modèle n'ait été correctement anonymisé. En mots simples : un modèle construit sur des données sales peut rester sale, et l'utiliser peut rapporter ce problème dans votre entreprise.

Le message pratique pour une petite entreprise est clair. Quand vous choisissez un fournisseur d'IA, la question de confidentialité n'est pas seulement « que faites-vous de mes données maintenant », mais « sur quelles données ce modèle a-t-il été entraîné, et peut-on retirer des données personnelles de lui ? ». Cette question a sa place dans votre liste de contrôle fournisseur.

## Un exemple d'entreprise réel

### L'outil RH et la demande d'accès

Une entreprise de taille moyenne de 120 employés adopte un outil d'IA pour filtrer les candidatures. Elle téléverse des CV et des lettres de motivation — toutes des données personnelles, certaines sensibles, car un CV peut révéler des périodes de maladie, l'âge, la nationalité et l'activité syndicale. L'outil classe les candidats.

Trois mois plus tard, une candidate rejetée écrit à l'entreprise. Elle fait une **demande d'accès** : en vertu du RGPD, elle a le droit de savoir quelles données personnelles l'entreprise détient sur elle et comment elles ont été utilisées. L'entreprise doit répondre, généralement sous un mois et gratuitement.

Désormais, l'entreprise doit répondre à des questions difficiles qu'elle ne s'est jamais posées. Où sont stockés son CV et le classement de l'IA ? Peut-elle produire les données et expliquer la logique ? Y avait-il une base légale pour traiter son CV avec cet outil ? A-t-elle fait une évaluation des risques d'abord ? Si l'outil était un service tiers, le contrat couvrait-il tout cela ? Si le classement de l'IA compte comme une décision automatisée ayant un effet sérieux sur elle, des règles supplémentaires s'appliquent, y compris son droit de ne pas faire l'objet d'une décision purement automatisée ayant des effets juridiques ou similaires significatifs.

L'entreprise s'agite parce qu'elle a adopté l'outil avant de réfléchir aux données. La leçon est l'ordre des opérations : vous devez comprendre les données et la base légale **avant** d'allumer l'outil, pas quand une demande arrive. Le reste de ce chapitre vous donne les pièces pour faire cela.

## Comment faire

### 10.1 Le RGPD sur une page : les principes de base

Le RGPD repose sur quelques principes. Si vous les respectez, vous respectez la majeure partie de la loi.

**Licéité, équité, transparence.** Vous avez besoin d'une raison légale valide pour traiter des données personnelles, vous ne devez pas les utiliser de façons que les gens jugeraient injustes, et vous devez dire aux gens ce que vous faites.

**Limitation de la finalité.** Collectez les données pour une finalité claire et déclarée. Ne les réutilisez pas plus tard pour quelque chose d'étranger sans une nouvelle base légale.

**Minimisation des données.** Collectez seulement ce dont vous avez réellement besoin. Si vous n'avez pas besoin d'un numéro de téléphone, ne le demandez pas. Cela compte pour l'IA : ne déversez pas toute votre base de données dans un outil quand une petite tranche suffirait.

**Exactitude.** Gardez les données correctes et mettez-les à jour. Les personnes peuvent exiger des corrections.

**Limitation de la conservation.** Ne gardez pas les données personnelles plus longtemps que nécessaire. Ayez un calendrier de suppression.

**Intégrité et confidentialité.** Gardez-les sécurisées contre les violations. Le mode d'emploi est au [Chapitre 6](ch06-cybersecurity-in-the-ai-era.md).

**Responsabilité.** Vous devez pouvoir *montrer* que vous vous conformez — avec des registres, des politiques et des documents. C'est pourquoi la paperasse de la section Liste de contrôle n'est pas facultative.

### 10.2 Données personnelles, données sensibles, données anonymes : les différences qui comptent

**Donnée personnelle** : toute information sur une personne vivante qui peut être identifiée, directement ou indirectement. Un nom, un email, un numéro de téléphone, une photo, un numéro d'identité, une localisation, un identifiant en ligne comme un ID de cookie. Même une combinaison de détails qui individualise quelqu'un compte. Si vous pouvez désigner une personne, c'est une donnée personnelle.

**Donnée sensible** (la loi parle de « catégories particulières ») bénéficie d'une protection plus forte. Elle comprend : origine raciale ou ethnique, opinions politiques, convictions religieuses ou philosophiques, appartenance syndicale, données génétiques, données biométriques servant à identifier une personne, données de santé, et données concernant la vie sexuelle ou l'orientation sexuelle d'une personne. La règle est que traiter ces données est interdit sauf si une condition spécifique s'applique, comme un consentement explicite ou une exigence légale claire. En IA, surveillez-les cachées dans les CV, les tickets de support et les dossiers RH. Un chatbot qui apprend « ce client suit une chimiothérapie » a touché des données de santé.

**Donnée anonyme** : une information qui ne peut plus identifier une personne, même en la combinant avec d'autres données. Une donnée vraiment anonyme est hors du RGPD, car il n'y a pas de personne identifiable. Mais la vraie anonymité est difficile à atteindre. Si vous pouviez réidentifier quelqu'un, ce n'est pas anonyme. C'est la différence qui piège les gens, et c'est le sujet de la section 10.8.

La règle pratique : traitez presque tout ce qui concerne un client, un employé ou un candidat comme une donnée personnelle par défaut. Traitez tout ce qui touche la santé, les croyances ou l'identité comme sensible, et manipulez-le avec une soin particulier. N'appelez une donnée anonyme que si vous avez réellement supprimé la capacité d'identifier quiconque.

### 10.3 Le consentement : quand il est nécessaire et quand il ne l'est pas

Le consentement est une base légale de traitement, pas la seule, et il est souvent mal compris.

Pour être valide, le consentement doit être **librement donné, spécifique, éclairé et non ambigu**, et donné par un acte clair. Une case pré-cochée n'est pas un consentement. Des clauses enfouies ne sont pas un consentement. Un consentement pour « le marketing et tout le reste » n'est pas un consentement valide.

Vous avez besoin d'un consentement quand aucune autre base ne s'applique, et toujours pour les données sensibles dans la plupart des cas, et pour certaines choses comme les emails marketing aux consommateurs dans beaucoup de pays de l'UE.

Vous n'avez souvent **pas** besoin de consentement quand une autre base s'applique. Si vous traitez des données pour exécuter un contrat que vous avez avec le client, c'est la base « contrat », pas le consentement. Si une loi vous oblige à garder des registres, c'est l'« obligation légale ». Demander un consentement quand vous avez déjà un contrat peut en fait créer des problèmes, car le consentement peut être retiré à tout moment, et alors vous ne pouvez plus livrer ce que vous avez promis.

Pour l'IA, le consentement est délicat. Si vous voulez utiliser les données clients pour entraîner un modèle, un vague « nous pouvons utiliser vos données pour améliorer nos services » ne suffit généralement pas. Vous devez être spécifique, et vous devez laisser les gens dire non sans perdre le service. Le chemin le plus sûr est d'éviter d'avoir besoin d'un large consentement du tout : minimisez les données, utilisez-les seulement là où une vraie base existe, et préférez des entrées non personnelles ou anonymisées pour l'entraînement.

### 10.4 L'intérêt légitime : quand vous pouvez utiliser des données sans consentement explicite

L'intérêt légitime est la base la plus souple et la plus mal utilisée. Elle vous permet de traiter des données personnelles sans consentement quand vous avez une raison d'entreprise réelle et licite — mais seulement après un test soigneux.

Le test a trois parties. **Finalité :** votre raison est-elle légitime ? Améliorer la détection de fraude ou la sécurité du réseau l'est généralement. **Nécessité :** traiter les données personnelles est-il réellement nécessaire pour y arriver, ou pourriez-vous le faire avec moins, ou avec des données anonymes ? **Mise en balance :** vos intérêts l'emportent-ils sur les droits et attentes de la personne ? Une personne raisonnable serait-elle surprise ou lésée ?

Vous devez documenter ce test de mise en balance. Ce n'est pas un sentiment ; c'est une évaluation écrite que vous pouvez montrer.

Pour l'IA, l'intérêt légitime peut couvrir certains usages — par exemple, utiliser les données de support client pour améliorer la qualité du service, si c'est nécessaire et équilibré. Mais il ne vous permet pas de faire quoi que ce soit qu'un client trouverait intrusif. Entraîner un modèle sur des données sensibles sous « intérêt légitime » est très difficile à justifier. Et comme le dit l'avis du CEPD dans la section Curiosité, les tests de nécessité et de mise en balance doivent réellement passer.

La règle empirique : si vous vous sentiriez mal à l'aise d'expliquer l'usage à voix haute à la personne concernée, l'intérêt légitime ne le couvre probablement pas.

### 10.5 Les droits des personnes : accès, rectification, effacement, portabilité

Les personnes détiennent des droits sur leurs données, et vous devez pouvoir les honorer. Les principaux :

**Droit d'être informé.** Vous devez dire aux gens, clairement, quelles données vous collectez et pourquoi, généralement dans un avis de confidentialité.

**Droit d'accès.** Une personne peut demander quelles données vous détenez sur elle et comment vous les utilisez. C'est la demande d'accès de l'exemple. Vous devez en fournir une copie, généralement sous un mois, gratuitement.

**Droit de rectification.** Si les données sont fausses, elles peuvent être corrigées.

**Droit à l'effacement (« droit à l'oubli »).** Ils peuvent vous demander de supprimer leurs données, et vous devez le faire, sauf si une raison légale de les garder l'emporte — par exemple, un dossier fiscal que vous êtes tenu de conserver.

**Droit à la limitation du traitement.** Ils peuvent suspendre la façon dont vous utilisez les données dans certaines situations pendant qu'un litige est réglé.

**Droit à la portabilité des données.** Ils peuvent demander leurs données dans un format structuré, courant et lisible par machine pour pouvoir les déplacer ailleurs. Cela rejoint le problème d'enfermement du [Chapitre 9](ch09-third-party-services-and-shadow-ai.md).

**Droit d'opposition.** Ils peuvent s'opposer à un traitement fondé sur l'intérêt légitime, et au marketing direct.

**Droits autour des décisions automatisées.** En vertu de l'article 22, une personne a le droit de ne pas faire l'objet d'une décision fondée uniquement sur un traitement automatisé ayant un effet juridique ou similaire significatif sur elle, avec des exceptions limitées, et le droit à une intervention humaine. C'est critique pour une IA qui filtre des personnes pour des emplois, du crédit ou des services.

Construisez un processus simple et écrit pour recevoir et répondre à ces demandes dans les délais. Quand vous utilisez une IA tierce, assurez-vous que le fournisseur peut vous aider à produire et supprimer les données, sinon vous ne pouvez pas honorer la demande.

### 10.6 L'AI Act européen : ce qui change pour la vie privée

L'AI Act européen est une loi distincte du RGPD, et elle est traitée en entier au [Chapitre 5](ch05-rules-and-legal-responsibility.md). Voici seulement l'angle de la vie privée, pour que les deux ne soient pas confondus.

Pensez-y ainsi. **Le RGPD régit les données personnelles qui traversent un système d'IA. L'AI Act régit le système d'IA lui-même — son niveau de risque, ses obligations, et comment il peut être utilisé.** Si votre système d'IA utilise des données personnelles, les deux s'appliquent en même temps. Ce ne sont pas des alternatives ; ils se cumulent.

Pour un système d'IA à haut risque qui traite des données personnelles, vous finissez par faire deux travaux liés. Sous l'AI Act, vous suivez un processus de risque et de conformité pour le système. Sous le RGPD, vous avez besoin d'une base légale pour les données personnelles et, là où le risque est élevé, d'une analyse d'impact relative à la protection des données. La bonne nouvelle est que le travail se recoupe : comprendre vos données, documenter votre processus et évaluer les risques servent les deux lois.

L'AI Act insiste aussi sur la qualité des données pour les systèmes à haut risque — les données d'entraînement et de test doivent être pertinentes et représentatives, et exemptes d'erreurs dans la mesure du possible. Cela rejoint le principe d'exactitude du RGPD. Et les devoirs de transparence de l'AI Act — dire aux gens qu'ils interagissent avec une IA — s'ajoutent aux devoirs de transparence du RGPD.

Le point pratique : ne traitez pas l'AI Act et le RGPD comme une seule liste de contrôle. Posez deux questions sur chaque système d'IA. *Quel est le niveau de risque du système sous l'AI Act ?* Et *quelles données personnelles le traversent, et cela est-il licite sous le RGPD ?* La première est le travail du Chapitre 5 ; la seconde est celui de ce chapitre.

### 10.7 L'analyse d'impact relative à la protection des données (AIPD) : quand elle est obligatoire et comment la faire

Une analyse d'impact relative à la protection des données est un examen structuré que vous faites **avant** de démarrer une activité de traitement susceptible d'être à haut risque pour les personnes. Pour l'IA, vous en aurez souvent besoin.

Vous devez faire une AIPD quand le traitement est à haut risque. Des déclencheurs clairs incluent : une évaluation systématique et approfondie des personnes fondée sur un traitement automatisé produisant des effets significatifs (cela couvre l'IA qui note, classe ou profile des personnes) ; un traitement à grande échelle de données sensibles ; et une surveillance systématique à grande échelle de zones accessibles au public. Les nouvelles technologies utilisées de façons nouvelles augmentent aussi le risque.

Comment en faire une, en étapes simples :

1. **Décrivez le traitement.** Quelles données, quelle finalité, combien de temps, qui les voit, où elles sont stockées, et si un tiers ou une IA est impliqué.
2. **Vérifiez la nécessité et la proportionnalité.** Est-ce le moyen le moins intrusif d'atteindre votre objectif ?
3. **Évaluez les risques pour les personnes.** Pas le risque pour votre entreprise — le risque pour leur vie privée, leur équité et leurs droits. Pensez aux biais, aux erreurs, à la surcollecte et à la réidentification.
4. **Listez les mesures pour réduire ces risques.** Minimisez les données, anonymisez où possible, ajoutez une revue humaine, sécurisez le système, fixez une courte conservation.
5. **Décidez.** Si un risque élevé subsiste après vos mesures, vous devez consulter votre autorité nationale de protection des données avant de procéder.
6. **Documentez et revoyez.** Écrivez-le et révisez-le quand le système change.

Une AIPD n'est pas un formulaire à cocher. C'est un exercice de réflexion qui, fait honnêtement, change souvent votre conception pour le mieux.

### 10.8 Anonymisation et pseudonymisation : ce que c'est et pourquoi c'est important

Ces deux mots se ressemblent et sont très différents. Les confondre cause de vrais problèmes.

**La pseudonymisation** signifie que vous remplacez les identifiants directs par un substitut, comme un code, et gardez séparée et en sécurité la clé qui relie le code à la personne. « Client 4471 » au lieu de « Maria Rossi », avec le tableau de correspondance sous clé. Une donnée pseudonymisée est **toujours une donnée personnelle** sous le RGPD, car avec la clé vous pouvez réidentifier la personne. C'est une mesure de sécurité précieuse — elle réduit le risque si les données sont volées — mais elle ne vous sort pas de la loi.

**L'anonymisation** signifie que vous retirez les informations identifiantes si complètement que personne ne peut réidentifier une personne, même en combinant les données avec d'autres sources. La loi demande si la réidentification est « raisonnablement probable », en tenant compte du coût, du temps et de la technologie actuelle. Une donnée vraiment anonyme est **hors du RGPD**, car il n'y a pas de personne identifiable. Mais la vraie anonymité est réellement difficile. Des jeux de données qui semblaient anonymes ont été réidentifiés en croisant d'autres données publiques.

Pourquoi c'est important pour l'IA : si vous voulez entraîner un modèle sur des données sans que le RGPD s'applique, vous avez besoin d'une vraie anonymité, pas d'une pseudonymisation. Et comme l'avertit l'avis du CEPD, même un modèle entraîné peut ne pas être anonyme si des données personnelles peuvent en être extraites par des questions astucieuses. Donc « nous avons anonymisé les données d'entraînement » est une affirmation que vous devez pouvoir défendre, pas juste asséner.

La règle de travail sûre : traitez les données pseudonymisées comme des données personnelles, parce que c'en est. Ne traitez des données comme anonymes que si vous avez testé que la réidentification n'est pas raisonnablement possible. Dans le doute, gardez les protections du RGPD actives.

## Éthique et responsabilité

Le RGPD est le plancher, pas le plafond. La conformité signifie que vous évitez les amendes ; l'éthique signifie que vous faites ce qu'il faut même là où la loi se tait.

**Respectez la personne derrière la donnée.** Chaque dossier est la vie privée de quelqu'un. Demandez-vous si votre usage vous semblerait juste si c'était vous qui étiez profilé par une IA.

**Ne vous cachez pas derrière « le modèle l'a fait ».** Si une IA prend une décision injuste sur une personne en utilisant vos données, vous êtes responsable. Gardez un humain qui assume le résultat, comme l'expose le [Chapitre 4](ch04-ethical-ai-doing-the-right-thing.md).

**Soyez transparent sur l'IA.** Dites aux gens quand une IA touche leurs données et ce qu'elle fait. Les surprises érodent la confiance plus vite que n'importe quel défaut technique.

**Minimisez comme habitude morale.** Collecter moins n'est pas juste une règle légale ; c'est du respect. Chaque champ que vous ne collectez pas est un champ qui ne peut pas être fui ou mal utilisé.

**Protégez les vulnérables.** Les données sensibles sur la santé, les croyances ou les finances méritent le plus grand soin. Si un outil ne peut pas le garantir, ne les mettez pas dans l'outil.

## Erreurs à éviter

1. **« Nous sommes trop petits pour le RGPD. »** La taille ne vous exempte pas. Si vous traitez des données personnelles de personnes dans l'UE, les règles s'appliquent.
2. **Penser que le consentement est toujours nécessaire, ou jamais nécessaire.** C'est une base parmi six. Utilisez la bonne et documentez pourquoi.
3. **Confondre pseudonymisation et anonymat.** Une donnée pseudonymisée est toujours une donnée personnelle et toujours dans le champ.
4. **Déverser toute votre base de données dans un outil d'IA.** Cela viole la minimisation des données et répand le risque.
5. **Pas de base légale pour s'entraîner sur des données personnelles.** « Améliorer nos services » ne suffit généralement pas.
6. **Ignorer les données sensibles cachées dans les CV et les tickets.** La santé, les croyances et l'activité syndicale peuvent être dans des documents ordinaires.
7. **Pas d'AIPD avant un déploiement d'IA à haut risque.** Faites-la avant, pas après une plainte.
8. **Pas de processus pour les demandes d'accès et de suppression.** Si vous ne pouvez pas trouver et supprimer les données, vous ne pouvez pas honorer le droit.
9. **Perdre le contrôle des données au profit d'un tiers.** Si le fournisseur ne peut pas vous aider à supprimer ou exporter, vous êtes exposé. Voir le [Chapitre 9](ch09-third-party-services-and-shadow-ai.md).
10. **Traiter la loi comme un projet ponctuel.** Le RGPD est continu. La conservation, les violations et les demandes continuent d'arriver.

## Exercice pratique

### 10.10 Votre liste de contrôle de conformité RGPD pour l'IA

Prenez une demi-journée et travaillez ceci pour un cas d'usage de l'IA qui touche des données personnelles.

1. **Cartographiez les données.** Listez exactement quelles données personnelles entrent dans l'IA. Nommez chaque champ. Marquez toute catégorie sensible. (Un modèle d'inventaire de données est en annexes.)
2. **Nommez la base légale.** Pour chaque usage, écrivez laquelle des six bases s'applique et pourquoi. Si vous ne pouvez en nommer aucune, arrêtez-vous et reconsidérez.
3. **Cherchez les données sensibles.** Si une donnée d'une catégorie particulière est présente, confirmez qu'une condition spécifique l'autorise, ou retirez-la.
4. **Appliquez la minimisation.** Coupez chaque champ dont vous n'avez pas strictement besoin.
5. **Décidez la destination.** Les données vont-elles à un tiers ? Si oui, passez les questions fournisseur du [Chapitre 9](ch09-third-party-services-and-shadow-ai.md).
6. **Faites une AIPD.** Si l'usage est à haut risque — profilage, données sensibles à grande échelle, décisions automatisées — complétez les étapes d'AIPD de la section 10.7.
7. **Planifiez les droits.** Écrivez comment vous traiterez les demandes d'accès, de correction et de suppression pour ces données, y compris les données détenues par le fournisseur.
8. **Fixez la conservation.** Décidez combien de temps vous gardez les données et quand vous les supprimez.
9. **Vérifiez les règles sur les décisions automatisées.** Si l'IA décide sur des personnes avec un effet significatif, assurez-vous qu'un chemin de revue humaine existe.
10. **Documentez tout.** Écrivez les réponses. La responsabilité signifie que vous pouvez montrer votre travail.

Si une étape laisse un blanc que vous ne pouvez pas remplir, ce blanc est votre liste de choses à faire.

## Liste de contrôle

### 10.11 Les documents que vous devez avoir

Pour un système d'IA qui touche des données personnelles, gardez ces documents prêts et à jour.

- [ ] **Avis de confidentialité** qui explique clairement quelles données vous collectez, pourquoi, et comment l'IA est impliquée.
- [ ] **Registre des activités de traitement** décrivant chaque usage de données personnelles.
- [ ] **Déclaration de base légale** pour chaque finalité de traitement, écrite.
- [ ] **Inventaire des données** listant chaque champ de données personnelles et où il se trouve.
- [ ] **AIPD** pour tout traitement d'IA à haut risque, avec la décision sur le risque résiduel.
- [ ] **Test de mise en balance** si vous vous appuyez sur l'intérêt légitime.
- [ ] **Accord de traitement des données** avec chaque fournisseur qui manipule vos données.
- [ ] **Calendrier de conservation** indiquant combien de temps chaque type de donnée est gardé et quand il est supprimé.
- [ ] **Procédure de demande des personnes** pour l'accès, la rectification, l'effacement et la portabilité, avec une horloge d'un mois.
- [ ] **Plan de réponse aux violations** incluant la notification à l'autorité sous 72 heures et aux personnes affectées quand requis.
- [ ] **Garde-fous sur les décisions automatisées** avec un chemin de revue humaine pour les décisions significatives.
- [ ] **Coordonnées du délégué à la protection des données**, si votre traitement en exige un.

Gardez-les vivants. Un document que vous ne mettez jamais à jour est un document qui vous laissera tomber quand un régulateur ou un client demandera.

## Points à retenir

- Le RGPD s'applique à toute donnée personnelle sur des personnes identifiables dans l'UE, y compris quand elle traverse un outil d'IA, et il atteint les entreprises hors de l'UE qui servent des clients européens.
- Vous avez besoin d'une base légale pour chaque usage ; le consentement n'est qu'une base sur six, et les données sensibles exigent une condition spécifique en plus.
- Les personnes détiennent de vrais droits — accès, correction, effacement, portabilité — et vous devez pouvoir les honorer, y compris pour les données détenues par un fournisseur tiers.
- La pseudonymisation n'est pas l'anonymat ; seules les données qui ne peuvent pas raisonnablement être réidentifiées sortent du RGPD, et un modèle qui laisse fuiter des données personnelles n'est pas anonyme.
- Pour une IA à haut risque, faites une AIPD avant de commencer, et rappelez-vous que l'AI Act et le RGPD s'appliquent ensemble, et pas l'un à la place de l'autre.
