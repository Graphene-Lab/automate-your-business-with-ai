# Chapitre 4 — L'IA éthique : faire ce qu'il faut

## En mots simples

L'IA éthique, ce n'est pas un cours de philosophie. C'est un ensemble de choix concrets que vous faites avant d'allumer un système.

Voici l'idée, simplement. Un système d'IA prend des décisions, ou aide des gens à en prendre. Ces décisions touchent de vraies personnes : clients, employés, candidats, patients. Quand une machine affecte la vie de quelqu'un, quelqu'un doit en répondre. Et ce quelqu'un, c'est vous, l'entreprise qui a choisi de l'utiliser.

Beaucoup de dirigeants considèrent l'éthique comme un luxe. Quelque chose pour les grandes entreprises avec des services juridiques, ou une phrase marketing pour le rapport annuel. Ce chapitre défend le contraire. L'éthique est une nécessité, pour trois raisons simples.

D'abord, **une IA non éthique coûte de l'argent**. Un outil de recrutement biaisé, un chatbot qui ment, un système qui laisse fuiter des données privées — chacun peut finir en procès, en amende, ou en perte de confiance publique qui met des années à se réparer.

Ensuite, **une IA non éthique est généralement une mauvaise IA**. Un outil qui discrimine est aussi un outil qui écarte de bons candidats. Un outil incapable de s'expliquer est aussi un outil que vous ne pouvez pas débugger. Le correctif éthique et le correctif de qualité sont souvent le même.

Enfin, **la loi l'exige désormais**. Dans l'Union européenne, les règles sur la maîtrise de l'IA et sur les systèmes à haut risque sont déjà en vigueur ou arrivent selon un calendrier fixé. Le [chapitre 5](ch05-rules-and-legal-responsibility.md) détaille ces règles. Ce chapitre, lui, couvre la réflexion qui les sous-tend.

Une phrase traverse tout ce qui suit : **vous ne pouvez pas confier votre responsabilité à une machine, mais vous pouvez lui confier votre travail.** La machine fait les gros efforts. Vous gardez le jugement, la supervision, et le blâme.

## Un peu d'histoire

L'éthique et la technologie se sont rencontrées plusieurs fois, et chaque rencontre a produit une règle.

En 1942, l'écrivain Isaac Asimov publie ses « Trois lois de la robotique » dans une nouvelle de science-fiction : un robot ne peut pas faire de mal à un humain, doit obéir aux ordres, et doit se protéger lui-même, dans cet ordre. Ces lois sont de la fiction, mais elles ont planté une vraie question qui anime encore le domaine : comment faire pour qu'une machine se comporte bien ?

La conversation moderne et sérieuse a commencé en **2017 à Asilomar**, en Californie. Des chercheurs en intelligence artificielle se sont réunis et ont rédigé une longue liste de principes pour une IA sûre et bénéfique. Ce n'était pas une loi. C'était un avertissement de la part de ceux qui construisaient la technologie : cette technologie avait besoin de garde-fous.

Un travail institutionnel a suivi rapidement. L'**IEEE**, un organisme professionnel d'ingénieurs, a lancé un projet sur la conception éthique des systèmes autonomes. L'**OCDE** a publié en 2019 des principes concertés sur l'IA. En 2021, l'**UNESCO** a adopté une recommandation mondiale sur l'éthique, approuvée par 193 pays. L'Union européenne est passée des principes aux règles contraignantes : en 2018, elle a constitué un groupe d'experts dont la checklist de l'« IA de confiance » est devenue la base du Règlement européen sur l'IA.

Remarquez la forme de cette histoire. Elle est passée des récits, aux principes, aux checklists, à la loi. Chaque étape rendait la précédente plus concrète et plus applicable. Une petite entreprise d'aujourd'hui se trouve au bout de cette ligne. Le débat abstrait est terminé. Ce qui reste, c'est un ensemble d'attentes que vous êtes censé satisfaire.

## Curiosité

### 4.7 La loi exige désormais que votre personnel comprenne l'IA

Voici un fait qui surprend la plupart des dirigeants. Depuis le **2 février 2025**, une entreprise européenne qui utilise l'IA a l'obligation légale de s'assurer que ses gens la comprennent.

Cela vient de l'**Article 4 du Règlement européen sur l'IA**, qui porte sur la « maîtrise de l'IA ». En mots simples, la loi dit que les fournisseurs et les déployeurs de systèmes d'IA doivent prendre des mesures pour garantir, dans la limite de leurs moyens, un niveau suffisant de maîtrise de l'IA chez leur personnel et chez toute personne exploitant un système d'IA en leur nom.

Un **déployeur** est simplement une entreprise qui utilise un système d'IA, par opposition à un **fournisseur** qui en construit un. La plupart des petites et moyennes entreprises sont des déployeurs. Cela signifie que l'Article 4 s'applique à vous même si vous n'écrivez jamais une ligne de code.

La loi est prudente sur ce que « suffisant » veut dire. Cela doit être adapté aux connaissances techniques, à l'expérience et à la formation de chaque personne, ainsi qu'au contexte où l'IA est utilisée et aux personnes qu'elle affecte. Un agent de support qui utilise un chatbot n'a pas besoin du même niveau de compréhension que le manager qui approuve son usage.

Surtout, le Règlement précise que cette obligation **ne vous demande pas de garantir un niveau de maîtrise précis pour qui que ce soit.** C'est une obligation de moyens, pas une promesse de résultat. Vous devez montrer que vous avez pris des mesures raisonnables : formation, consignes, rôles clairs. Vous n'avez pas à certifier que tout le monde a réussi un examen.

Pourquoi c'est intéressant pour un dirigeant ? Parce que cela transforme « l'éthique de l'IA » d'une valeur vague en une tâche concrète avec une échéance. On peut vous demander, à vous, un régulateur, un client ou un tribunal : « qu'avez-vous fait pour vous assurer que vos gens comprenaient l'IA que vous avez mise devant eux ? » « Nous l'avons achetée en espérant » n'est pas une réponse. Une courte session de formation, une politique écrite et un responsable nommé, si. L'obligation de maîtrise est la partie la moins chère de la conformité et celle qui a l'effet le plus large : un personnel qui comprend qu'un modèle peut se tromper est un personnel qui repère les problèmes tôt.

## Un exemple d'entreprise réel

### L'outil de recrutement qui a appris à ne pas aimer les femmes

En juillet 2018, l'agence de presse Reuters a rapporté qu'Amazon avait construit un système d'IA pour filtrer les candidatures, et qu'il avait un grave défaut : il favorisait les hommes.

L'histoire est une leçon limpide sur les biais. Amazon avait entraîné l'outil sur dix ans de CV reçus. Pendant la majeure partie de ces années, la plupart des candidats aux postes techniques étaient des hommes. Le système a appris, à partir de cet historique, qu'« un bon candidat » ressemblait aux candidats qu'il avait déjà embauchés — surtout des hommes.

Il est allé plus loin que les signaux évidents. Il s'est mis à pénaliser les CV contenant le mot « femmes », comme dans « capitaine du club d'échecs féminin ». Il dégradait les diplômées de deux colleges réservés aux femmes. Il récompensait un langage plus courant dans les CV d'hommes, comme « exécuté » ou « conquis », et punissait des formulations plus douces plus fréquentes chez les femmes.

Les ingénieurs d'Amazon ont essayé de corriger. Ils ont supprimé les termes liés au genre. Mais le système continuait à trouver d'autres variables substitutives — des signaux indirects qui tenaient lieu de genre. Ils ne pouvaient pas être sûrs que l'outil soit équitable. Amazon a fini par dissoudre l'équipe et a cessé d'utiliser le système comme filtre principal.

Deux leçons se détachent.

D'abord, **le biais n'était pas dans le code. Il était dans les données.** Personne n'a écrit « préférer les hommes ». Le modèle a absorbé un déséquilibre du passé et l'a reproduit à grande échelle. Un recruteur humain avec le même préjugé affecte quelques candidats. Un modèle avec ce préjugé affecte tous les candidats, instantanément, et a l'air objectif en le faisant.

Ensuite, **l'entreprise l'a repéré avant que cela ne provoque un désastre public**, et a choisi de s'arrêter. C'était le geste éthique, et c'était aussi le geste sensé. Un outil qui écarte en silence de bons candidats à cause de leur genre perd des talents et attire un procès pour discrimination. Le correctif éthique et le correctif commercial pointaient dans la même direction. Si vous utilisez l'IA pour classer, filtrer, noter ou trier des personnes de quelque manière que ce soit, le même piège s'applique.

## Comment faire

### 4.3 Les six principes d'une adoption responsable

Les cadres de réflexion ne sont utiles que si vous pouvez agir dessus. Ces six principes sont ordonnés de sorte que chacun réponde à une question que vous devez réellement trancher avant et pendant un projet.

**Principe 1 : Décidez qui est responsable.** Avant toute chose, nommez une personne. Pas une équipe, pas un fournisseur — un humain nommé qui possède ce système d'IA et répond de ses résultats. Si vous n'arrivez pas à nommer cette personne, vous n'êtes pas prêt à déployer. Une responsabilité qui appartient à tout le monde n'appartient à personne.

**Principe 2 : Comprenez les impacts et planifiez.** Écrivez qui ce système touche et comment. À qui s'applique-t-il ? Que décide-t-il à leur sujet ? Quel est le pire dommage réaliste ? Un bot de service client qui donne une mauvaise réponse sur un remboursement agace quelqu'un. Un outil de crédit qui rejette à tort un candidat lui refuse de l'argent. Planifiez le pire cas, pas seulement le cas moyen.

**Principe 3 : Mesurez et gérez les risques.** Un risque que vous ne voyez pas est un risque que vous ne pouvez pas corriger. Décidez comment vous testerez le système avant le lancement et comment vous le surveillerez après. Contrôlez un échantillon de ses décisions. Suivez les réclamations. Fixez un seuil qui déclenche une revue humaine. La mesure transforme un espoir en un contrôle.

**Principe 4 : Soyez transparent et explicable.** Les gens doivent savoir quand ils ont affaire à une IA, et ils doivent pouvoir obtenir une raison claire pour une décision qui les affecte. « Le modèle l'a dit » n'est pas une raison. Si vous ne pouvez pas expliquer une décision en une phrase, vous ne devriez pas laisser cette décision tenir toute seule. Voir la section 4.5.

**Principe 5 : Protégez la vie privée et les données.** Les données personnelles sont le carburant de la plupart des IA. Traitez-les avec soin : ne collectez que ce dont vous avez besoin, sachez où elles vont, et ne nourrissez jamais un outil que vous n'avez pas vérifié avec des détails clients. Le volet légal est traité au [chapitre 10](ch10-privacy-and-gdpr.md) ; le volet sécurité au [chapitre 6](ch06-cybersecurity-in-the-ai-era.md).

**Principe 6 : Gardez les humains aux commandes.** Pour toute décision qui compte, un humain doit pouvoir revoir, contredire et arrêter le système. « Humain dans la boucle » signifie que l'humain est un vrai décideur, pas une chambre d'enregistrement. Concevez le flux de travail de sorte qu'une personne puisse dire non, et que dire non soit facile et attendu.

Passez ces six en checklist sur chaque projet. Si vous ne pouvez pas en satisfaire un, arrêtez-vous et corrigez-le avant d'avancer. Ils sont peu coûteux à appliquer au départ et coûteux à retrofit plus tard.

## Éthique et responsabilité

### 4.1 Pourquoi l'éthique n'est pas un luxe mais une nécessité

Traitez l'éthique comme un centre de coût et vous la supprimerez. Traitez-la comme un contrôle de risque et vous ne le ferez pas. Voici le dossier commercial honnête.

**Le risque de se tromper est grand et concret.** Les plaintes pour discrimination, les violations de données, les amendes pour contenus trompeurs et les dommages réputationnels coûtent tous de l'argent réel et du temps réel. Un seul système biaisé qui aboutit à la mauvaise décision sur un groupe protégé peut déclencher des enquêtes sur tous les dossiers qu'il a touchés.

**Le bénéfice de bien faire est opérationnel, pas seulement moral.** Les systèmes explicables sont plus faciles à débugger. Les systèmes équitables élargissent votre vivier de candidats et de clients au lieu de le rétrécir. La rigueur sur les données privées réduit votre exposition aux violations. La conception éthique et la bonne conception se recouvrent presque complètement.

**La confiance est votre vrai produit.** Les petites entreprises gagnent sur la confiance. Un client qui croit que vous traitez ses données et sa candidature équitablement est un client qui revient. Un client qui soupçonne une boîte noire d'avoir pris une décision froide et inexpliquable à son sujet, non. L'éthique est la façon dont vous gardez la confiance dont dépendent les petites entreprises et que les grandes ont souvent en moins.

Donc l'éthique n'est pas une décoration que vous ajoutez quand il vous reste du budget. C'est le plancher sous l'ensemble. Le sauter, ce n'est pas économiser de l'argent ; c'est emprunter des ennuis à un taux d'intérêt élevé.

### 4.2 Les quatre piliers d'une gouvernance éthique

Comment faire tenir l'éthique dans toute une entreprise, et pas seulement sur un projet ? La gouvernance repose sur quatre piliers. Retirez-en un et la structure penche.

**Pilier 1 : Les principes.** Une courte déclaration écrite de ce que votre entreprise croit à propos de l'IA — équité, honnêteté, contrôle humain, vie privée. C'est votre boussole interne. Elle doit tenir sur une page et être lue par tous ceux qui touchent à l'IA. Des principes sans les trois autres piliers sont des affiches au mur.

**Pilier 2 : La réglementation.** Les règles externes que vous devez suivre : le Règlement européen sur l'IA, le RGPD, le droit de la consommation, le droit anti-discrimination. Vous ne les choisissez pas ; elles s'appliquent à vous. Le [chapitre 5](ch05-rules-and-legal-responsibility.md) est le foyer approfondi du Règlement sur l'IA, et le [chapitre 10](ch10-privacy-and-gdpr.md) pour le RGPD. Sachez quelles règles lient vos cas d'usage.

**Pilier 3 : Les normes techniques.** Les façons convenues de construire et de tester qui transforment les principes en pratique : tester les biais, journaliser les décisions, documenter les modèles, normes de sécurité, gestion de la qualité. Les normes sont la façon dont « soyez équitables » devient « lancez ce test et enregistrez le résultat ». Elles rendent l'éthique auditable.

**Pilier 4 : L'auto-régulation.** Ce que vous faites parce que vous l'avez choisi, au-delà du minimum exigé par la loi : un comité de revue interne, un code de conduite, une personne qui peut mettre son veto à un usage nuisible, l'habitude de demander « devons-nous ? » et pas seulement « pouvons-nous ? ». L'auto-régulation est la culture qui comble les lacunes que la loi laisse.

Une entreprise en bonne santé a les quatre. Les principes indiquent la direction. La réglementation fixe le plancher. Les normes rendent le tout mesurable. L'auto-régulation vous garde honnête quand personne ne regarde.

### 4.4 Biais et discrimination : comment les reconnaître et les éviter

Un **biais**, c'est quand un système traite certaines personnes moins bien que d'autres de façon systématique, pas par accident mais à cause de la manière dont il a été construit ou entraîné. Quand ce schéma correspond à une caractéristique protégée — genre, race, âge, handicap, religion, et d'autres — cela devient une **discrimination** illégale dans beaucoup d'endroits.

Le biais entre généralement par les données, comme l'exemple Amazon l'a montré. Si vos décisions passées favorisaient un groupe, un modèle entraîné dessus apprend à favoriser ce groupe. Le modèle est un miroir. Il reflète les exemples, y compris leurs défauts.

**Comment le reconnaître.** Posez trois questions à tout système qui trie ou note des personnes :

1. **Qui est dans les données d'entraînement, et qui manque ?** Si un groupe a été historiquement sous-représenté, le système le servira probablement plus mal.
2. **Le système utilise-t-il des variables substitutives ?** Vous pouvez supprimer le champ genre et avoir quand même un biais, parce que les intitulés de poste, les écoles, les loisirs ou les trous dans un CV peuvent tenir lieu de genre. Cherchez les signaux qui corrèlent avec un trait protégé.
3. **Les résultats sont-ils inégaux selon les groupes ?** Le test le plus simple : prenez les décisions du système et regroupez-les par genre, âge ou origine ethnique. Si un groupe est rejeté à un taux bien plus élevé, enquêtez sur la raison. L'écart est le voyant d'alerte.

**Comment l'éviter.** Utilisez des données qui représentent les gens que vous servez réellement. Testez les résultats par groupe avant le lancement, pas après. Gardez un humain revoyant les décisions limites. Documentez ce que vous avez vérifié, pour pouvoir montrer votre diligence. Et rappelez-vous que supprimer une étiquette ne supprime pas une variable substitutive — vous devez chercher les signaux indirects volontairement.

Le biais n'est pas un échec moral de la machine. C'est un échec des humains qui ont choisi les données et ont sauté le test. C'est une bonne nouvelle : les échecs humains se réparent par un processus humain.

### 4.5 Transparence et explicabilité : pourquoi il est important de savoir comment l'IA décide

La **transparence** signifie que les gens savent quand l'IA est impliquée et ce qu'elle fait à grands traits. L'**explicabilité** signifie que vous pouvez donner une raison claire pour une décision précise.

Ils comptent pour trois raisons.

**La confiance.** Une personne accepte plus volontiers une décision quand elle la comprend. « Votre candidature n'a pas été retenue parce que le poste exige X et votre profil montre Y » est dur à accepter mais facile à comprendre. « Rejeté par une IA » sans raison semble arbitraire et invite à la colère et aux réclamations.

**Le contrôle.** Vous ne pouvez pas corriger ce que vous ne voyez pas. Si un modèle prend une mauvaise décision et que personne ne peut dire pourquoi, vous ne pouvez pas la corriger, et cela se reproduira. Un système explicable vous permet de remonter à la cause et de la supprimer. Un système opaque cache ses propres défauts jusqu'à ce qu'ils fassent des dégâts.

**La loi et l'équité.** Dans plusieurs contextes juridiques, y compris sous le RGPD pour certaines décisions automatisées, une personne a droit à une explication. Au-delà de la loi, une décision inexpliquable à propos d'une personne est difficile à défendre comme équitable. Si vous ne pouvez pas formuler la raison, vous ne pouvez pas prouver qu'elle n'était pas biaisée.

Une règle pratique : **pour toute décision qui affecte de manière significative une personne, vous devez pouvoir produire une raison en une phrase qu'un non-expert comprendrait.** Si vous ne le pouvez pas, cette décision a besoin d'un humain derrière elle, pas d'une machine devant eux. Méfiez-vous des fournisseurs qui prétendent que leur système est « entièrement explicable ». Demandez-leur de vous le montrer, sur un vrai cas, pendant la réunion. Une prétention que vous ne pouvez pas voir démontrée est une prétention sur laquelle vous ne devriez pas vous appuyer.

### 4.6 La responsabilité humaine : qui est responsable si l'IA fait une erreur ?

C'est la question que tout dirigeant pose. La réponse est simple et inconfortable : **c'est vous.**

Un système d'IA est un outil. Les outils ne portent pas de responsabilité légale ; ce sont les gens qui les utilisent qui la portent. Si un livreur que vous employez grille un feu rouge, vous êtes responsable en tant qu'employeur. Si une IA que vous déployez prend une décision nuisible, la même logique s'applique. La machine ne peut pas être poursuivie, amendée ni humiliée. Vous, si.

Quelques points qui rendent cela concret :

- **« L'IA du fournisseur l'a fait » n'est pas une défense.** Vous avez choisi l'outil, vous l'avez mis devant des gens, et vous avez gardé ou supprimé le contrôle humain. Ce sont vos choix, et c'est là que se trouve la responsabilité.
- **L'automatisation ne transfère pas la responsabilité ; elle la concentre.** Un humain qui prend 50 décisions par jour répartit le risque. Un système qui prend 5 000 décisions identiques le concentre. Une règle défectueuse désormais nuit à des milliers de personnes à la fois, et cette règle vous appartient.
- **La supervision humaine est votre principale protection.** Là où un humain qualifié peut revoir et contredire une décision, votre responsabilité baisse. Là où vous laissez le système agir seul sur quelque chose d'important, votre responsabilité monte. Garder les humains aux commandes (Principe 6) n'est pas seulement éthique ; c'est ainsi que vous vous protégez.
- **Documenter votre processus est votre preuve.** Si on vous conteste, vous voulez montrer que vous avez évalué le risque, testé les biais, gardé un humain dans la boucle, et agi raisonnablement. Une trace papier d'un bon processus est votre meilleure défense.

La façon propre de tenir tout cela : **l'IA décide vite et à grande échelle ; un humain décide s'il la laisse faire, et assume le blâme quand cela tourne mal.** Ne laissez jamais la commodité de l'automatisation brouiller cette ligne.

## Erreurs à éviter

**Erreur 1 : Traiter l'éthique comme une étape ultérieure.** L'ajouter après le lancement et vous découvrez les problèmes trop tard et les corrigez en public.

**Erreur 2 : Supposer que le fournisseur s'en charge.** Le fournisseur construit l'outil ; vous le déployez, et la responsabilité de la façon dont il touche vos gens vous revient.

**Erreur 3 : Croire que supprimer une étiquette supprime le biais.** Enlevez le champ genre et le modèle trouve une variable substitutive ; cherchez les signaux indirects volontairement.

**Erreur 4 : Laisser « le modèle l'a dit » être la réponse finale.** Si vous ne pouvez pas expliquer une décision en une phrase simple, ne la laissez pas tenir seule.

**Erreur 5 : La chambre d'enregistrement.** Un humain « dans la boucle » qui est toujours d'accord avec l'IA n'est pas une supervision ; rendez la revue réelle et le « non » facile.

**Erreur 6 : Sauter la trace papier.** Pas de documentation signifie pas de preuve que vous avez agi de façon responsable quand on vous conteste.

**Erreur 7 : Confondre une déclaration de valeurs avec une gouvernance.** Une affiche sur l'« IA responsable » sans responsable nommé, sans test et sans droit de veto est une décoration, pas une gouvernance.

**Erreur 8 : Ignorer l'obligation de maîtrise de l'IA parce qu'elle semble floue.** L'Article 4 est la loi depuis février 2025 ; un personnel formé est à la fois une réponse légale et votre contrôle le moins cher.

## Exercice pratique

### 4.8 Évaluer les risques éthiques d'un projet IA dans votre entreprise

Choisissez un projet d'IA que vous envisagez, ou un que vous menez déjà. Travaillez ceci sur papier. Cela prend environ une heure et fera remonter la plupart des risques sérieux.

**Étape 1 — Nommez le responsable.** Écrivez un nom : la personne responsable de ce système. Si vous hésitez, c'est votre premier constat.

**Étape 2 — Cartographiez les personnes affectées.** Listez tous les groupes que le système touche : clients, candidats, employés, autres. Pour chacun, écrivez ce que le système décide ou influence à leur sujet.

**Étape 3 — Pire dommage réaliste.** Pour la décision la plus sérieuse, écrivez le pire résultat plausible pour une vraie personne. Soyez précis. « Un parent seul se voit refuser un crédit pour lequel il est éligible » est un constat ; « un mauvais résultat » ne l'est pas.

**Étape 4 — Contrôle des biais.** Posez les trois questions : qui manque dans les données, quelles variables substitutives pourraient tenir lieu de trait protégé, et les résultats sont-ils inégaux par groupe. Si le système trie des personnes, vous devez pouvoir répondre aux trois.

**Étape 5 — Test d'explicabilité.** Prenez une décision que le système prend et écrivez la raison en une phrase qu'un non-expert comprendrait. Si vous ne le pouvez pas, signalez-le : cette décision a besoin d'un humain.

**Étape 6 — Contrôle humain.** Décrivez exactement où un humain revoit, peut contredire, et peut arrêter le système. Si la réponse est « nulle part », c'est votre correction la plus urgente.

**Étape 7 — Données et vie privée.** Écrivez où vont les données, qui peut les voir, et si des données personnelles échappent à votre contrôle. Recoupez avec le [chapitre 10](ch10-privacy-and-gdpr.md).

**Étape 8 — Maîtrise.** Notez quel personnel a besoin d'une formation pour utiliser ce système de façon responsable, et ce que vous allez faire à ce sujet.

**Étape 9 — Décidez.** Pour chaque signal d'alerte, écrivez une action et un responsable. Un projet est prêt à avancer quand chaque dommage sérieux a un contrôle et un nom attachés.

Gardez cette page. C'est le premier brouillon de votre registre d'éthique et votre défense si on vous le demande un jour.

## Checklist

### 4.9 Votre politique d'éthique IA

- [ ] J'ai une déclaration d'une page sur nos principes d'IA : équité, honnêteté, contrôle humain, vie privée.
- [ ] Chaque système d'IA a un unique responsable humain nommé, pas une équipe ni un fournisseur.
- [ ] Pour chaque système, j'ai cartographié qui il affecte et ce qu'il décide à leur sujet.
- [ ] J'ai écrit le pire dommage réaliste pour chaque décision sérieuse.
- [ ] Pour tout système qui trie ou note des personnes, j'ai vérifié les groupes manquants, les variables substitutives et les résultats inégaux.
- [ ] Pour chaque décision qui affecte une personne, je peux produire une raison claire en une phrase.
- [ ] Un humain qualifié peut revoir, contredire et arrêter chaque décision importante.
- [ ] Je sais où vont nos données et qui peut les voir, et je ne nourris jamais d'outils non vérifiés avec des données personnelles.
- [ ] J'ai un plan pour élever la maîtrise de l'IA chez le personnel qui utilise nos systèmes (obligation de l'Article 4).
- [ ] Je sais quelles règles externes nous lient : le Règlement européen sur l'IA, le RGPD, le droit de la consommation et anti-discrimination.
- [ ] J'utilise des normes techniques : tests, journalisation, documentation, sécurité.
- [ ] J'ai une habitude d'auto-régulation : quelqu'un peut mettre son veto à un usage légal mais mauvais.
- [ ] Je garde un registre écrit de l'évaluation des risques pour chaque système.
- [ ] Je comprends que c'est l'entreprise, pas le fournisseur et pas la machine, qui est responsable des résultats.
- [ ] Je revois chaque système périodiquement, pas seulement au lancement.

## Points clés à retenir

- L'IA éthique est un contrôle de risque pratique, pas une philosophie : elle économise de l'argent, améliore la qualité et protège la confiance dont vivent les petites entreprises.
- La gouvernance repose sur quatre piliers — principes, réglementation, normes techniques et auto-régulation — et la structure penche si vous en laissez tomber un.
- Les six principes d'adoption mettent sur chaque projet un humain nommé, un plan contre les dommages, une mesure du risque, une explication, une protection des données et un contrôle humain.
- Le biais vient des données et se cache dans les variables substitutives ; vous le supprimez en testant les résultats par groupe, pas en effaçant une étiquette.
- La responsabilité ne se transfère jamais à la machine ni au fournisseur : l'entreprise qui déploie un système d'IA possède ses résultats, et un humain dans la boucle plus une trace papier sont votre meilleure protection.
