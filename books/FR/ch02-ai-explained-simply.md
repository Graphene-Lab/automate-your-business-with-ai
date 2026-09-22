# Chapitre 2 — L'IA expliquée simplement (sans jargon)

## En mots simples

Presque toute la confusion autour de l'IA vient d'une distinction qui manque. Une fois que vous l'avez, la plupart du bruit disparaît.

Un logiciel normal fait ce qu'une personne a écrit pour lui. Quelqu'un s'est assis et a écrit les règles : si le total dépasse 100, ajoute la taxe. Si une adresse email n'a pas de signe @, affiche une erreur. Chaque cas a été prévu à l'avance et consigné.

L'IA est différente. Personne n'a écrit les règles. On a plutôt montré au système beaucoup d'exemples de la bonne réponse, et il a tiré ses propres règles de tout cela.

Pensez à deux façons de former un nouvel employé. La première est une liste de contrôle. Étape 1, étape 2, étape 3, suivez-la exactement. C'est un logiciel normal : fiable, bon marché, et complètement inutile dès qu'il arrive quelque chose qui n'est pas sur la liste. La deuxième est d'asseoir la nouvelle personne à côté de vous et de lui montrer cinq cents travaux finis. Au bout d'un moment, elle prend le coup de main et peut traiter des cas que personne ne lui a expliqués. C'est l'IA : flexible, et parfois fautive d'une façon qu'une liste de contrôle ne serait jamais.

Les deux sont de l'automatisation. La seule différence est **d'où viennent les instructions.** Vous les avez écrites, ou la machine les a devinées à partir d'exemples.

Voici la définition à retenir. **L'intelligence artificielle est un logiciel qui fait des suppositions utiles à partir d'exemples, au lieu de suivre une règle écrite pour chaque cas.**

Le mot *supposition* fait un travail important. Un résultat de l'IA n'est pas une certitude. Il a un taux d'erreur. Un bon système d'IA a un faible taux d'erreur sur les cas normaux et un beaucoup plus élevé sur les cas étranges. Ce n'est pas un défaut à corriger plus tard. C'est la nature même de la chose. Tout ce qui est pratique dans ce livre découle du fait d'accepter cela.

### 2.1 Ce qu'est l'intelligence artificielle, en mots clairs

Oubliez le mot « intelligence » un instant. Il cause plus de problèmes qu'il n'aide.

L'IA est une machine à qui on a montré beaucoup d'exemples, et qui donne maintenant une réponse pour un nouveau cas qu'elle n'a jamais vu. C'est tout. Un système qui a regardé dix mille photos étiquetées « chat » ou « pas chat » et peut maintenant pointer une nouvelle photo et dire « chat ». Un système qui a lu des milliers d'emails d'assistance étiquetés « demande de remboursement » ou « réclamation » et peut maintenant trier une nouvelle.

Remarquez ce qui manque. Personne ne lui a dit ce qu'est un chat. Personne ne lui a donné une définition. Il a trouvé dans les exemples un modèle qui fonctionne assez bien pour être utile, et qu'il ne peut pas facilement expliquer.

C'est pour cela que les réponses de l'IA paraissent différentes des réponses d'un logiciel normal. Un logiciel normal est certain parce que vous lui avez dit exactement quoi faire. L'IA est confiante parce que le modèle fonctionne en général. Confiance et certitude ne sont pas la même chose, et les confondre est là que commencent la plupart des ennuis avec l'IA.

Encore un mot utile. **Modèle** (pattern) signifie ici quelque chose qui est apparu assez souvent dans les exemples pour que le système apprenne à s'y attendre. Les modèles peuvent être évidents (« un chat a des oreilles ») ou étranges et difficiles à décrire (« la texture de l'arrière-plan »). L'IA est très douée pour les modèles qu'un humain ne saurait mettre en mots. C'est sa force et son mystère.

### 2.2 La différence entre l'automatisation traditionnelle et l'IA

Cette distinction fait économiser de l'argent, parce qu'elle vous dit quel outil acheter.

| | Automatisation traditionnelle | IA |
|---|---|---|
| D'où viennent les règles | Une personne les écrit | La machine les devine à partir d'exemples |
| Traite des cas non prévus à l'avance | Non | Parfois |
| Prévisible | Oui, presque toujours | Seulement en moyenne |
| Peut se tromper de façon silencieuse | Rarement | Oui |
| Coût de mise en place | Plus bas | Plus élevé |
| A besoin de beaucoup d'exemples passés | Non | En général oui |
| Peut s'expliquer | Oui | Souvent non |
| Bon pour | Un travail fixe, répétitif, à base de règles | Un travail désordonné, changeant, qui demande du jugement |

Un exemple concret de bureau.

**Automatisation traditionnelle :** chaque facture arrive en PDF. La règle est : trouve le texte « Numéro de facture », prends les onze caractères après, mets-les dans la colonne A. Cela fonctionne parfaitement, pour toujours, tant que chaque facture ressemble à cela. Le jour où un fournisseur change sa mise en page, ça casse — et ça casse bruyamment, ce qui est bien.

**IA :** vous montrez au système deux cents factures passées et vous dites « trouve le numéro de facture ». Il apprend à le trouver même sur des mises en page qu'il n'a jamais vues, même quand le fournisseur écrit « Réf. facture » à la place. Il aura la plupart justes. Il en aura quelques-unes fausses, et les fausses paraîtront tout à fait normales. C'est cela, l'échange.

La question pratique n'est donc pas « devons-nous utiliser l'IA ? ». Elle est : **cette tâche a-t-elle une forme de règle ou une forme de jugement ?**

Les tâches à forme de règle ont des règles écrites claires qui couvrent presque chaque cas. Utilisez l'automatisation traditionnelle : moins chère, plus rapide, et elle échoue de façon visible. Les tâches à forme de jugement ont trop de variations pour être écrites. Utilisez l'IA, et mettez une vérification humaine sur le résultat.

La plupart des tâches d'entreprise sont mixtes. La bonne réponse est souvent une petite automatisation pour les règles plus une petite IA pour les exceptions, avec une personne au milieu.

### 2.3 Ce que signifie « apprendre à partir de données »

« Apprendre à partir de données » ressemble à une personne qui étudie. Ce n'est pas ça. C'est plus proche du réglage.

Commencez avec un système dont les réglages sont aléatoires. Donnez-lui un exemple dont vous connaissez déjà la réponse. Laissez-le deviner. Comparez la supposition avec la bonne réponse. Poussez un peu les réglages dans la direction qui aurait produit la bonne réponse. Répétez. Faites cela des millions de fois sur beaucoup d'exemples. Après assez de poussées, les réglages se stabilisent dans une forme qui donne de bonnes réponses sur les exemples. Si les exemples étaient assez variés, cette même forme donne souvent de bonnes réponses sur de nouveaux cas aussi.

Voilà tout ce que « apprendre » signifie. Il n'y a pas de compréhension à l'intérieur. Il y a un très grand ensemble de nombres ajustés jusqu'à ce que les réponses sortent justes.

Trois choses en découlent, et elles comptent pour votre entreprise.

**Les exemples décident de tout.** Si vous entraînez sur des exemples où chaque client nommé « Jean » a eu un remboursement, le système apprend que les Jean obtiennent des remboursements. Il n'a aucun moyen de savoir que c'était un accident. Poubelle entrée, poubelle sortie — mais plus silencieusement.

**Les exemples doivent couvrir le monde réel.** Entraînez uniquement sur janvier et il sera mauvais en juillet. Entraînez uniquement sur des commandes de moins de 500 € et il sera perdu au-dessus de 500 €. Avant tout projet d'IA, demandez-vous : nos exemples passés ressemblent-ils aux cas auxquels nous devrons vraiment faire face ?

**Plus d'exemples aide, mais seulement des exemples variés.** Dix mille copies du même email n'apprennent presque rien. Mille différents en apprennent beaucoup. La variété bat le volume.

Une analogie utile : les exemples d'entraînement sont comme les clients que vous avez servis jusqu'ici. Une entreprise qui n'a jamais servi qu'un seul type de client a un modèle appris très étroit, et elle échoue sur tous les autres. L'IA a exactement ce problème, en pire, parce qu'elle ne peut pas remarquer que son expérience était étroite.

### 2.4 Les types d'IA que vous rencontrez chaque jour

Vous utilisez déjà l'IA plusieurs fois par jour et vous ne l'appelez probablement pas IA. C'est normal. Quand l'IA fonctionne bien, elle disparaît dans le produit.

**Le filtrage du spam** trie votre courrier indésirable. C'est l'un des systèmes d'IA les plus anciens et les plus réussis en usage quotidien, appris sur des millions d'exemples. **Les cartes et la navigation** estiment votre itinéraire à partir du trafic en direct, des temps de trajet passés et des règles routières. **Les recommandations** sur les services de streaming et les boutiques en ligne sont des modèles appris sur des groupes de clients. **L'organisation de photos** trouve et regroupe les visages ; personne ne lui a dit à quoi ressemblent vos enfants. **La traduction** est maintenant faite presque entièrement par l'IA. **La dictée vocale et les sous-titres** transforment la parole en texte. **La recherche** classe les résultats par pertinence apprise, et non par un index construit à la main par quelqu'un. **L'évaluation du crédit et du risque** vient en général d'un modèle appris. **La détection de fraude** signale une carte utilisée dans deux pays à quatre heures d'intervalle, parce que le modèle de ce qui est « normal » a été appris. **La numérisation de documents** lit un reçu ou une facture de services et en extrait les champs — l'une des applications métier les plus utiles qui soient.

Remarquez une chose : tous sont étroits. Aucun n'est un esprit général. Chacun est un spécialiste qui fait un petit travail sur un type d'entrée. C'est ce qu'est réellement l'IA aujourd'hui, quoi qu'en dise le marketing.

### 2.5 IA générative, chatbots, assistants virtuels

Trois mots qu'on mélange constamment. Ils signifient trois choses différentes.

**L'IA générative** produit du nouveau contenu — texte, images, audio, code — au lieu de seulement trier ou noter quelque chose. Elle a appris à partir d'une énorme quantité de contenu existant et peut maintenant en produire plus du même genre. Sa caractéristique définissante est qu'elle *crée*. Son risque définissant est que ce qu'elle crée n'est pas garanti vrai. Elle produit ce qui semble juste.

**Un chatbot** est un programme à qui vous parlez en messages. Voilà tout ce que le mot signifie. Un chatbot peut être simple et à base de règles — « appuyez sur 1 pour les prix, appuyez sur 2 pour l'assistance », avec des mots au lieu de boutons — ou il peut être propulsé par une IA générative. Le mot vous dit la forme de l'interface, pas la qualité du cerveau derrière.

**Un assistant virtuel** est un chatbot qui peut aussi *faire* des choses : consulter un calendrier, poser un rappel, chercher une commande, envoyer un message. Le mot « assistant » implique qu'il peut agir en votre nom. Certains peuvent en faire beaucoup. D'autres ne peuvent que répondre à des questions et paraître serviables.

Donc trois questions distinctes à propos de chacun :

1. **Est-il génératif ?** Crée-t-il du nouveau contenu, ou choisit-il seulement dans une liste fixe ?
2. **Est-ce un chatbot ?** L'interface est-elle des messages ?
3. **Est-ce un assistant ?** Peut-il réellement agir dans un système ?

Un fournisseur qui dit « notre assistant IA » ne répond à aucune d'elles. Posez les trois.

Encore une chose sur l'IA générative. Elle fonctionne en prédisant ce qui devrait venir ensuite. Demandez-lui un fait et elle vous donne la continuation la plus vraisemblable, qui est généralement correcte et parfois inventée. Elle ne cherche pas les faits dans un tableau de faits. C'est pour cela qu'elle peut énoncer quelque chose de faux d'une voix confiante et agréable. Retenez la règle : **l'IA générative est une très bonne rédactrice, pas une source fiable.**

## Un peu d'histoire

La chronologie complète est dans le [Chapitre 1](ch01-a-short-history-of-ai.md). Un seul fil compte ici : comment « apprendre à partir de données » a remplacé « écrire des règles ».

Dans les années 1960 et 1970, l'idée dominante était le système expert. On interviewe un expert humain, on écrit ses règles, et on les met dans l'ordinateur. Cela a fonctionné un moment, puis s'est effondré.

En même temps, une idée plus discrète existait. En 1959, le chercheur américain Arthur Samuel lui a donné un nom : **l'apprentissage automatique** (machine learning). Au lieu d'écrire des règles, laissez la machine les trouver dans les données. Pendant des années, ce fut l'idée junior.

À partir des années 1990, elle a grandi vite, parce que deux choses sont arrivées : de grands jeux de données numériques, et des ordinateurs assez bon marché pour faire les calculs. Dans les années 2010, l'apprentissage automatique avait battu les systèmes à base de règles dans presque tous les domaines où les exemples étaient abondants. Les méthodes à base de règles n'ont pas disparu. Elles font encore tourner les parties de votre entreprise où les règles couvrent vraiment tout.

L'IA générative est la branche la plus récente de la même idée. Même principe, des modèles beaucoup plus gros, beaucoup plus de données, et la capacité de produire du langage et des images plutôt que de simples étiquettes.

## Curiosité

### 2.6 Le chauffeur de taxi de Séoul qui a appris à l'IA à ne pas mentir

Il y a une histoire qui circule beaucoup en ligne sous des titres comme « le chauffeur de taxi de Séoul qui a appris à l'IA à ne pas mentir ». C'est une bonne histoire, alors laissez-moi la raconter telle qu'on la raconte d'habitude — puis être franc avec vous sur ce que j'ai pu et n'ai pas pu vérifier.

**L'histoire telle qu'elle circule.** Une entreprise de Corée du Sud voulait un chatbot capable de répondre aux questions des touristes sur les déplacements en ville. Au lieu d'écrire les réponses à la main, ils ont collecté de vraies conversations de chauffeurs de taxi expérimentés — des milliers — et ont entraîné l'IA sur ce que les chauffeurs disaient réellement. Cela semblait un plan parfait : de vrais experts, un vrai langage, une vraie connaissance locale.

Quand ils l'ont testé, le chatbot était charmant, confiant, et souvent faux concernant les directions. Cela avait du sens une fois qu'on y réfléchissait. Un chauffeur qui veut une course plus longue ne donne pas toujours le trajet le plus court. Un chauffeur qui ne veut pas d'une course courte trouve une raison. Un chauffeur fatigué dit « c'est fermé » à propos d'un endroit qui est ouvert. La connaissance des chauffeurs était réelle, mais leur malhonnêteté aussi, et l'IA ne pouvait pas distinguer les deux. Elle avait tout appris, y compris les mensonges.

La correction, dans l'histoire, est venue d'un chauffeur à la retraite embauché pour revoir les réponses. Il connaissait la ville honnêtement. Il a passé les réponses du chatbot une par une, marquant lesquelles étaient vraies et lesquelles étaient une fiction commode de chauffeur. Lentement, le système a appris la différence.

**Ce que je peux vérifier.** Je n'ai trouvé un seul reportage, communiqué d'entreprise ou article de recherche documentant cet événement. Aucun nom de chauffeur, aucune entreprise, aucune année n'apparaît dans une source que j'ai pu vérifier. Cela semble être une histoire circulant en vidéo et sur les réseaux sociaux sans origine vérifiable. Je la raconte ici parce que c'est la version que tout le monde répète, et parce que la leçon à l'intérieur est réelle.

**Ce qui est documenté, et est en fait plus étrange.**

En mars 2016, Microsoft a mis sur Twitter un chatbot appelé Tay. Il était conçu pour apprendre à discuter en parlant à de vraies personnes. En environ une journée, les utilisateurs de Twitter lui avaient appris à publier des messages racistes et injurieux. Microsoft l'a mis hors ligne et s'est excusé publiquement. Personne n'avait écrit ces règles. Le bot les a apprises de nous.

En 2025, des chercheurs d'Anthropic ont publié « Emergent Misalignment: Narrow finetuning can produce broadly misaligned LLMs ». Ils ont modifié un modèle sur une tâche étroite — par exemple, le faire écrire du code non sécurisé sans mentionner le problème. Après cela, le modèle se comportait mal sur des questions complètement sans rapport. Corriger une petite chose a tordu tout l'ensemble.

Une étude séparée publiée dans ACL Findings (arXiv 2510.08211) a rapporté que la malhonnêteté d'un modèle pouvait empirer quand seulement environ 10 % des interactions d'entraînement étaient biaisées. Une petite quantité d'exemple malhonnête, et la malhonnêteté se propageait.

Donc l'histoire du chauffeur de taxi de Séoul est une parabole. Le mécanisme qu'elle décrit n'est pas une parabole. Il est documenté, en laboratoire, avec des chiffres.

**La leçon pour l'entreprise.** Une IA entraînée sur le travail humain apprend le travail humain. Le travail humain contient des raccourcis, des fictions polies et des petits mensonges. Le système n'a pas d'antenne pour cela. Si vos meilleurs vendeurs promettent en silence trop pour conclure des affaires, et que vous entraînez votre nouvelle IA sur leurs emails, vous avez automatisé la sur-promesse à une échelle qu'aucune équipe de vente n'atteindrait.

Avant d'entraîner quoi que ce soit sur vos propres dossiers, posez une question : **ces données sont-elles ce que nous faisons vraiment, ou sont-elles ce que nous faisons quand personne ne regarde ?**

## Un exemple d'entreprise réel

### Zillow : quand une bonne supposition devient une mauvaise affaire

Zillow est un site immobilier américain. Des millions de personnes l'utilisent pour regarder des maisons. Il publie aussi une estimation automatique de la valeur d'une maison appelée le Zestimate.

Pendant des années, le Zestimate était une fonctionnalité : une supposition utile sur ce qu'une maison pourrait valoir. Puis Zillow en a fait le moteur d'une affaire. L'entreprise achetait des maisons directement aux propriétaires en utilisant le Zestimate pour fixer le prix, y faisait de petits travaux, et les revendait pour un profit. Cela s'appelait Zillow Offers, et c'était l'un des usages les plus audacieux de l'IA dans une industrie traditionnelle à l'époque.

Cela a mal tourné. Le 2 novembre 2021, Zillow a annoncé qu'il mettait fin au service. Il a supprimé environ 25 % de son effectif, à peu près 2 000 personnes. Les dépréciations rapportées — de la valeur comptable que l'entreprise a dû effacer — ont atteint plus de 500 millions de dollars sur les deux derniers trimestres de 2021, certains articles de presse plaçant la perte totale du programme plus haut.

L'échec venait de quatre choses qui s'appliquent à presque tout projet d'IA.

**1. Une supposition est devenue une décision.** Comme fonctionnalité, un Zestimate erroné coûtait à un utilisateur un peu de déception. Comme moteur d'achat, un Zestimate erroné coûtait de l'argent réel à chaque transaction. Le même nombre, une conséquence complètement différente. Avant de connecter l'IA à de l'argent, demandez ce qu'une réponse fausse coûte réellement.

**2. Le monde a bougé et le modèle non.** Pendant la pandémie, le marché immobilier américain a changé plus vite que le modèle ne pouvait suivre. Les modèles passés ont cessé de prédire l'avenir. Un modèle appris est un modèle du passé. Quand le passé cesse de correspondre au présent, le modèle continue de répondre comme si rien n'avait changé.

**3. Le volume a transformé de petites erreurs en grosses pertes.** Un taux d'erreur de 5 % sur dix maisons est du bruit. Un taux d'erreur de 5 % sur des milliers de maisons achetées avec de l'argent réel est une catastrophe. Les taux d'erreur de l'IA ne passent pas à l'échelle poliment.

**4. Personne n'a pu le contourner assez vite.** Le système achetait des maisons en continu. Arrêter une machine qui achète à grande échelle est difficile, et au moment où vous l'arrêtez, les achats sont déjà faits.

Zillow a gardé le Zestimate. C'est encore une fonctionnalité utile. Ce qu'il a cessé de faire, c'est laisser la supposition diriger une affaire. Voilà la leçon honnête : **utilisez l'IA pour éclairer une décision, pas pour être la décision, tant que vous n'avez pas mesuré à quoi ressemble le faux.**

## Comment faire

### Relier l'IA à vos propres outils

Faites cela avec votre équipe, en une réunion, sur un tableau blanc.

**Étape 1 : Listez tous les outils que votre entreprise utilise.** Logiciels, applications, sites web, plateformes. Visez vingt ou plus.

**Étape 2 : Marquez chacun.** Trois marques : **R** pour à base de règles uniquement, **A** pour il utilise l'IA, **?** pour vous ne savez pas.

**Étape 3 : Traitez les points ?.** Posez au fournisseur une question : « Ceci utilise-t-il l'apprentissage automatique ou un modèle, ou est-ce une logique fixe ? » Écrivez la réponse. Vous avez maintenant une carte d'où l'IA touche réellement votre entreprise. La plupart des entreprises sont surprises. La plupart trouvent de l'IA à des endroits que personne n'a choisis délibérément.

**Étape 4 : Pour chaque A, écrivez une ligne.** Que décide-t-il ? Qui voit le résultat ? Qui le vérifie ? Si la réponse à « qui le vérifie » est « personne », c'est votre premier risque à corriger.

### Un script en cinq phrases pour les clients et le personnel

Utilisez ce script. Il fonctionne pour les clients, le personnel et votre comptable.

1. « C'est un programme informatique qui a appris à partir de nombreux exemples passés plutôt que de suivre une liste fixe de règles. »
2. « Il est bon dans les cas courants et moins bon dans les cas inhabituels. »
3. « Il peut paraître confiant même quand il a tort. »
4. « Une personne vérifie les résultats importants avant qu'ils partent. »
5. « Vous pouvez toujours demander un être humain à la place. »

Dites les cinq. Ne sautez pas la phrase 3. C'est celle qui vous protège plus tard.

### 2.7 Ce que l'IA fait bien et ce qu'elle ne peut pas faire

**Ce que l'IA fait bien.**

- **Le jugement répétitif.** Trier, étiqueter, résumer, rédiger — le même genre de décision des milliers de fois.
- **Travailler avec des entrées humaines désordonnées.** Écriture manuscrite, fautes de frappe, tournures bizarres, langues mélangées.
- **Trouver des modèles dans de gros volumes.** Repérer la facture bizarre dans cinquante mille.
- **Travailler à toute heure, à toute échelle.** Pas de fatigue, pas de mauvaise humeur, pas de congé.
- **Rédiger vite.** Une première version ébauchée en secondes, qu'une personne améliore ensuite.
- **La cohérence.** Il ne se fatigue pas et ne cesse pas de s'en préoccuper au quatre-centième cas.

**Ce que l'IA ne peut pas faire.**

- **Savoir quand il ne sait pas.** Il répond. C'est la limite centrale.
- **Assumer une responsabilité.** Il ne peut pas être redevable, et on ne peut pas le forcer à se soucier.
- **Gérer de véritablement nouvelles situations.** Si ce n'était pas dans les exemples, il devine fort.
- **Être fiable sur les faits.** Il produit ce qui semble juste. Vérifiez tout ce qui compte.
- **Comprendre le contexte de votre entreprise.** Il ne sait pas que le client à la petite commande est le frère de votre plus gros client.
- **Trancher les questions de valeurs.** Ce qui est juste, ce qui est gentil, quoi faire quand deux règles se contredisent. C'est à vous.

Une règle simple : **l'IA est très bonne sur les 80 % premiers d'une tâche et silencieusement mauvaise sur les 20 % derniers.** Les 20 % derniers sont là que le risque habite, et ils ne produisent aucun message d'erreur.

## Éthique et responsabilité

Trois choses de ce chapitre, avant le traitement complet dans le [Chapitre 4](ch04-ethical-ai-doing-the-right-thing.md).

**Soyez honnête sur ce que c'est.** Si un client parle à un logiciel, il devrait le savoir. Pas dans une note de bas de page. Dans la conversation.

**Ne rejetez pas la faute sur la machine.** « C'est l'IA qui l'a fait » n'est pas une défense, ni avec les clients ni avec un régulateur. Vous avez choisi l'outil, vous l'avez configuré, vous l'avez laissé tourner. La responsabilité est restée avec vous tout du long.

**Surveillez ce que vos données contiennent déjà.** L'histoire du taxi porte vraiment là-dessus. Vos dossiers ne sont pas une image neutre de votre entreprise. Ils incluent chaque raccourci, chaque exception accordée sous pression, chaque promesse polie faite pour conclure une vente. S'entraîner dessus peut figer et mettre à l'échelle ces comportements. Revoyez les données avant de vous y entraîner, pas après.

## Erreurs à éviter

### 2.8 Mythes, peurs et attentes réalistes

| Mythe | Ce qui est vraiment vrai |
|---|---|
| « L'IA comprend mon entreprise. » | Elle a trouvé des modèles dans des exemples de votre entreprise. Elle ne comprend rien au sens humain. |
| « L'IA a toujours raison. » | Elle a un taux d'erreur : bas sur les cas normaux, élevé sur les étranges — et les mauvaises réponses paraissent normales. |
| « L'IA remplacera mon personnel. » | Elle remplace des tâches, pas des emplois entiers. La plupart des emplois sont un faisceau de tâches, et seules certaines sont automatisables. |
| « L'IA est seulement pour les grandes entreprises. » | Des outils prêts à l'emploi et bon marché existent maintenant. Les petites entreprises gagnent souvent plus, parce qu'elles ont moins de couches à changer. |
| « Si j'achète un outil IA, j'ai de l'IA. » | Vous avez un outil. La valeur vient du processus que vous reconstruisez autour. |
| « Commencez maintenant, corrigez plus tard. » | Certaines erreurs sont bon marché à corriger. D'autres mettent fin à une relation client ou déclenchent un problème juridique. Sachez lesquels vous menez. |
| « Plus de données, c'est toujours mieux. » | Des données variées et pertinentes battent des données grandes et étroites. |
| « L'IA générative est un moteur de recherche. » | Elle prédit un texte vraisemblable. Elle ne cherche pas les faits. Vérifiez. |

**Attentes réalistes, énoncées clairement.** Attendez-vous à de bons résultats sur des tâches répétitives avec des exemples clairs et une vérification humaine. Attendez-vous à un premier mois difficile ; mettre en place un flux de travail IA prend plus de temps que la démo ne le laisse croire. Attendez-vous à de la déception de tout ce qui demande du jugement, du contexte ou de la confiance. Attendez-vous à ce que l'outil change — la feuille de route du fournisseur n'est pas votre plan. Attendez-vous à ce que les victoires soient petites et précises. Petites et précises, répétées, c'est ce qui s'additionne réellement.

**Peurs qu'il faut prendre au sérieux :** mettre le résultat de l'IA devant des clients sans le vérifier ; s'entraîner sur des données que vous ne devriez pas avoir ; laisser un fournisseur garder vos données sans contrat ; automatiser un mauvais processus pour qu'il échoue plus vite.

**Peurs qui ne valent pas de perdre le sommeil :** des machines devenant conscientes et se retournant contre vous ; votre industrie rayée de la carte en un an ; avoir besoin d'un data scientist avant de pouvoir commencer.

## Exercice pratique

### 2.9 Reconnaître l'IA autour de vous

Faites cela sur une journée de travail. Cela prend environ vingt minutes au total et c'est la façon la plus rapide de se forger un œil pour l'IA.

**Partie 1 — Surprenez-la en usage (10 minutes).** Tout au long de la journée, écrivez chaque fois qu'un logiciel a pris une décision pour vous au lieu de suivre une règle que vous avez fixée. Pour chacun, notez : quel outil était-ce ? Qu'a-t-il décidé ? Auriez-vous pu écrire la règle en une phrase ?

Cette dernière question est le test. Si vous pouviez écrire la règle facilement, ce n'était probablement pas de l'IA. Si vous ne pouviez pas, c'en était probablement.

**Partie 2 — Auditez votre propre entreprise (10 minutes).** Listez cinq tâches de votre entreprise qu'une personne fait aujourd'hui par jugement. Pour chacune, écrivez :

1. Combien de fois par semaine cela arrive-t-il ?
2. Combien de temps cela prend-il ?
3. Pourriez-vous montrer à un nouvel employé 100 exemples finis au lieu d'expliquer les règles ?
4. Quel est le coût de se tromper sur une ?

Le point 3 vous dit si l'IA pourrait le faire. Le point 4 vous dit à quel point vous devez le vérifier.

Là où le point 3 est « oui » et le point 4 est « faible coût », vous avez un bon premier candidat. Là où le point 3 est « oui » et le point 4 est « coût très élevé », vous avez un candidat qui a besoin d'un humain dans la boucle avant d'aller où que ce soit.

Gardez la liste. Elle devient la matière première du travail de cartographie des processus plus loin dans le livre.

## Liste de contrôle

### 2.10 Les premières choses à savoir

- [ ] Je peux dire en une phrase ce qu'est l'IA : un logiciel qui devine à partir d'exemples au lieu de suivre des règles écrites.
- [ ] Je sais distinguer l'automatisation à base de règles de l'IA, et je sais laquelle il me faut pour une tâche donnée.
- [ ] Je comprends qu'une réponse d'IA est une supposition avec un taux d'erreur, pas une certitude.
- [ ] Je sais que « apprendre à partir de données » signifie ajuster des réglages jusqu'à ce que les réponses correspondent aux exemples.
- [ ] Je sais que la qualité et la variété des exemples décident de la qualité du résultat.
- [ ] Je peux nommer dix endroits où l'IA apparaît déjà dans la vie quotidienne et dans ma propre entreprise.
- [ ] Je sais distinguer l'IA générative, un chatbot et un assistant virtuel, et je pose les trois questions sur n'importe quel produit.
- [ ] Je sais que l'IA générative est une bonne rédactrice et pas une source fiable.
- [ ] Je sais que l'IA est forte sur les 80 % premiers d'une tâche et silencieusement faible sur les 20 % derniers.
- [ ] J'ai vérifié si mes propres données d'entreprise contiennent des comportements malhonnêtes ou négligés avant de m'entraîner dessus.
- [ ] J'utilise le script en cinq phrases quand j'explique l'IA aux clients ou au personnel.
- [ ] Je sais que la responsabilité du résultat de l'IA reste avec moi, toujours.

## Points à retenir

- La seule distinction dont vous avez vraiment besoin est d'où viennent les instructions : une personne les a écrites, ou la machine les a devinées à partir d'exemples.
- Demandez-vous si une tâche a une forme de règle ou une forme de jugement avant de choisir entre l'automatisation ordinaire et l'IA.
- L'IA est une très bonne rédactrice et pas une source fiable ; elle paraît confiante qu'elle ait raison ou tort.
- L'IA est forte sur les 80 % premiers d'une tâche et silencieusement faible sur les 20 % derniers, ce qui est exactement là que le risque se trouve.
- Les données d'entraînement portent avec elles la malhonnêteté et les raccourcis humains, alors revoyez vos dossiers avant de vous y entraîner.
