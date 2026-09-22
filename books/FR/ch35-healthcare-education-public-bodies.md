# Chapitre 35 — Santé, éducation et organismes publics

*Ce chapitre est une synthèse représentative. Ce n'est pas une seule organisation réelle. Il réunit les schémas courants que nous observons dans les petits cabinets médicaux, les écoles et les bureaux publics qui adoptent l'IA pour l'administration. Tous les chiffres sont illustratifs — ils montrent la forme de la décision, pas une promesse. Remplacez-les par les vôtres. Les règles applicables aux données réglementées sont exposées au [Chapitre 10 — Confidentialité et RGPD](ch10-privacy-and-gdpr.md) et au [Chapitre 5 — Règles et responsabilité juridique](ch05-rules-and-legal-responsibility.md) ; ce chapitre montre comment ces règles s'appliquent en pratique.*

## Le contexte

Imaginez un petit cabinet médical de quartier. Nous l'appellerons **Cabinet Familial Riverside**. Il compte quatre médecins généralistes, deux infirmières et un accueil avec trois employés administratifs. Il dessert quelques milliers de patients dans une ville.

La journée du cabinet tourne autour de l'accueil. Le téléphone sonne sans arrêt. Les gens appellent pour prendre rendez-vous, pour en déplacer un, pour demander quoi apporter, pour demander une ordonnance de référence, pour savoir quand un résultat est prêt. Les trois employés passent l'essentiel de leur journée au téléphone et sur papier. Les lettres d'orientation arrivent par la poste et il faut les lire, les classer et les transmettre au bon médecin. Les formulaires doivent être vérifiés avant qu'un patient soit reçu. Pendant ce temps, les médecins terminent chaque consultation puis passent du temps à rédiger les notes — une tâche qui s'accumule jusqu'à ce qu'une partie soit faite tard le soir.

Imaginez maintenant deux autres lieux de même forme. Une **école primaire** où le secrétariat répond chaque jour aux mêmes questions des parents, gère les papiers d'admission et jongle avec les emplois du temps. Un **bureau communal** où le personnel traite les demandes des citoyens — un permis, une demande d'allocation, une inscription — chacune étant une pile de formulaires et de documents qu'il faut lire, vérifier et faire avancer.

Trois lieux différents. Le même schéma : une petite équipe submergée par la planification, les documents et les questions répétées, pendant que les personnes formées — médecins, enseignants, assistants sociaux — passent leur temps sur la paperasse au lieu du travail pour lequel elles ont été formées.

Ce qui rend ces trois endroits spéciaux, ce sont les données. Un cabinet détient des **données de santé**. Une école détient des données sur des enfants. Un bureau public détient des données sur les citoyens et leurs droits. Ce ne sont pas des dossiers ordinaires. Ce sont parmi les catégories les plus protégées de données personnelles. Ce seul fait fixe une barre plus haute pour tout ce chapitre.

## Le problème

Les fuites sont les habituelles, mais le coût de l'erreur est plus élevé.

**Surcharge de l'accueil.** La file d'attente téléphonique est le goulot d'étranglement du cabinet. Le personnel passe des heures sur des questions répétées — horaires d'ouverture, quoi apporter, comment reporter — pendant que les vrais appels urgents attendent. Les longues attentes frustrent les patients et épuisent le personnel.

**Rendez-vous manqués.** Quand un patient oublie un rendez-vous, le créneau est perdu alors qu'un autre aurait pu l'avoir. Dans un cabinet occupé, un taux élevé d'absences signifie que les vrais patients attendent plus longtemps pour être soignés.

**Fardeau de documentation.** Après chaque consultation, le médecin rédige des notes. C'est nécessaire et c'est lourd. Partout, les cliniciens déclarent passer une grande part de leur journée sur les dossiers plutôt qu'auprès des patients. C'est un facteur connu de stress et d'épuisement. Le travail est méticuleux mais répétitif.

**Traitement des documents.** Les lettres d'orientation, les formulaires et les résultats arrivent dans de nombreux formats. Quelqu'un doit lire chacun, en extraire les faits essentiels, le classer et le transmettre à la bonne personne. Rater un document et un patient attend.

**Questions répétées des citoyens et des parents.** À l'école et au bureau communal, les mêmes questions reviennent sans cesse, dans plusieurs langues, et la réponse est toujours la même. Y répondre est simple, mais cela absorbe le bureau.

Par-dessus tout cela se trouve la règle selon laquelle ces données sont de **catégorie particulière**. Selon le RGPD, les données de santé et les données sur les enfants bénéficient d'une protection supplémentaire. La loi européenne sur l'IA en ajoute : les systèmes utilisés dans des dispositifs médicaux ou de façons qui affectent les droits des personnes sont considérés à plus haut risque et comportent des obligations plus lourdes. Les détails se trouvent au [Chapitre 10](ch10-privacy-and-gdpr.md) et au [Chapitre 5](ch05-rules-and-legal-responsibility.md). L'idée ici est simple : dans ces contextes, la confidentialité et la conformité ne sont pas une case à cocher à la fin. Elles façonnent chaque choix dès le départ.

## La solution

Riverside s'attaque à la charge administrative par ordre de sécurité. La règle est la même que dans un cabinet d'avocats : commencer là où une erreur coûte peu et où la donnée est le moins sensible, et avancer vers le travail sensible seulement quand les outils sont fiables. Et dans un cabinet, le travail le plus sensible — le jugement clinique — n'est jamais automatisé du tout.

**Prise de rendez-vous et rappels par IA.** Un chatbot sur le site et un standard téléphonique gèrent les réservations courantes : réserver, déplacer, annuler. Ils répondent instantanément aux questions répétées. Des rappels automatiques partent avant chaque rendez-vous, ce qui réduit les absences. Le personnel d'accueil est libéré pour les appels qui demandent un humain — un patient inquiet, un cas complexe. La technologie du chatbot est la même qu'au [Chapitre 27 — Service et support client](ch27-customer-care-and-support.md).

**Documentation ambiante qui rédige, le médecin signe.** Pour une consultation, un outil écoute la conversation (avec le consentement clair du patient) puis rédige la note clinique. Le médecin la relit, corrige ce qui est faux et la signe. Le médecin est entièrement responsable de la note ; l'outil ne fait que supprimer la frappe. C'est le même schéma « la machine rédige, l'humain relit » que montre l'affaire Elanco au [Chapitre 25 — Administration et finances](ch25-administration-and-finance.md). L'outil ne pose pas de diagnostic. Il met par écrit ce qui a été dit pour que le médecin puisse le vérifier.

**Acheminement des documents.** Un outil lit les lettres d'orientation et les formulaires entrants, en extrait les faits essentiels — le patient, la demande, l'urgence — et les classe et transmet. Une personne vérifie toujours la pile, mais le tri est fait, ainsi rien ne reste sans lecture.

**Un assistant aux questions pour les citoyens et les parents.** À l'école et au bureau communal, un chatbot répond aux questions répétées en langage simple et dans plusieurs langues, à toute heure. Un parent qui demande « quels documents me faut-il pour l'admission ? » ou un citoyen qui demande « comment faire une demande pour ce permis ? » obtient une réponse immédiate. Le personnel du bureau ne traite que les questions que le bot ne peut pas.

Remarquez la ligne qui ne bouge jamais. L'IA réserve, rappelle, rédige, extrait et répond. Un médecin signe la note clinique. Un assistant social tranche une demande. Un enseignant prend la décision pédagogique. Dans ces contextes, l'IA touche l'administration autour de la décision, jamais la décision elle-même.

## Les outils

Les outils sont ordinaires, mais ils sont déployés sous un ensemble de règles beaucoup plus strict.

- **Un système de rendez-vous et de rappels** avec chatbot et gestion téléphonique pour les réservations courantes.
- **Un outil de documentation ambiante** qui rédige les notes de consultation à partir d'une conversation enregistrée, pour que le clinicien les relise et les signe.
- **Un outil d'extraction de documents** qui lit les lettres et les formulaires et les achemine.
- **Un chatbot de questions** pour les parents et les citoyens, fonctionnant en plusieurs langues.

Comment choisir ces outils sans être ébloui par une démo est traité au [Chapitre 17 — Choisir ses outils sans se faire avoir](ch17-choosing-tools-without-being-fooled.md). Comment les connecter au système de patients du cabinet ou au système de dossiers du bureau se trouve au [Chapitre 19 — Connecter l'IA aux systèmes que vous utilisez déjà](ch19-connecting-ai-to-systems-you-already-use.md).

**La barre de conformité est tout l'enjeu ici.** Les données de santé et les données sur les enfants ne peuvent pas être collées dans un chatbot public. Ces organismes doivent utiliser des outils qui gardent la donnée protégée : un service de niveau entreprise avec un contrat clair de non-apprentissage et de non-partage et un accord de traitement des données, ou un modèle exécuté sur leurs propres machines ou dans un cloud contrôlé et dans la même région. L'auto-hébergement est expliqué au [Chapitre 8 — Auto-hébergement : gardez vos données sous contrôle](ch08-self-hosting-keep-your-data-under-control.md). Le danger que le personnel colle en douce des données sensibles dans des outils publics — l'IA fantôme — fait l'objet du [Chapitre 9 — Services tiers et IA fantôme](ch09-third-party-services-and-shadow-ai.md). Garder la donnée dans le pays ou la région, plutôt qu'à l'étranger, c'est la question de souveraineté du [Chapitre 11 — Souveraineté numérique](ch11-digital-sovereignty.md). Et les obligations légales pour cette catégorie de données sont exposées au [Chapitre 10](ch10-privacy-and-gdpr.md) et au [Chapitre 5](ch05-rules-and-legal-responsibility.md).

Deux règles pratiques en découlent. D'abord, la **minimisation des données** : collectez et traitez seulement ce qui est nécessaire. Un bot de rendez-vous n'a pas besoin du dossier médical complet d'un patient. Ensuite, la **piste d'audit** : chaque action de l'IA et chaque relecture humaine doivent être journalisées, pour que l'organisme puisse montrer plus tard qui a fait quoi.

## Les coûts

Voici un budget illustratif de première année pour un cabinet comme Riverside. Ce sont des chiffres inventés pour montrer la forme. Utilisez les vôtres. Le travail de conformité rend ces contextes plus coûteux à mettre en place qu'un commerce.

**Coûts directs.**
- Système de rendez-vous et de rappels : environ 6 000 € par an.
- Outil de documentation ambiante (conforme, avec accord de traitement des données) : environ 14 400 € par an.
- Extraction et acheminement de documents : environ 7 200 € par an.
- Chatbot de questions pour les patients : environ 3 600 € par an.
- Mise en place, intégration et travail de conformité (analyse d'impact sur la protection des données, examen des fournisseurs, revue de sécurité) : environ 18 000 € une fois pour toutes.
- Formation du personnel : environ 5 000 € une fois pour toutes.

Total première année : environ **54 200 €**. En années de croisière, les abonnements récurrents reviennent à environ **31 200 €**.

**Coûts indirects.**
- Les cliniciens passent du temps à relire chaque note rédigée. C'est le filet de sécurité et il doit rester.
- La charge de conformité : une analyse d'impact sur la protection des données n'est pas gratuite, et elle doit être faite avant la mise en service, pas après.
- Le creux d'apprentissage pendant que le personnel et même les patients s'adaptent.
- Le coût d'une erreur si une ébauche est crue sans vérification — dans un cabinet, cela peut nuire à un patient, ce qui est bien pire qu'une vente perdue.
- Une surveillance continue pour que les outils restent conformes quand les règles changent.

La méthode complète pour compter ces coûts et transformer les économies en un chiffre de retour se trouve au [Chapitre 16 — Objectifs, coûts et retour sur investissement](ch16-goals-costs-and-return-on-investment.md). Dans un contexte réglementé, ajoutez le coût de la conformité au registre avant de compter la moindre économie.

## Les résultats

Après un an, mesuré par rapport à une référence que le cabinet a enregistrée avant de commencer, le résultat illustratif ressemble à ceci. Vos chiffres seront différents. Ils montrent à quoi peut ressembler une bonne adaptation.

- **Les absences ont baissé.** Les rappels automatiques ont amené plus de patients à leurs rendez-vous, donc moins de créneaux perdus et plus de gens reçus.
- **La file téléphonique s'est raccourcie.** Le chatbot et la prise de rendez-vous autonome ont géré les appels courants, si bien que l'accueil a pu se concentrer sur les patients qui avaient besoin d'une personne.
- **Le temps de documentation a diminué.** Les médecins ont passé moins de temps à taper des notes et plus auprès des patients, car ils partaient d'une ébauche à vérifier au lieu d'une page blanche.
- **Les documents ont circulé plus vite.** Les orientations et les formulaires étaient triés et acheminés automatiquement, donc moins sont restés sans lecture et moins de patients ont été laissés en attente.
- **L'accès s'est amélioré.** L'assistant multilingue a aidé les parents et les citoyens qui ne parlent pas la langue locale à obtenir des réponses sans attendre un interprète.

La mise en garde honnête : rien de tout cela n'a été instantané. L'outil de documentation rédigeait des notes imparfaites au début et exigeait que chaque médecin corrige son style. Le bot de rendez-vous malcomprenait certaines demandes au départ. Les gains ont monté en quelques semaines, comme le prévoit l'avertissement sur la courbe d'apprentissage du [Chapitre 16](ch16-goals-costs-and-return-on-investment.md). Le cabinet a mesuré les vrais chiffres après la montée, pas pendant.

## Leçons tirées

**Des données réglementées signifient une barre plus haute, dès la première étape.** Les données de santé et les données sur les enfants sont de catégorie particulière. Vous ne pouvez pas les traiter comme une fiche produit. Utilisez des outils conformes, signez un accord de traitement des données, gardez la donnée dans la région, et faites une analyse d'impact sur la protection des données avant la mise en service. Les règles sont au [Chapitre 10](ch10-privacy-and-gdpr.md) et au [Chapitre 5](ch05-rules-and-legal-responsibility.md).

**Ne jamais automatiser la décision.** Un outil peut rédiger une note clinique, mais un médecin la signe et l'assume. Un outil peut trier une demande, mais un assistant social la tranche. Dans ces contextes, l'IA travaille sur l'administration autour de la décision et ne prend jamais la décision. C'est à la fois une règle de sécurité et, pour les usages à plus haut risque, une règle légale sous la loi européenne sur l'IA.

**Le consentement à l'enregistrement n'est pas facultatif.** La documentation ambiante enregistre une conversation. Le patient doit le savoir et accepter, clairement et à l'avance. N'enregistrez pas en douce. C'est un traitement de données personnelles au sens du [Chapitre 10](ch10-privacy-and-gdpr.md).

**La minimisation des données vous protège.** Donnez à chaque outil seulement la donnée dont il a besoin. Le bot de rendez-vous n'a pas besoin du dossier médical complet. Moins un outil touche de données sensibles, moindre est le dégât s'il se trompe.

**Gardez une piste d'audit.** Journalisez ce que l'IA a fait et ce que l'humain a relu. Dans un contexte réglementé, pouvoir montrer le registre plus tard compte autant que le résultat lui-même.

**Méfiez-vous de la réponse fausse mais assurée.** Une note rédigée qui déforme ce qui a été dit, ou un chatbot qui donne une consigne erronée, peut causer un vrai préjudice ici. Un humain doit vérifier. Le problème de fiabilité est au [Chapitre 2 — L'IA expliquée simplement](ch02-ai-explained-simply.md), et le devoir d'honnêteté est au [Chapitre 4 — IA éthique : faire ce qu'il faut](ch04-ethical-ai-doing-the-right-thing.md).

**L'IA peut élargir l'accès, pas seulement réduire les coûts.** L'assistant multilingue et le chatbot toujours ouvert ont aidé des gens qui autrement ont du mal à joindre le bureau. Dans les services publics, cette équité est un résultat qui vaut autant que l'argent économisé.

**Mesurez honnêtement et attendez-vous à la montée.** Enregistrez la référence avant de commencer. Jugez le projet après la courbe d'apprentissage, pas pendant. La méthode est au [Chapitre 22 — Mesurer les résultats et le ROI](ch22-measuring-results-and-roi.md).

La leçon pour les cabinets, les écoles et les bureaux publics est la même que pour tout secteur, avec la barrière la plus stricte de toutes : trouvez la charge administrative — planification, documents, questions répétées — laissez l'IA rédiger, trier et répondre, gardez un humain formé sur chaque décision, protégez la donnée sensible comme la loi l'exige, et mesurez honnêtement. Le prix n'est pas seulement un bureau moins cher. C'est plus de temps auprès des patients, des élèves et des citoyens — ce qui est tout le sens du travail.
