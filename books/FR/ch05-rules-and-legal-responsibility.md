# Chapitre 5 — Règles et responsabilité juridique : le Règlement européen sur l'IA

## En mots simples

Chaque nouvel outil apporte ses règles. Les voitures ont apporté le code de la route. Les banques ont apporté des règles sur la manipulation de l'argent. L'IA est en train d'avoir son propre règlement, et si vous faites des affaires en Europe ou avec l'Europe, ce règlement est le **Règlement européen sur l'IA** (l'« AI Act »).

Ce chapitre est le guide en langage clair de ce règlement. Aucune formation juridique n'est nécessaire. Le but est simple : vous devez être capable de dire si un outil que vous voulez utiliser est faiblement réglementé, fortement réglementé, ou carrément interdit, et ce que vous devez faire en conséquence.

Deux idées expliquent l'essentiel de la loi.

La première est le **risque**. Le Règlement sur l'IA ne traite pas toutes les IA de la même façon. Il classe les systèmes d'IA par niveaux selon le tort qu'ils pourraient causer. Un filtre anti-spam est à peine touché. Un système qui décide qui obtient un prêt ou un emploi est surveillé de près. Quelques pratiques sont tout simplement interdites. Plus le risque est élevé, plus vous devez en faire.

La seconde est **votre rôle**. La loi sépare le **fournisseur** (qui construit ou met sa marque sur un système d'IA et le met sur le marché) du **déployeur** (qui l'utilise). La plupart des petites et moyennes entreprises sont des déployeurs. Vos devoirs diffèrent de ceux du vendeur, mais ils existent, et ils sont les vôtres.

Une note sur la portée. Le Règlement européen sur l'IA est une loi européenne. Si vous êtes hors de l'UE mais que votre IA a un effet sur des personnes dans l'UE, certaines parties peuvent quand même vous atteindre. Vérifiez auprès d'un professionnel si vous servez des clients européens.

### 5.1 Le RGPD en mots simples : ce que vous devez savoir

Le **RGPD** (le Règlement général sur la protection des données) est la loi européenne sur les données personnelles. Il s'applique depuis 2018 et il régit encore tout ce que vous faites avec des informations sur des personnes identifiées — y compris les données que vous donnez à une IA.

En un paragraphe : si vous collectez, stockez ou traitez des données personnelles de personnes dans l'UE, vous avez besoin d'un motif licite pour le faire, vous devez dire aux gens à quoi servent leurs données, les garder en sécurité, ne conserver que ce dont vous avez besoin, permettre aux gens d'y accéder ou de les supprimer sur demande, et ne pas les garder plus longtemps que nécessaire. Les violations peuvent entraîner de grosses amendes. L'IA ne change pas ces devoirs ; elle vous donne juste plus de façons de les enfreindre, parce que les modèles ont besoin de données et que ces données sont personnelles. Le traitement complet et détaillé du RGPD — les bases licites, les droits des personnes concernées et comment s'y conformer — est le domaine du [Chapitre 10 — Vie privée et RGPD](ch10-privacy-and-gdpr.md). Lisez ce chapitre avant de traiter des données clients avec une IA. L'idée ici est seulement que le Règlement sur l'IA et le RGPD s'appliquent ensemble, l'un par-dessus l'autre, et pas l'un à la place de l'autre.

### 5.2 Données personnelles et données sensibles : la différence qui compte

Le RGPD trace une ligne qui compte beaucoup pour l'IA, parce que la catégorie supérieure impose des règles plus strictes.

Une **donnée personnelle** est toute information sur une personne vivante qui peut être identifiée, directement ou indirectement. Un nom, un email, un numéro de téléphone, une localisation, un identifiant en ligne. Même une combinaison de faits ordinaires qui pointe vers une seule personne compte.

Une **donnée sensible** (la loi parle de « catégories particulières ») est un ensemble plus restreint de faits plus délicats : origine raciale ou ethnique, opinions politiques, convictions religieuses ou philosophiques, appartenance syndicale, données génétiques, données biométriques utilisées pour identifier quelqu'un, données de santé, et données sur la vie sexuelle ou l'orientation sexuelle d'une personne.

Pourquoi cette ligne compte pour vous : traiter des données sensibles exige un fondement juridique plus solide et plus de protection. C'est aussi les données les plus susceptibles de causer de la discrimination si elles façonnent une décision d'IA. Beaucoup des règles les plus strictes du Règlement sur l'IA existent parce que l'IA peut transformer des données ordinaires en déductions sensibles, ou utiliser des données sensibles pour trier les gens. Pour les définitions et les règles de manipulation complètes, voir le [Chapitre 10 — Vie privée et RGPD](ch10-privacy-and-gdpr.md).

## Un peu d'histoire

L'Europe a écrit son règlement sur la vie privée en premier et son règlement sur l'IA en second, et cet ordre explique les deux.

Le **RGPD** a été adopté en 2016 et est devenu directement applicable en mai 2018. C'était la loi sur la protection des données la plus complète de son époque, et comme tant d'entreprises mondiales traitent avec des Européens, elle a fixé une norme mondiale. Son idée centrale — les gens sont propriétaires de leurs données personnelles et vous avez besoin d'un motif licite pour les utiliser — est devenue le modèle des lois sur la vie privée ailleurs.

Pour l'IA, l'Europe a pris une voie fondée sur les principes. En 2018, la Commission européenne a créé un Groupe d'expert de haut niveau sur l'IA, qui a publié en 2019 des lignes directrices éthiques volontaires construites autour de l'« IA de confiance ». La Commission a ensuite transformé les principes en loi, en proposant le Règlement sur l'IA en avril 2021. Après des années de négociation, il a été publié au Journal officiel de l'Union européenne le **12 juillet 2024** et est entré en vigueur le **1er août 2024**. C'est la première loi complète et horizontale au monde sur l'intelligence artificielle — « horizontale » voulant dire qu'elle couvre l'IA dans tous les secteurs, et pas un secteur à la fois.

La loi ne démarre pas d'un coup. Elle s'allume par étapes, pour donner aux entreprises le temps de se préparer. Ce calendrier par étapes est la chose la plus pratique de ce chapitre, et il apparaît dans la section 5.3. L'histoire montre la direction : des lignes directrices éthiques souples à des obligations fermes et datées. Le débat est clos. L'horloge tourne.

## Curiosité

### La première loi sur l'IA au monde — et des amendes qui dépassent le RGPD

Voici un fait bon à connaître avant toute conversation sur « la conformité coûte trop cher ».

Le Règlement européen sur l'IA est la première loi complète sur l'IA où que ce soit. Aucune autre grande économie n'en a une qui égale son ampleur. Cela en fait un cas d'école, et cela lui donne aussi une sorte de poids : les entreprises du monde entier se construisent souvent selon la règle la plus stricte à laquelle elles pourraient faire face, si bien qu'une règle européenne peut discrètement devenir un défaut mondial. On appelle cela l'« effet Bruxelles ».

L'autre fait frappant est la taille des sanctions. L'amende maximale du RGPD va jusqu'à 4 % du chiffre d'affaires annuel mondial total d'une entreprise. Le Règlement sur l'IA va plus haut pour les pires violations. Pour les pratiques interdites de la section 5.5, les amendes peuvent atteindre **jusqu'à 35 millions d'euros ou 7 % du chiffre d'affaires annuel mondial total, le montant le plus élevé étant retenu.** Pour la plupart des autres manquements au Règlement, le plafond est d'environ 15 millions d'euros ou 3 %. Pour avoir fourni des informations inexactes aux autorités, environ 7,5 millions d'euros ou 1 %. (Pour les petites et moyennes entreprises, la loi plafonne les amendes au plus bas des deux chiffres, donc la charge est réduite — mais elle reste réelle.)

La leçon est sans détour. La pratique que la loi craint le plus — les usages interdits — porte l'amende la plus lourde de la réglementation numérique européenne, plus lourde que le RGPD. Cela vous dit exactement où se trouve la ligne, et cela vous dit que « nous ne savions pas » n'est pas une excuse bon marché.

## Un exemple d'entreprise réel

### Un petit prêteur qui évalue le crédit avec une IA

Cet exemple est illustratif. C'est un scénario réaliste, pas le résultat rapporté d'une entreprise, construit pour montrer comment les niveaux fonctionnent en pratique.

Imaginez une petite société de crédit à la consommation qui veut utiliser un modèle d'IA pour décider d'approuver ou non un prêt personnel.

La première étape est de trouver le niveau. Le Règlement sur l'IA énumère dans une annexe les catégories d'IA à haut risque. Une catégorie couvre les **services privés et publics essentiels**, et elle inclut explicitement l'**évaluation de la solvabilité** — décider si une personne obtient du crédit. Donc ce modèle de prêt est **à haut risque**. Il n'est pas interdit, mais il se trouve dans le niveau de travail le plus fortement réglementé.

Ce que cela signifie pour la société, en termes simples :

- Elle doit mettre en place un **système de gestion des risques** sur toute la durée de vie du modèle, pas seulement une fois.
- Elle doit gouverner ses **données** : les données utilisées pour entraîner et tester le modèle doivent être pertinentes, représentatives et aussi exemptes d'erreurs que possible pour l'usage visé. Un modèle entraîné surtout sur un type d'emprunteur traitera les autres injustement.
- Elle doit conserver une **documentation technique** et des **journaux automatiques** du fonctionnement du système.
- Elle doit prévoir une **supervision humaine** : une personne doit pouvoir examiner et annuler une décision.
- Elle doit garantir l'**exactitude, la robustesse et la cybersécurité**.
- Avant de le mettre sur le marché pour usage, elle doit mener une **évaluation de conformité**, rédiger une **déclaration UE de conformité**, apposer un **marquage CE** et **enregistrer le système dans la base de données UE** pour l'IA à haut risque.

Changez maintenant un détail et le niveau change. Supposons que la société utilise plutôt l'IA uniquement pour rédiger des emails de rappel amicaux sur des prêts existants, sans aucune décision d'approbation. Ce n'est pas une fonction à haut risque. Cela tombe dans un niveau léger, où le principal devoir est la transparence : les gens doivent savoir que des moyens automatisés sont impliqués là où c'est requis.

Même entreprise, même vendeur de technologie, deux charges juridiques très différentes — parce que c'est l'*usage* qui détermine le niveau, pas l'outil. C'est toute la logique du Règlement résumée en une scène.

## Comment faire

### 5.3 Le Règlement européen sur l'IA : ce qui change pour les entreprises

Le Règlement classe l'IA en quatre niveaux de risque, plus une filière séparée pour les grands modèles à usage général qui sont derrière les chatbots.

**Niveau 1 — Inacceptable (interdit).** Un petit ensemble de pratiques est banni purement et simplement. Voir la section 5.5. Si votre usage tombe ici, vous ne pouvez pas du tout le faire.

**Niveau 2 — Haut risque.** Systèmes qui peuvent porter un tort grave à la santé, à la sécurité ou aux droits fondamentaux. Ils portent le régime de conformité complet : gestion des risques, gouvernance des données, documentation, journaux, transparence envers les utilisateurs, supervision humaine, exactitude et sécurité, évaluation de conformité, marquage CE et enregistrement. Les usages à haut risque sont listés dans deux annexes : l'annexe I (l'IA comme composant de sécurité dans des produits réglementés) et l'annexe III (usages sensibles listés).

**Niveau 3 — Risque limité / de transparence.** Systèmes qui ne sont pas à haut risque mais qui interagissent avec des gens ou génèrent du contenu. Le principal devoir est la divulgation : dire aux gens qu'ils ont affaire à une IA, et étiqueter le contenu synthétique. Voir la section 5.6.

**Niveau 4 — Risque minimal.** Tout le reste — filtres anti-spam, prévision de stock, la plupart des outils de productivité internes. Aucune nouvelle obligation au-delà de la loi existante.

Les **catégories à haut risque de l'annexe III** sont celles qu'un dirigeant d'entreprise a le plus de chances de rencontrer. Elles comprennent : la biométrie (là où elle n'est pas interdite) ; les composants de sécurité des infrastructures critiques ; l'éducation et la formation (admissions, évaluation des apprentissages) ; **l'emploi et la gestion des travailleurs** (recrutement, filtrage des candidatures, promotion, licenciement, attribution des tâches, surveillance de la performance) ; les **services essentiels** (admissibilité aux prestations, solvabilité, tri des appels d'urgence, risque et tarification en assurance) ; le maintien de l'ordre ; la migration et le contrôle aux frontières ; et l'administration de la justice et les processus démocratiques.

Une exception utile : un système de l'annexe III n'est **pas** à haut risque s'il ne fait qu'une tâche procédurale étroite, améliore quelque chose qu'un humain a déjà fait, détecte des motifs sans remplacer l'évaluation humaine, ou fait une pure étape préparatoire. Mais il est **toujours à haut risque s'il dresse le profil d'une personne.** Le profilage signifie utiliser des données pour évaluer ou prédire des aspects sur un individu.

**Votre rôle décide vos devoirs.** Un fournisseur porte les lourdes obligations de construction. Un déployeur (la plupart des entreprises) porte des devoirs d'usage : utiliser le système comme indiqué, assurer la supervision humaine, surveiller, conserver certains journaux, et dans certains cas mener une vérification des droits fondamentaux. Si vous *utilisez* seulement un outil à haut risque d'un vendeur, vous ne faites pas l'évaluation de conformité — le fournisseur la fait — mais vous devez quand même le déployer correctement et de façon responsable.

**Le calendrier par étapes.** Mémorisez ces dates si vous touchez à l'IA en Europe :

| Date | Ce qui s'applique |
|---|---|
| 1er août 2024 | Entrée en vigueur du Règlement |
| 2 février 2025 | Pratiques interdites (art. 5) et devoir de maîtrise de l'IA (art. 4) s'appliquent |
| 2 août 2025 | Règles pour les modèles d'IA à usage général, organes de gouvernance et cadre de sanctions |
| 2 août 2026 | Obligations haut risque pour les usages de l'annexe III (emploi, crédit, éducation, services essentiels, etc.) |
| 2 août 2027 | Obligations haut risque pour les produits de l'annexe I (composants de sécurité IA dans des produits réglementés) |

L'UE a proposé depuis quelques simplifications, parfois appelées un « omnibus numérique », et les dates ou détails peuvent bouger. Traitez le tableau comme la base de travail et confirmez les dates actuelles contre le texte officiel avant de vous fier à une échéance.

### 5.4 Obligations pour les systèmes à haut risque : évaluation de conformité et documentation technique

Si votre usage est à haut risque, voici les choses concrètes requises. Vous n'avez pas besoin de toutes les réaliser vous-même en tant que déployeur, mais vous devez les comprendre pour choisir un vendeur et déployer correctement.

**Gestion des risques.** Un processus continu, sur toute la durée de vie du système, qui trouve, évalue et réduit les risques pour la santé, la sécurité et les droits fondamentaux. Pas un formulaire ponctuel.

**Gouvernance des données.** Les données d'entraînement, de validation et de test doivent être pertinentes, représentatives et aussi exemptes d'erreurs et complètes que le but le permet. C'est là que le biais est attrapé ou manqué.

**Documentation technique.** Un écrit montrant que le système est conforme et permettant aux autorités de le vérifier. Elle couvre comment le système fonctionne, sur quoi il a été entraîné, comment il a été testé, et comment l'utiliser. Conservez-la, avec les décisions d'évaluation et les changements approuvés.

**Conservation des journaux (logging).** Le système doit enregistrer automatiquement les événements pertinents pour les risques et pour les changements, afin que son comportement puisse être revu plus tard. Les journaux sont vos preuves.

**Transparence envers les déployeurs.** Des instructions d'utilisation claires pour que les gens qui exploitent le système puissent se conformer à leurs propres devoirs.

**Supervision humaine.** Le système doit être conçu pour qu'un humain puisse le comprendre, le surveiller, interpréter sa sortie, et intervenir ou l'arrêter.

**Exactitude, robustesse, cybersécurité.** Le système doit atteindre des niveaux appropriés des trois et résister à l'erreur et à l'attaque.

**Gestion de la qualité et accessibilité.** Un système pour maintenir la conformité dans le temps, et les exigences d'accessibilité satisfaites.

**Évaluation de conformité, marquage CE, enregistrement.** Avant qu'un système à haut risque ne soit mis sur le marché, le fournisseur mène une **évaluation de conformité** (une vérification indépendante par un « organisme notifié » là où la loi l'exige). En cas de réussite, le fournisseur rédige une **déclaration UE de conformité**, appose un **marquage CE** et **enregistre le système dans la base de données UE**. En tant que déployeur, vous devriez demander à voir ces éléments avant d'acheter. Si un vendeur ne peut pas montrer de parcours de conformité pour un usage à haut risque, c'est un grave signal d'alerte.

### 5.5 Pratiques interdites : ce que vous ne pouvez absolument pas faire avec l'IA

Celles-ci sont interdites dans toute l'UE depuis le 2 février 2025. Si un cas d'usage correspond, abandonnez-le. Les amendes ici sont les plus lourdes de la loi.

1. **Techniques subliminales ou manipulatrices** qui dépassent la conscience d'une personne et faussent sensiblement son comportement d'une façon qui cause, ou est susceptible de causer, un tort important.
2. **Exploiter des vulnérabilités** de personnes à cause de l'âge, d'un handicap, ou d'une situation sociale ou économique, pour fausser leur comportement et causer un tort important.
3. **Notation sociale** par des autorités publiques — noter systématiquement les gens sur leur comportement social ou leurs traits personnels de façons qui mènent à un traitement nuisible sans rapport avec le contexte, ou disproportionné par rapport au comportement.
4. **Collecte sans cible d'images faciales** sur internet ou la vidéosurveillance pour construire des bases de données de reconnaissance faciale.
5. **Reconnaissance d'émotions sur le lieu de travail et dans l'éducation** — déduire les émotions de travailleurs ou d'élèves, sauf pour des raisons médicales ou de sécurité. (Un outil qui « lit » l'humeur d'un agent de centre d'appels pour le noter tombe en plein dans cette interdiction.)
6. **Catégorisation biométrique qui déduit des attributs sensibles** — utiliser des données biométriques pour deviner la race, les opinions politiques, l'appartenance syndicale, les convictions religieuses ou philosophiques, la vie sexuelle ou l'orientation sexuelle.
7. **Identification biométrique à distance en temps réel dans les espaces publics pour le maintien de l'ordre**, interdite sauf pour quelques situations étroites et autorisées telles que rechercher des personnes disparues ou empêcher une menace grave imminente et spécifique.

La plupart des petites entreprises ne toucheront jamais à celles-ci. Mais deux prennent les gens par surprise : **la reconnaissance d'émotions au travail** et **le design manipulateur qui exploite une vulnérabilité**. Si un vendeur vous pitch une « IA qui détecte les émotions des clients ou des employés », sachez que dans un cadre de travail ou scolaire c'est interdit.

### 5.6 Obligations de transparence : quand vous devez informer clients et employés

Pour les systèmes qui ne sont pas à haut risque mais qui interagissent avec des gens ou créent du contenu, le principal devoir est d'être ouvert. Ces règles de transparence s'appliquent à partir du 2 août 2026.

**Dites aux gens qu'ils parlent à une IA.** Si un système d'IA interagit directement avec une personne — un chatbot, par exemple — cette personne doit être informée qu'elle a affaire à une IA, sauf si c'est évident. Un bot de service client devrait le dire.

**Étiquetez le contenu synthétique et les deepfakes.** L'audio, les images, la vidéo ou le texte générés ou manipulés par IA doivent être marqués comme générés ou manipulés artificiellement. Cela vise les deepfakes et les médias faits par machine.

**Divulguez la reconnaissance d'émotions et la catégorisation biométrique.** Là où de tels systèmes sont utilisés légalement (hors des cas interdits du travail et de l'éducation), les personnes exposées doivent être informées.

Une petite note de tolérance : les systèmes déjà mis sur le marché avant le 2 août 2026 ont une courte fenêtre jusqu'à fin 2026 pour satisfaire la règle d'étiquetage du contenu synthétique. Prévoyez de vous conformer de toute façon.

Pour une entreprise, le geste pratique est simple et bon marché : mettez un avis clair dans votre chatbot (« Vous discutez avec un assistant automatisé »), étiquetez tout média généré par IA que vous publiez, et ne faites jamais d'analyse cachée des émotions ou biométrique sur les gens.

### 5.7 Documenter les décisions importantes

À travers chaque niveau, une habitude vous protège : **écrivez vos décisions et votre raisonnement.**

Une bonne documentation n'est pas de la bureaucratie. C'est votre mémoire et votre défense. Quand un régulateur, un client ou un tribunal demande pourquoi vous avez utilisé un système d'une certaine façon, l'écrit est votre réponse.

Pour chaque système d'IA, gardez un simple dossier qui enregistre :

- **Ce qu'il fait et qui le possède.** Le cas d'usage, le niveau où vous l'avez classé, et le responsable nommé.
- **Pourquoi vous l'avez choisi.** La raison métier et les alternatives que vous avez envisagées.
- **Comment vous avez évalué le risque.** La revue éthique et juridique du risque, y compris toute vérification de biais et toute vérification des droits fondamentaux.
- **Quels contrôles vous avez mis en place.** Supervision humaine, journaux, avis de transparence, limites de données.
- **Ce que vous avez testé et quand.** Résultats des tests, dates, et qui les a revus.
- **Les changements dans le temps.** Toute modification du système ou de son usage, avec la raison et la date.
- **Incidents et corrections.** Tout ce qui a mal tourné et ce que vous avez fait à ce sujet.

Ce dossier se connecte directement au travail d'éthique du [Chapitre 4 — IA éthique : faire ce qui est juste](ch04-ethical-ai-doing-the-right-thing.md). L'évaluation des risques que vous faites là devient une partie de votre dossier juridique ici. Un seul document, deux objectifs.

Une règle pratique : **si c'était important et que vous ne l'avez pas écrit, préparez-vous à ce que ce soit remis en question et à ce que vous n'ayez pas de réponse.**

## Éthique et responsabilité

La conformité est le plancher, pas le plafond. Respecter la lettre du Règlement sur l'IA ne rend pas un usage éthique, et cela n'enlève pas votre responsabilité. La loi vous dit ce que vous ne devez pas faire et ce que les usages à haut risque exigent. Elle ne vous dit pas si un usage est juste ou avisé. C'est votre jugement, traité au [Chapitre 4 — IA éthique : faire ce qui est juste](ch04-ethical-ai-doing-the-right-thing.md). Un système peut être entièrement conforme et quand même nuire à la confiance si vous le déployez négligemment.

Votre rôle façonne votre devoir. En tant que **déployeur**, vous êtes responsable d'utiliser un système comme indiqué, de garder un humain aux commandes là où c'est requis, de surveiller comment il se comporte, et d'être honnête avec les gens qu'il touche. Vous ne pouvez pas pointer le vendeur du doigt et passer votre chemin. Une posture pratique : **traitez chaque exigence légale comme le minimum, et laissez votre propre éthique fixer la norme au-dessus.** Quand vous pouvez montrer que vous avez fait plus que le minimum, vous gagnez en crédibilité — et pour une petite entreprise, la crédibilité vaut plus que n'importe quelle automatisation isolée.

## Erreurs à éviter

**Erreur 1 : Présumer que votre outil est « juste un chatbot » et non réglementé.** Le niveau dépend de ce qu'il décide, pas de ce qu'on l'appelle. Un chatbot qui influence le crédit ou le recrutement est à haut risque.

**Erreur 2 : Ne pas connaître son rôle.** Fournisseur et déployeur ont des devoirs différents. Si vous utilisez seulement un outil à haut risque d'un vendeur, vous avez quand même des devoirs de déployeur. Sachez lequel vous êtes.

**Erreur 3 : Rater les dates par étapes.** Les interdictions et le devoir de maîtrise de l'IA sont déjà en vigueur (février 2025). Les devoirs haut risque arrivent en 2026 et 2027. Ne traitez pas toute la loi comme « plus tard ».

**Erreur 4 : Acheter un outil à haut risque sans parcours de conformité.** Si un vendeur ne peut pas montrer une évaluation de conformité, une déclaration de conformité et un enregistrement pour un usage à haut risque, ne l'achetez pas.

**Erreur 5 : Faire de la reconnaissance d'émotions au travail.** C'est interdit sur les lieux de travail et dans les écoles. Un pitch de vendeur pour une « détection d'humeur » sur le personnel est un piège.

**Erreur 6 : Oublier le devoir de maîtrise de l'IA.** L'article 4 est la loi maintenant. Vous devez prendre des mesures raisonnables pour former les gens qui utilisent votre IA.

**Erreur 7 : Confondre le RGPD et le Règlement sur l'IA.** Ce sont des lois séparées qui s'empilent. Se conformer à l'une ne couvre pas l'autre. Lisez le [Chapitre 10 — Vie privée et RGPD](ch10-privacy-and-gdpr.md) pour le volet vie privée.

**Erreur 8 : Ne pas documenter.** Pas d'écrit signifie pas de défense quand on vous demande d'expliquer une décision.

**Erreur 9 : Traiter la conformité comme la ligne d'arrivée.** La loi est le plancher. L'éthique et la confiance sont au-dessus, et vous les gardez quand même.

## Exercice pratique

### 5.8 Votre checklist de conformité

Prenez un système d'IA que vous utilisez ou prévoyez d'utiliser et classez-le. Cela prend environ une heure et vous dit quelles règles vous lient.

**Étape 1 — Est-ce interdit ?** Lisez les sept pratiques bannies de la section 5.5. Si votre usage en correspond à une, arrêtez. Ne poursuivez pas.

**Étape 2 — Est-ce à haut risque ?** Vérifiez les catégories de l'annexe III : biométrie, infrastructures critiques, éducation, **emploi et gestion des travailleurs**, **services essentiels (crédit, prestations, assurance)**, maintien de l'ordre, migration, justice. Votre usage en correspond-il à une ? Si oui, c'est à haut risque sauf si l'exception étroite s'applique — et c'est toujours à haut risque si cela dresse le profil d'une personne.

**Étape 3 — Est-ce un cas de transparence ?** Interagit-il avec des gens ou génère-t-il du contenu ? Si oui, vous devez divulguer l'usage de l'IA et étiqueter le contenu synthétique.

**Étape 4 — Minimal ?** Si rien de ce qui précède, vous êtes au niveau minimal. Pas de nouvelles obligations liées au Règlement, mais la loi existante et votre propre éthique s'appliquent toujours.

**Étape 5 — Quel est votre rôle ?** Fournisseur ou déployeur ? Écrivez-le. Listez les devoirs qui découlent de ce rôle.

**Étape 6 — Si à haut risque, rassemblez les preuves du vendeur.** Demandez l'évaluation de conformité, la déclaration UE de conformité, le marquage CE et l'enregistrement dans la base de données UE. Notez ce qui manque.

**Étape 7 — Cartographiez vos devoirs de déployeur.** Supervision humaine, surveillance, journaux, avis de transparence, et toute vérification des droits fondamentaux qui vous concerne.

**Étape 8 — Vérifiez le calendrier.** Lesquelles de vos obligations sont déjà en vigueur (maîtrise, interdictions) et lesquelles arrivent en 2026 ou 2027 ? Mettez des dates dessus.

**Étape 9 — Ouvrez le dossier.** Démarrez le dossier de documentation de la section 5.7 avec votre classification et votre plan.

Si vous ne pouvez pas placer un système dans un niveau avec assurance, c'est en soi le constat : faites appel à un expert avant de déployer.

## Checklist

### 5.9 Votre politique juridique pour l'IA

- [ ] Je connais les quatre niveaux de risque : interdit, haut risque, transparence, minimal.
- [ ] Je peux nommer les catégories à haut risque de l'annexe III, surtout l'emploi et les services essentiels (crédit, assurance).
- [ ] Je sais que dresser le profil d'une personne rend un usage de l'annexe III toujours à haut risque.
- [ ] Je connais les sept pratiques interdites et que la reconnaissance d'émotions au travail/à l'école en est une.
- [ ] Je connais mon rôle pour chaque système : fournisseur ou déployeur.
- [ ] Je connais les dates par étapes : interdictions et maîtrise de l'IA en vigueur depuis le 2 février 2025 ; haut risque annexe III en août 2026 ; produits annexe I en août 2027.
- [ ] Pour les outils à haut risque, j'exige l'évaluation de conformité du vendeur, la déclaration de conformité, le marquage CE et l'enregistrement dans la base de données UE.
- [ ] Je divulgue l'interaction IA aux clients et j'étiquette le contenu généré par IA.
- [ ] Je garde la supervision humaine et les journaux là où le niveau l'exige.
- [ ] J'ai un plan pour satisfaire le devoir de maîtrise de l'IA pour le personnel qui utilise nos systèmes.
- [ ] Je comprends que le RGPD s'applique par-dessus le Règlement sur l'IA, et j'ai lu le [Chapitre 10 — Vie privée et RGPD](ch10-privacy-and-gdpr.md).
- [ ] Je garde un dossier de documentation pour chaque système : usage, niveau, responsable, évaluation des risques, contrôles, tests, changements, incidents.
- [ ] Je traite la conformité comme le plancher et ma propre éthique comme la norme au-dessus.
- [ ] Je fais appel à un expert pour tout système que je ne peux pas classer avec assurance.

## Points clés à retenir

- Le Règlement européen sur l'IA classe l'IA par risque — interdit, haut risque, transparence, minimal — et plus le risque est élevé, plus vous devez en faire.
- L'emploi et les services essentiels comme le crédit et l'assurance sont à haut risque ; dresser le profil d'une personne rend toujours un usage de l'annexe III à haut risque.
- Sept pratiques sont bannies purement et simplement, y compris la reconnaissance d'émotions sur les lieux de travail et à l'école, et elles portent les amendes les plus lourdes du droit numérique européen.
- La loi s'est allumée par étapes : les interdictions et le devoir de maîtrise de l'IA sont déjà en vigueur, et les devoirs haut risque arrivent en 2026 et 2027.
- En tant que déployeur, vous portez quand même de vrais devoirs — supervision, transparence, maîtrise et documentation — et la conformité est le plancher, pas la fin de votre responsabilité.
