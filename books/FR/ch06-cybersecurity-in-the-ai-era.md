# Chapitre 6 — La cybersécurité à l'ère de l'IA

## En mots simples

Pendant la plus grande partie de l'histoire de l'informatique d'entreprise, la sécurité voulait dire une seule chose : empêcher les inconnus d'entrer dans votre bâtiment. Vous aviez une porte verrouillée, un mot de passe, un pare-feu. Le méchant était dehors. Vos données étaient dedans.

L'intelligence artificielle a brouillé cette frontière. Aujourd'hui, quand un employé tape une liste de clients, un contrat ou une fiche de paie dans un outil d'IA en ligne, ce texte quitte le bâtiment. Il voyage jusqu'à des ordinateurs qui appartiennent à quelqu'un d'autre. Il y sera peut-être stocké. Il sera peut-être lu par du personnel de support. Il sera peut-être gardé pendant des mois. Dans certains cas, il servira peut-être à améliorer le produit de cette entreprise. La plupart des gens n'y pensent jamais, parce que l'outil ressemble à une barre de recherche. Ce n'est pas une barre de recherche. C'est un service, géré par une entreprise, sur des machines que vous ne contrôlez pas.

L'IA change le tableau de la sécurité dans deux directions à la fois.

**Les attaquants sont devenus meilleurs.** Un modèle de langage donne à un criminel trois choses qui coûtaient cher avant : la vitesse, l'échelle et le fini. Un email d'hameçonnage qui, autrefois, ressemblait à une mauvaise traduction peut maintenant être écrit dans un allemand ou un japonais des affaires courant en quelques secondes, personnalisé avec des détails tirés d'un profil public. Une voix peut être copiée à partir de quelques secondes d'un enregistrement ; c'est ainsi que des employés de finance, dans des cas de fraude signalés, ont approuvé des virements parce que l'appelant semblait être leur propre patron. Rien de tout cela ne demande un génie. Cela demande un abonnement.

**Votre surface d'attaque a grossi.** « Surface d'attaque » est juste un terme pour désigner le nombre d'endroits par où quelqu'un peut entrer. Chaque fonctionnalité d'IA que vous ajoutez est une nouvelle porte : outils de chat, plugins qui accèdent à votre email, agents qui lisent des dossiers et envoient des messages, modèles entraînés sur vos archives, fournisseurs qui gardent une copie de chaque prompt et de chaque réponse. Il y a deux ans, votre entreprise avait une seule porte d'entrée. Elle en a peut-être quarante maintenant, et la plupart ont été ouvertes par votre propre personnel sans le dire à personne.

Une idée de plus organise tout le reste. La sécurité protège trois choses, connues par trois mots courts.

- **Confidentialité.** Seules les bonnes personnes voient les données.
- **Intégrité.** Les données n'ont pas été modifiées en secret.
- **Disponibilité.** Le système fonctionne quand vous en avez besoin.

La plupart des dirigeants traitent la sécurité de l'IA comme un problème de confidentialité seulement. Ce n'est pas le cas. Un concurrent qui empoisonne votre modèle est un problème d'intégrité. Un fournisseur dont les systèmes tombent en panne et bloquent vos paiements pendant des semaines est un problème de disponibilité, et c'est celui qui a causé le plus de dégâts dans l'histoire racontée plus loin dans ce chapitre. Quand vous examinez un outil d'IA, posez les trois questions.

Un avertissement. La pensée « nous sommes trop petits pour être attaqués » est fausse. Les attaques modernes sont automatisées : un logiciel balaie tout internet à la recherche de portes ouvertes, comme un voleur essaie chaque voiture d'un parking. On ne vous choisit pas parce que vous êtes intéressant. On vous frappe parce que vous étiez une cible facile, et parce que vous détenez des coordonnées clients, des coordonnées bancaires et des dossiers fiscaux avec très peu de protection autour.

La bonne nouvelle, c'est que la plupart des protections dont vous avez besoin ne sont pas de la haute technologie. C'est une courte liste d'habitudes ennuyeuses, une carte de l'endroit où vont vos données, et quelques contrôles au bon endroit.

Le volet légal des données personnelles est au [Chapitre 10](ch10-privacy-and-gdpr.md). L'utilisation d'outils d'IA par le personnel sans approbation — « l'IA fantôme » — est au [Chapitre 9](ch09-third-party-services-and-shadow-ai.md). La construction étape par étape est au [Chapitre 20](ch20-implementing-ai-securely.md).

## Un peu d'histoire

L'histoire de la sécurité répète une seule leçon : le périmètre se déplace, et les défenseurs mettent du temps à le remarquer.

En **1988**, le ver Morris a neutralisé environ dix pour cent des ordinateurs connectés du tout premier internet. Il a été écrit par un étudiant diplômé, pas par un criminel, et il a prouvé qu'un programme auto-reproductible pouvait traverser la planète en quelques heures. Pendant **les années 1990 et 2000**, la réponse standard était le modèle du périmètre : un pare-feu à la limite, un antivirus sur chaque PC, des données sur un serveur dans un placard. Cela fonctionnait tant que les données restaient où vous les aviez mises.

En **2013**, le détaillant américain Target a été piraté. Les attaquants ne se sont pas introduits chez Target. Ils se sont introduits chez une petite entreprise qui fournissait des équipements de chauffage et de climatisation pour ses magasins, ont pris les identifiants de connexion de cette entreprise, et s'en sont servis pour atteindre les systèmes de paiement de Target. Environ 40 millions de numéros de carte ont été volés. La leçon portait sur la connexion, pas sur le code : votre risque inclut désormais tous ceux à qui vous vous branchez.

En **2016**, Microsoft a mis en ligne un chatbot nommé Tay sur les réseaux sociaux. En un jour, des utilisateurs lui ont appris à publier du contenu offensant en lui soumettant des messages répétés, et il a été retiré. Personne n'a cassé le programme. Ils ont cassé ce que le modèle lisait. C'est la graine de l'injection de prompt, même si elle n'avait pas encore de nom.

En **2017**, le logiciel malveillant NotPetya s'est propagé depuis un logiciel de comptabilité ukrainien et a causé des dégâts chiffrés en dizaines de milliards de dollars dans le monde, touchant le géant du transport maritime Maersk, le fabricant pharmaceutique Merck, et beaucoup d'autres. Un seul maillon empoisonné dans une chaîne d'approvisionnement logicielle est devenu le problème de tout le monde d'un coup.

En **2020**, le travail à distance a supprimé le périmètre physique presque du jour au lendemain. En **2022**, ChatGPT a fait de l'IA générative un outil de bureau normal en quelques semaines, et le personnel a commencé à coller de vrai travail dans des outils sans contrat d'entreprise derrière. En **septembre 2022**, le chercheur en sécurité Simon Willison a publié un article intitulé « Prompt injection attacks against GPT-3 » et a donné un nom à un problème que les gens voyaient mais ne savaient pas décrire : des instructions cachées dans un texte que lit un modèle, et qui prennent le pas sur les instructions que vous lui avez données.

En **2023**, les modèles à poids ouverts signifiaient qu'une entreprise pouvait faire tourner l'IA sur son propre matériel, comme l'explique le [Chapitre 8](ch08-self-hosting-keep-your-data-under-control.md). La même année, des fournisseurs ont commencé à livrer des « agents » capables d'agir et pas seulement de répondre, ce qui a augmenté le coût de chaque erreur. En **2024**, le risque fournisseur est devenu impossible à ignorer, comme raconté dans la section Curiosité ci-dessous. À partir de **2025**, les agents sont arrivés avec des outils et des identifiants attachés, si bien que la zone d'effet d'une mauvaise permission est maintenant tout ce que cet agent peut atteindre.

Lisez la chronologie comme un seul long argument. Chaque étape a déplacé la confiance loin d'une porte verrouillée et vers une relation : un sous-traitant, un fournisseur, un plugin, un modèle, un agent. La sécurité a cessé d'être un mur et est devenue une question sur qui, et quoi, vous avez connecté.

## Curiosité

### 6.8 Le fournisseur qui a failli arrêter un système de santé

Le 12 février 2024, des attaquants se sont introduits dans Change Healthcare, une entreprise qui traite les factures médicales et les paiements aux États-Unis. D'après le témoignage que le directeur général de UnitedHealth Group a livré au Congrès américain en mai 2024, ils sont entrés par un portail d'accès à distance qui n'exigeait pas d'authentification à plusieurs facteurs — la deuxième vérification d'une connexion qui empêche la plupart des mots de passe volés de fonctionner. Il n'y avait pas de logiciel malveillant astucieux à la porte d'entrée. Il y avait un mot de passe volé et un deuxième verrou manquant. Les attaquants sont restés neuf jours à l'intérieur, se déplaçant en silence et copiant environ six téraoctets de données. Le 21 février, ils ont activé un rançongiciel et verrouillé les systèmes.

Change Healthcare est une filiale de UnitedHealth Group, et elle se trouve au milieu de la chaîne de paiement du système de santé américain. Quand elle s'est arrêtée, une très grande part des demandes de remboursement de médecins, des paiements de pharmacies et des autorisations d'assurance s'est arrêtée avec elle. Les petites cliniques ne pouvaient plus être payées et sont tombées à court de trésorerie en quelques semaines ; des groupes du secteur ont signalé des pertes pour les prestataires atteignant des dizaines de millions de dollars par jour à travers le réseau touché. De grands noms sans aucun lien avec la violation — chaînes de pharmacies, assureurs régionaux, un hôpital de la marine — ont trouvé leurs propres opérations bloquées, parce qu'ils faisaient tous transiter leurs données par le même intermédiaire.

UnitedHealth a ensuite avancé plus de 2 milliards de dollars de prêts d'urgence aux prestataires touchés à la mi-mars, et plus de 6 milliards à la mi-avril. Des reportages de Reuters et Wired ont dit qu'une rançon d'environ 22 millions de dollars en bitcoin a été versée à un portefeuille lié au groupe criminel ALPHV, aussi connu sous le nom de BlackCat, que UnitedHealth a confirmé le 29 février comme l'attaquant. En octobre 2024, UnitedHealth a estimé qu'environ 190 millions de personnes avaient vu leurs données touchées, l'une des plus grandes violations jamais enregistrées.

Pourquoi cela compte-t-il pour une petite entreprise qui ne touchera jamais une demande médicale ? À cause de qui était la vraie victime. Les hôpitaux et les pharmacies qui ont souffert n'ont pas été piratés. Beaucoup d'entre eux avaient une bonne sécurité. Ils ont été blessés parce qu'une entreprise au milieu de leur flux de travail a été piratée, et ils ne pouvaient pas survivre sans cette entreprise. Leur sécurité n'était bonne que jusqu'au fournisseur le moins protégé de leur chaîne.

Ajoutez maintenant l'angle de l'analytique, parce qu'il est plus proche de chez vous qu'il n'y paraît. En 2024, OpenAI a révélé un incident qui n'était pas du tout une violation de ses propres systèmes. Le problème venait de Mixpanel, un service d'analytique tiers utilisé sur le site développeur de son interface de programmation d'application. Les services d'analytique sont de petits morceaux de logiciel qu'une entreprise met sur son site web pour compter les visites et voir comment les gens cliquent. Ce fournisseur a été piraté, et les noms, adresses email et détails d'appareil de certains titulaires de compte ont été exposés. Le contenu des conversations, les mots de passe et les clés secrètes ne l'ont pas été.

Les dégâts, là, ont été limités. La leçon, non. Quand vous achetez un service d'IA, vous achetez aussi toutes les entreprises sur lesquelles ce service s'appuie : son analytique, son hébergement, ses outils de support, ses plugins. Vous héritez d'une chaîne d'approvisionnement que vous n'avez jamais choisie et dont vous n'avez peut-être jamais entendu parler.

## Un exemple réel d'entreprise

### L'ingénieur qui a demandé de l'aide au chatbot

En avril 2023, Bloomberg a rapporté que Samsung avait interdit les outils d'IA générative comme ChatGPT sur le matériel de l'entreprise. La raison n'était pas une théorie sur le risque. Des ingénieurs avaient collé du code source confidentiel dans un chatbot public en cherchant à corriger un bug, à plus d'une reprise, dans une division qui travaillait sur les semi-conducteurs — l'un des types de code les plus jalousement gardés au monde. Une note interne examinée par Bloomberg notait, selon toute apparence, qu'une enquête interne avait trouvé que 65 pour cent des personnes interrogées croyaient déjà que l'outil représentait un risque pour la sécurité.

Regardez cela du côté de l'ingénieur. Rien n'a été volé. Personne n'a forcé la porte. Une personne était bloquée sur un problème, a trouvé un outil qui l'a résolu en dix secondes, et s'en est servie. L'outil était excellent. Le jugement était mauvais. Le code n'était pas à elle pour être donné.

C'est l'échec de sécurité lié à l'IA le plus courant qui existe, et il n'a rien d'exotique. Il se produit dans les cabinets d'avocats quand quelqu'un colle le contrat d'un client pour le résumer. Dans les cabinets comptables avec une déclaration fiscale. Dans les agences avec une campagne client non encore publiée. Aux ressources humaines avec une pile de CV. Le schéma est toujours le même : un outil serviable, une personne pressée, et un copier-coller qui franchit une frontière que personne n'a tracée.

Deux choses en découlent. D'abord, la solution n'est pas seulement une interdiction, parce qu'une interdiction sans alternative n'arrête pas le comportement ; elle le cache, ce qui est pire, puisque maintenant vous ne pouvez plus voir les données circuler. Ensuite, la solution n'est pas seulement la formation, parce qu'une personne pressée à cinq heures du soir ne se souviendra pas d'une politique de quarante pages. La solution est de faire du chemin sûr le chemin facile : un outil approuvé plus rapide que l'outil dangereux, plus un contrôle qui attrape les pires données avant qu'elles ne partent. Les deux sont dans la section suivante.

## Comment faire

### 6.7 Comment vous protéger : pare-feu d'IA, filtres, surveillance

Faites cela dans l'ordre. Chaque étape dépend de celle qui la précède.

**Étape 1 : Dessinez la carte avant d'acheter quoi que ce soit.**
Prenez une feuille de papier. Listez chaque outil d'IA qui touche votre entreprise, y compris les gratuits sur les téléphones du personnel. Pour chacun : quelles données entrent, ce qui en sort, où c'est stocké, qui est le fournisseur, et si vous avez un contrat signé. Vous trouverez des outils dont vous ne saviez pas l'existence. C'est le document de sécurité le plus précieux que vous produirez cette année.

**Étape 2 : Mettez une seule porte entre vos gens et les services d'IA.**
Une « passerelle d'IA » ou un « pare-feu d'IA » est un point unique par où passe tout le trafic d'IA, pour que vous puissiez le voir et le contrôler. Des produits grand public font cela : services de sécurité de contenu et de bouclier de prompt des grandes plateformes cloud, garde-fous intégrés aux services de modèles cloud, passerelles conscientes de l'IA, et outils de prévention des fuites de données qui inspectent ce que envoient les employés. Vous devez savoir que la catégorie existe et ce qu'elle achète : un seul endroit pour autoriser ou bloquer des outils, inspecter le contenu et garder des journaux.

**Étape 3 : Filtrez ce qui sort.**
Le contrôle de plus grande valeur de cette liste. Configurez votre passerelle ou votre outil de prévention des fuites pour bloquer ou avertir sur les catégories qui ne doivent jamais partir : numéros d'identité nationale et fiscaux, numéros bancaires et de carte, informations de santé, fichiers de paie, contrats signés, code source et documents confidentiels clients. Une fenêtre pop-up qui dit « cela ressemble à des données personnelles, êtes-vous sûr ? » arrête à elle seule une grande part des accidents, parce que la plupart d'entre eux sont des accidents.

**Étape 4 : Filtrez ce qui entre.**
C'est la défense contre l'injection de prompt, et elle a une règle d'or : **ne laissez jamais un outil d'IA agir sur des instructions qu'il trouve dans un document, un email, une page web ou une feuille de calcul.** Un modèle qui lit votre boîte de réception doit résumer, pas obéir. Quand un outil doit agir, exigez qu'un humain confirme avant qu'il ne s'exécute. Traitez chaque document externe comme une entrée non fiable, comme vous traitez une pièce jointe d'un inconnu.

**Étape 5 : Donnez aux agents le moins de pouvoir possible.**
Décidez les permissions d'un agent sur le papier avant de le connecter. En lecture seule quand vous le pouvez. Son propre compte de service, jamais une connexion d'administrateur partagée. Un dossier, pas tout le disque. Un plafond de dépenses sur tout ce qui coûte de l'argent. Une limite de temps. Un responsable humain nommé. S'il n'a pas besoin de supprimer, ne le laissez pas supprimer. Donnez à l'outil le plus petit jeu de clés qui lui permet quand même de faire le travail.

**Étape 6 : Journalisez tout et lisez les journaux.**
Enregistrez qui a utilisé quel outil d'IA, quand, et à peu près pour quoi — puis relisez-le. Un coup d'œil de quinze minutes chaque semaine vous montre des outils non approuvés, un volume inhabituel, et des schémas que vous pouvez transformer en politique. Pas de journaux veut dire pas d'enquête : après un incident, vous serez à deviner.

**Étape 7 : Gardez un point de contrôle humain sur tout ce qui est irréversible.**
Toute action qui ne peut pas être annulée — envoyer de l'argent, supprimer des dossiers, envoyer une liste de clients par email, signer quelque chose — a besoin d'une étape d'approbation humaine. Pas une notification. Une approbation.

**Étape 8 : Ne négligez pas les bases ennuyeuses.**
L'IA ne remplace pas la sécurité ordinaire ; elle se pose par-dessus. Authentification à plusieurs facteurs sur chaque compte qui peut atteindre des données d'entreprise, y compris les portails fournisseurs. Un gestionnaire de mots de passe pour que personne ne réutilise de mots de passe. Des mises à jour rapides. Des sauvegardes testées gardées hors ligne. Une protection des points terminaux sur chaque machine. Si celles-ci sont faibles, aucun contrôle spécifique à l'IA ne vous sauvera.

**Étape 9 : Formez avec une règle, pas un manuel.**
Donnez au personnel une phrase qu'il peut emporter : *si vous ne le mettriez pas dans un email à un inconnu, ne le mettez pas dans un outil d'IA.* Puis dites-leur quoi faire à la place, et rendez cette alternative facile. Les règles sans alternatives sont ignorées.

**Étape 10 : Prévoyez la panne du fournisseur.**
Demandez à chaque fournisseur d'IA : que se passe-t-il si vous êtes indisponible pendant une semaine ? Ayez une solution de repli manuelle pour tout processus que vous avez rendu dépendant d'eux. La disponibilité est une propriété de sécurité, et l'histoire de la santé ci-dessus en est la preuve.

## Éthique et responsabilité

La sécurité est une question d'éthique avant d'être une question technique. Quand des clients vous donnent leur adresse, leur information de santé ou leur information de paiement, ils vous font confiance pour la garder en sécurité. La perdre n'est pas un accident qui vous est arrivé ; c'est un tort qui leur est fait. C'est le même devoir de diligence dont il est question au [Chapitre 4](ch04-ethical-ai-doing-the-right-thing.md), appliqué aux systèmes plutôt qu'aux décisions.

Trois devoirs en découlent. **Devoir de compétence :** déployer un outil que vous ne comprenez pas n'est pas neutre. Si vous ne pouvez pas dire où vont vos données, vous ne pouvez pas les protéger, et « nous ne savions pas » est une défense faible devant un régulateur, un client ou un tribunal. Le devoir de littératie dans la loi européenne sur l'IA, traité au [Chapitre 5](ch05-rules-and-legal-responsibility.md), le rend explicite. **Devoir de divulgation :** si vous êtes victime d'une violation, dites-le aux personnes touchées rapidement et clairement. Le cacher pour protéger votre réputation transfère le coût de votre problème sur les gens qui vous ont fait confiance ; les délais légaux sont au [Chapitre 10](ch10-privacy-and-gdpr.md). **Proportionnalité dans la surveillance :** journaliser l'usage de l'IA protège l'entreprise, et cela veut aussi dire lire ce que tape votre personnel. Fixez une politique écrite disant ce qui est journalisé, pourquoi, qui peut le voir, et pendant combien de temps. Surveillez le flux de données, pas la personne. La surveillance secrète abîme la confiance et enfreint souvent la loi locale.

Une dernière règle : n'utilisez pas d'outils d'IA pour attaquer d'autres systèmes, et ne testez pas vos propres défenses sur des données en production ou des comptes clients réels. Utilisez un environnement de test séparé.

## Erreurs à éviter

1. **Traiter un outil d'IA comme un moteur de recherche.** Un moteur de recherche indexe des pages publiques. Un service d'IA reçoit votre texte, le stocke, et le traite sur les ordinateurs de quelqu'un d'autre.
2. **Accorder des permissions larges « pour que ça marche ».** La commodité aujourd'hui est une violation demain. Accordez le minimum et n'élargissez que sur un besoin prouvé.
3. **Laisser une IA tout lire.** Pointer un assistant vers un lecteur partagé qui contient la paie, des dossiers juridiques et des dossiers clients transforme un compte compromis en exposition totale.
4. **Pas de journalisation.** Sans registres, vous ne pouvez pas découvrir ce qui s'est passé, ni prouver que vous aviez le contrôle.
5. **Accepter « de qualité entreprise » comme réponse.** Demandez plutôt : entraînez-vous sur mes données, combien de temps gardez-vous les prompts, qui sont vos sous-traitants, où sont stockées les données, me préviendrez-vous en cas de violation.
6. **Ignorer le plan grand public gratuit.** Du personnel sur des comptes personnels veut dire que vos données vont quelque part sans contrat et sans contrôles.
7. **Tout bloquer.** Une interdiction sans alternative approuvée n'arrête pas l'usage ; elle le cache.
8. **Confondre confidentialité et intégrité.** L'empoisonnement et la falsification ne sont pas des fuites. Ne protéger que contre la sortie de données et vous manquerez la corruption des données.
9. **Faire confiance à un fournisseur parce qu'il est gros.** La plus grande violation de paiement de la santé de l'histoire a commencé par un deuxième facteur de connexion manquant.
10. **Traiter la sécurité comme un projet ponctuel.** Les menaces, les outils et le personnel changent. Revoyez la carte chaque trimestre.

## Exercice pratique

### 6.9 Cartographiez vos points de vulnérabilité

Réservez quatre-vingt-dix minutes avec un collègue qui connaît le travail quotidien. Ne faites pas cela seul.

**Partie A — Listez les données (20 minutes).** Écrivez chaque catégorie d'information sensible que votre entreprise détient. Lignes typiques : noms et contacts clients, détails de paiement ou bancaires, numéros d'identité nationale ou fiscaux, dossiers employés et de paie, CV et données de candidats, informations de santé ou d'assurance, contrats et devis, code source ou dessins, stratégie et plans financiers.

**Partie B — Tracez chacun (40 minutes).** Pour chaque ligne, répondez par écrit à cinq questions :

1. Où vit-elle ? (système, dossier, tableur, papier)
2. Qui peut y accéder ? (rôles, personnes nommées, sous-traitants)
3. Quel outil d'IA y touche, le cas échéant ?
4. Quitte-t-elle notre bâtiment ? Où va-t-elle, et sous quel contrat ?
5. Pouvons-nous voir cela se produire ? (journalisation, oui ou non)

**Partie C — Notez et choisissez (30 minutes).** Marquez chaque ligne :

- **Rouge** — données sensibles qui quittent l'entreprise sans contrat et sans journalisation.
- **Ambre** — données sensibles qui restent à l'intérieur mais sont largement accessibles, ou qui partent sous un contrat que vous n'avez pas lu.
- **Vert** — données peu sensibles, ou données sensibles avec un contrat, un filtre et des journaux.

Chaque ligne rouge est une action pour ce mois-ci. Choisissez les cinq premières et écrivez un responsable et une échéance à côté de chacune. Un premier cinq typique : authentification à plusieurs facteurs sur les comptes fournisseurs, un outil d'IA approuvé pour le personnel, une règle de prévention des fuites pour les numéros d'identité, accès aux lecteurs partagés réduit aux dossiers dont chaque rôle a besoin, et une règle d'utilisation acceptable d'une page. Gardez la carte sur une seule page, et mettez-la à jour chaque trimestre et à chaque fois que vous ajoutez un nouvel outil d'IA.

## Liste de contrôle

### 6.10 Les 10 actions de sécurité minimales

- [ ] **Chaque compte a une authentification à plusieurs facteurs**, y compris les portails fournisseurs, l'email, la banque, le stockage cloud et les connexions d'administration.
- [ ] **Une carte écrite existe** de chaque outil d'IA en usage, quelles données entrent dans chacun, et où ces données sont stockées.
- [ ] **Un outil d'IA approuvé existe et est plus facile à utiliser** que les alternatives non approuvées.
- [ ] **Un filtrage en sortie est en place** pour les numéros d'identité et fiscaux, les détails de paiement, les données de santé, la paie, les contrats et le code source.
- [ ] **Aucun outil d'IA n'agit sur des instructions trouvées dans des documents qu'il lit** ; les actions ont besoin d'une confirmation humaine.
- [ ] **Chaque agent d'IA tourne avec le moindre privilège** : son propre compte, en lecture seule quand c'est possible, dépenses plafonnées, pas de droits d'administrateur.
- [ ] **Des journaux existent pour l'usage de l'IA, et quelqu'un les relit chaque semaine.**
- [ ] **Les actions irréversibles exigent une étape d'approbation humaine**, pas seulement une notification.
- [ ] **La diligence fournisseur est faite par écrit** : entraînement sur vos données, durée de rétention, sous-traitants, localisation des données, conditions de notification de violation.
- [ ] **Les sauvegardes sont testées et gardées hors ligne, et une solution de repli manuelle existe** pour tout processus qui dépend d'un fournisseur d'IA.

## Points à retenir

- L'IA rend les attaques moins chères et plus rapides, et elle multiplie le nombre de portes dans votre entreprise ; les deux changent à la fois.
- La fuite la plus courante n'est pas un piratage — c'est un employé serviable qui colle des données confidentielles dans un outil qu'il n'a jamais vérifié.
- Protégez les trois propriétés : confidentialité (données qui sortent), intégrité (données empoisonnées) et disponibilité (un fournisseur qui tombe).
- Les défenses de base sont une carte des données, une passerelle contrôlée unique, un filtrage en sortie, le moindre privilège pour les agents, et des journaux que quelqu'un lit vraiment.
- Votre risque inclut le risque de vos fournisseurs, et celui de leurs fournisseurs aussi ; demandez sur qui ils s'appuient avant de vous appuyer sur eux.
