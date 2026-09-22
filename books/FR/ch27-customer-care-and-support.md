# Chapitre 27 — Relation client et assistance

## En mots simples

La relation client est l'endroit où une entreprise prouve qu'elle se soucie. Quand quelque chose tourne mal ou qu'un client a une question, la vitesse et la qualité de votre réponse façonnent s'il reste ou part. Le problème est que l'assistance est pleine des mêmes questions posées encore et encore, et une petite équipe ne peut pas y répondre instantanément. L'IA aide en répondant aux courantes immédiatement et en routant les dures vers la bonne personne vite.

Pensez à l'assistance comme à une file d'attente. Chaque question fait la queue en attendant une réponse. Plus la file est longue, plus les gens s'énervent. L'IA raccourcit la file de deux façons : elle répond à certaines questions avant qu'elles n'atteignent un humain, et elle trie le reste pour que la bonne personne voie le bon problème en premier.

Ce chapitre couvre quatre métiers : les chatbots et FAQ qui répondent aux questions courantes, la gestion de tickets qui trie et route les problèmes, l'analyse de sentiment qui lit ce que ressentent les clients, et une base de connaissances intelligente qui garde toutes les réponses dans un seul endroit consultable.

Une idée honnête d'abord : le but de l'IA dans l'assistance n'est pas de cacher les clients à vos gens. C'est de libérer vos gens des questions répétitives pour qu'ils puissent passer leur temps sur les cas qui ont vraiment besoin d'un humain — le client en colère, le problème complexe, celui qui décide si quelqu'un reste dix ans. L'IA gère le volume ; les humains gèrent le soin. La méthode pour juger si cela rapporte vit dans le [Chapitre 16 — Objectifs, coûts et retour sur investissement](ch16-goals-costs-and-return-on-investment.md) ; ce chapitre vous montre quoi automatiser et comment.

## Un peu d'histoire

**Années 1960-1980 : le centre d'appels.** L'assistance client signifiait le téléphone. Un client appelait, attendait en ligne, et parlait à un agent. Toute la discipline consistait à avoir assez de personnel pour répondre au téléphone. Cela fonctionnait, mais c'était cher, lent, et ne passait à l'échelle qu'en embauchant plus de gens.

**Années 1990 : l'email et le ticket.** L'assistance s'est en partie déplacée vers l'email, et le « ticket » est né — chaque demande client devenait un enregistrement numéroté qui pouvait être suivi, assigné et fermé. Les tickets ont mis de l'ordre dans le chaos des emails d'assistance. Des outils comme les premiers logiciels d'aide technique (helpdesk) ont permis de voir chaque demande ouverte au même endroit.

**Années 2000 : la base de connaissances et le libre-service.** Les entreprises ont réalisé que la plupart des questions d'assistance étaient les mêmes quelques questions. Elles ont construit des bases de connaissances — des bibliothèques consultables de réponses — pour que les clients se débrouillent seuls. Le libre-service a enlevé une partie de la charge des agents, mais les premières bases de connaissances étaient difficiles à chercher et manquaient souvent ce dont le client avait besoin.

**Années 2010 : le chat et le chatbot à base de règles.** Le chat en direct est arrivé, et avec lui le chatbot. Les premiers chatbots étaient à base de règles : un arbre de décision qui faisait correspondre des mots-clés à des réponses préécrites. Ils étaient bon marché mais frustrants — ils ne pouvaient rien comprendre qui sortait du script, et les clients se sentaient souvent piégés.

**Fin des années 2010 : l'IA lit le sentiment.** L'apprentissage automatique a commencé à lire le *ton* d'un message — si un client était content, frustré ou en colère — et pouvait signaler un client en colère pour qu'un agent senior réponde en premier. L'analyse de sentiment a ajouté un nouveau signal au routage : non seulement quel est le problème, mais comment le client le ressent.

**Années 2020 : grands modèles de langage et assistance agentique.** Les grands modèles de langage — IA entraînée sur d'énormes quantités de texte — ont fait des chatbots qui comprennent réellement ce qu'un client a tapé et répondent en langage simple. La dernière étape est la plateforme agentique : une IA qui non seulement répond mais prend des actions — créer un ticket, mettre à jour un enregistrement, planifier un service. L'exemple TridentCare ci-dessous est exactement cela : une IA qui gère le travail de planification de bout en bout, avec des humains n'intervenant que quand le jugement est nécessaire.

L'arc : des files de téléphone, aux tickets suivis, aux réponses consultables, aux bots qui comprennent, aux agents qui agissent. Chaque étape a déplacé le travail de routine vers le logiciel et a laissé les agents humains libres pour les cas qui ont besoin d'un humain.

## Curiosité

### 27.5 Le répartiteur qui a laissé le système faire le travail

Dans l'ancienne façon de travailler de TridentCare, environ la moitié de toute la planification se faisait à la main — une personne faisant correspondre la demande d'un patient à un technicien, une heure et un lieu. Après que l'entreprise est passée à une plateforme propulsée par l'IA, la planification manuelle est tombée à seulement 4,3 %. Les répartiteurs n'ont pas disparu ; ils ont changé de travail. Ils ont cessé de faire la correspondance eux-mêmes et ont commencé à la superviser, n'intervenant que quand un cas avait vraiment besoin du jugement humain. Ce changement — de faire le travail à superviser le travail — est la révolution silencieuse dans l'assistance et les opérations. L'histoire complète est ci-dessous.

## Un exemple d'entreprise réel

**TridentCare : 96 % d'automatisation de la planification avec un CRM propulsé par l'IA.**

TridentCare est le plus grand fournisseur de services portables de diagnostic médical aux États-Unis. Il envoie des techniciens dans les hôpitaux, les maisons de retraite et les domiciles de patients pour effectuer des examens comme des radiographies et des échographies — des services qui ne peuvent pas attendre et doivent être planifiés de façon fiable sur une immense zone. Planifier ce travail à la main, sur des centaines de marchés, était lent et difficile à mettre à l'échelle.

Selon un communiqué de presse de ServiceNow (relayé par Business Wire le 22 avril 2026), TridentCare a sélectionné la plateforme IA de ServiceNow pour transformer ses opérations de bout en bout et largement remplacer la planification manuelle par l'automatisation. Les résultats rapportés :

- **96 % d'automatisation de la planification sur 127 marchés.** La planification manuelle des services portables de diagnostic médical est tombée de **50 % à seulement 4,3 %**. En d'autres termes, le système gère maintenant presque toute la planification, et une personne n'intervient que quand le jugement l'exige vraiment.
- **Les temps d'attente des patients au-delà du niveau de service convenu (SLA) ont été réduits de 57 %.** Un SLA est le niveau de service promis — par exemple, « un technicien arrive dans les deux heures ». Moins de patients ont attendu plus longtemps que promis.
- **L'efficacité sur le premier marché s'est améliorée d'environ 30 %.** L'entreprise en a fait plus dans les marchés où elle a commencé.

Le communiqué de presse décrivait aussi une transformation « lead-to-cash » (du prospect à l'encaissement) : en connectant directement le CRM de ventes aux données de performance sur le terrain, TridentCare a gagné la visibilité pour fixer des niveaux de service exacts, voir où la demande se déplaçait, et affûter la façon dont il vendait.

Deux leçons ressortent. D'abord, le rôle humain est passé de *faire* à *superviser* : les répartiteurs laissaient le système gérer la routine et n'intervenaient que pour les exceptions. Ensuite, la victoire n'était pas seulement la vitesse — c'était la fiabilité et le soin aux patients. Dans une entreprise où un technicien en retard affecte la santé d'un patient, une automatisation qui réduit les temps d'attente n'est pas juste une économie de coût ; c'est un meilleur service.

Une note sur la source : les chiffres ci-dessus viennent de l'annonce publiée de ServiceNow. Traitez-les comme les résultats déclarés de TridentCare ; vos propres chiffres dépendront de votre exploitation et de votre volume.

## Comment faire

### 27.1 Chatbots et FAQ

Un chatbot sur votre site web ou application peut répondre instantanément aux questions d'assistance courantes, pour que les clients n'aient pas à attendre une personne. Une page FAQ (Foire Aux Questions) est la cousine plus simple : une liste de questions courantes avec des réponses écrites.

**Ce qu'un chatbot devrait gérer.** Les questions répétitives, à faible risque : « Quels sont vos horaires ? », « Comment réinitialiser mon mot de passe ? », « Où est ma commande ? », « Quelle est votre politique de retour ? ». Ce sont les questions qui dévorent la plupart du temps d'une équipe d'assistance et n'ont besoin d'aucun jugement. Laissez le bot y répondre.

**Les bots modernes comprennent le langage.** Contrairement aux anciens bots à menu, un chatbot construit sur un grand modèle de langage comprend ce qu'un client tape et répond en mots simples. Il peut gérer « je n'arrive pas à me connecter, il dit mot de passe erroné » sans que le client ait à choisir dans une liste.

**Le passage de relais est tout.** Un chatbot qui ne peut pas répondre doit passer la conversation à un humain, avec le contexte intact — l'humain devrait voir ce que le client a déjà dit, pas repartir de zéro. Décidez les règles de passage de relais avant de construire : quand le bot n'est pas sûr, quand le client demande une personne, quand le sujet est sensible. Un bot qui connaît ses limites est digne de confiance ; un qui bluffe ne l'est pas.

**Gardez la FAQ vivante.** Une page FAQ périmée est pire que pas du tout — elle donne de fausses réponses avec assurance. Revoyez-la régulièrement et mettez-la à jour à mesure que vos produits et politiques changent. Le chatbot et la FAQ devraient puiser dans la même source de vérité (voir la base de connaissances ci-dessous).

**Mesurez la résolution et l'échec.** Suivez combien de questions le bot résout seul et combien il passe. Les échecs vous disent quoi lui apprendre ensuite. (La même technologie de chatbot, appliquée aux ventes plutôt qu'à l'assistance, est couverte dans le [Chapitre 26 — Ventes et marketing](ch26-sales-and-marketing.md).)

### 27.2 Gestion de tickets

Un *ticket* est un enregistrement numéroté d'une demande client. La gestion de tickets signifie trier chaque demande, l'assigner à la bonne personne, suivre sa progression, et la fermer quand elle est résolue. Quand le volume est élevé, une bonne gestion de tickets est la différence entre une équipe d'assistance organisée et une chaotique.

**L'IA trie et route.** Au lieu qu'une personne lise chaque ticket et décide qui devrait le traiter, l'IA lit le ticket et le route automatiquement vers la bonne équipe ou le bon agent, selon le sujet, l'historique du client et l'urgence. Cela économise l'étape de triage, qui est une pure charge.

**Prioriser par urgence et ressenti.** L'IA peut classer les tickets pour que les clients les plus urgents et les plus contrariés soient vus en premier. Un client dont le service est complètement en panne, ou qui est clairement en colère, ne devrait pas attendre derrière une question de routine. Combiner l'urgence avec le sentiment (voir ci-dessous) rend la file plus intelligente.

**Suggérer la réponse.** L'IA peut lire un ticket et suggérer une réponse, ou pointer l'agent vers l'article de la base de connaissances qui le résout. L'agent relit et envoie, au lieu d'écrire de zéro. Cela réduit le temps de traitement sur chaque ticket.

**Automatiser les actions de routine.** Certains tickets ont besoin d'une action simple — réinitialiser un mot de passe, renvoyer un document, mettre à jour une adresse. L'IA peut faire cela automatiquement et fermer le ticket, ou rédiger l'action pour qu'un humain l'approuve. Le travail de routine disparaît de la file.

**Gardez la piste d'audit.** Chaque ticket devrait enregistrer ce qui s'est passé, qui a fait quoi, et quand. Cela compte pour la revue qualité, pour la formation, et pour la responsabilité. De bons outils de ticketing produisent cela automatiquement ; confirmez que le vôtre le fait.

### 27.3 Analyse de sentiment

L'analyse de sentiment signifie utiliser l'IA pour lire le *ressenti* derrière un message — le client est-il content, neutre, frustré ou en colère ? Elle transforme un texte brut en un signal émotionnel sur lequel vous pouvez agir.

**Pourquoi c'est important.** Un client en colère qui attend dans une file normale peut partir avant que quiconque ne le voie. Si l'IA signale la colère tôt, un agent senior peut répondre vite et transformer un mauvais moment en un bon. Le sentiment est un signal de routage que le simple appariement de sujet manque.

**Comment ça marche.** L'IA lit les mots et le ton d'un message et assigne un sentiment — positif, neutre, négatif — ou un score. Elle apprend de nombreux exemples de messages étiquetés par des humains. Elle n'est pas parfaite, mais elle est assez bonne pour signaler les clients clairement contrariés.

**Utilisez-la pour prioriser, pas pour juger.** Injectez le sentiment dans la file de tickets pour que les messages les plus négatifs remontent en haut. Ne l'utilisez pas pour noter ou punir les agents, et ne traitez pas une seule lecture de sentiment comme le dernier mot sur les sentiments d'un client. C'est un indice pour prêter attention, pas un verdict.

**Surveillez les tendances dans le temps.** Le sentiment est le plus utile comme tendance. Si le sentiment négatif à travers tous les tickets monte de mois en mois, quelque chose ne va pas avec votre produit ou service, même avant que les clients n'écrivent une réclamation formelle. Suivez le sentiment moyen et surveillez la direction.

**Méfiez-vous des limites.** Le sarcasme, l'ironie et les différences culturelles peuvent tromper l'analyse de sentiment. Un « super, encore un problème » se lit comme positif pour un modèle naïf. Utilisez le sentiment comme un signal parmi d'autres, et laissez le jugement d'un humain le contredire.

### 27.4 Base de connaissances intelligente

Une base de connaissances est une bibliothèque consultable de réponses aux questions courantes. Une base de connaissances *intelligente* utilise l'IA pour rendre bien plus facile de trouver la bonne réponse — et pour garder les réponses à jour.

**Une recherche qui comprend la question.** Au lieu de faire correspondre des mots-clés exacts, une base de connaissances IA comprend ce que le client veut dire et renvoie l'article pertinent même si les mots diffèrent. « Ma carte a été débitée deux fois » trouve l'article sur le paiement en double, pas seulement les articles contenant ces mots exacts.

**L'IA écrit et met à jour les articles.** Quand un agent d'assistance résout un nouveau problème, l'IA peut rédiger un article de base de connaissances à partir du ticket résolu, pour que la réponse soit capturée pour la prochaine fois. Cela transforme chaque problème résolu en une réponse réutilisable, au lieu de la laisser enfermée dans la tête d'un seul agent.

**Une source unique de vérité.** Votre chatbot, votre page FAQ et vos agents devraient tous puiser dans la même base de connaissances. Quand vous mettez à jour un endroit, chaque canal obtient la bonne réponse. Si vous les maintenez séparément, ils dérivent et donnent des réponses contradictoires, ce qui détruit la confiance.

**Repérez les manques.** L'IA peut voir quelles questions les clients posent qui n'ont pas d'article. Ces manques sont une liste de choses à faire : écrivez les réponses manquantes, et le bot et la recherche s'améliorent. La base de connaissances s'améliore elle-même en vous montrant ce qui manque.

**Gardez-la fraîche.** Une base de connaissances périmée donne de fausses réponses avec assurance. Revoyez les articles régulièrement, retirez les périmés, et laissez l'IA signaler les articles qui pourraient avoir besoin d'une mise à jour parce que le produit a changé. La fraîcheur est toute la valeur d'une base de connaissances.

## Éthique et responsabilité

L'assistance est l'endroit où la confiance se gagne ou se perd, donc les enjeux éthiques sont élevés.

**Ne laissez jamais un bot cacher un humain.** Les clients ont le droit d'atteindre une personne. Un chatbot qui bloque le chemin vers un humain est un design hostile. Rendez le passage de relais facile, clair, et toujours disponible.

**Divulguez que c'est un bot.** Un client devrait savoir qu'il parle à une IA et pas à une personne. C'est une bonne pratique partout et une exigence légale dans certains endroits.

**N'ignorez pas un client en colère à cause d'une erreur de modèle.** Si l'analyse de sentiment manque un client en colère, la file humaine doit quand même le rattraper. Le sentiment est un assistant, pas un portier. Ne laissez jamais l'erreur d'un modèle enterrer une vraie réclamation.

**Protégez les données clients.** Les tickets d'assistance contiennent des informations personnelles, parfois sensibles. Traitez-les avec soin et suivez les règles de confidentialité — les bases sont dans le [Chapitre 10 — Confidentialité et RGPD](ch10-privacy-and-gdpr.md). Ne donnez pas de données clients sensibles à des outils IA publics sans vérifier les implications de sécurité (voir le [Chapitre 6 — La cybersécurité à l'ère de l'IA](ch06-cybersecurity-in-the-ai-era.md)).

**Gardez un humain responsable.** L'IA peut rédiger une réponse ou router un ticket, mais un humain possède le résultat. Quand quelque chose tourne mal, il doit y avoir une personne responsable, pas une boîte noire.

**Utilisez le sentiment pour aider, pas pour manipuler.** Lire les sentiments d'un client devrait vous aider à mieux le servir, pas exploiter sa frustration pour vendre plus ou le mettre sous pression. Restez du côté du soin.

**N'utilisez pas les données d'assistance pour surveiller les agents.** Suivre les métriques de tickets pour améliorer le processus va bien. Utiliser les mêmes données pour espionner et punir des agents individuels empoisonne la confiance. Mesurez le travail, pas la personne.

## Erreurs à éviter

**Un bot qui bloque l'humain.** La pire erreur d'assistance. Rendez toujours le passage de relais facile.

**Pas de contexte au passage de relais.** Passer un client à un humain qui lui demande ensuite de tout répéter. Faites voyager le contexte.

**Chatbot qui bluffe.** Un bot qui devine au lieu d'admettre qu'il ne sait pas. Apprenez-lui à passer le relais quand il n'est pas sûr.

**Base de connaissances périmée.** Des articles obsolètes donnant de fausses réponses avec assurance. Revoyez et mettez à jour régulièrement.

**Sources de vérité séparées.** Chatbot, FAQ et agents chacun avec leurs propres réponses qui dérivent. Utilisez une seule base de connaissances.

**Le sentiment comme verdict.** Traiter la lecture de sentiment d'un modèle comme le dernier mot sur un client. C'est un indice, pas un jugement.

**Manquer le client en colère.** Laisser une erreur de modèle enterrer un client contrarié. La file humaine doit quand même le rattraper.

**Automatiser un mauvais processus.** Si votre flux d'assistance est cassé, l'automatisation fait un flux cassé plus rapide. Réparez le processus d'abord.

**Fuir des données sensibles.** Mettre des données clients dans des outils IA non sécurisés. Vérifiez la sécurité et la confidentialité d'abord.

**Pas de piste d'audit.** Des tickets qui ne peuvent pas montrer ce qui s'est passé. Gardez l'enregistrement.

**Confondre la déviation avec le succès.** Compter combien de tickets le bot a « gérés » au lieu de savoir si le client était réellement satisfait. Mesurez la résolution et la satisfaction, pas la déviation.

**Sauter la référence de départ.** Ne pas mesurer le temps de réponse ou la satisfaction avant, pour ne pas pouvoir prouver l'amélioration. Mesurez d'abord (voir le Chapitre 22).

## Exercice pratique

### 27.7 Exercice : concevez votre automatisation d'assistance

Choisissez un canal d'assistance et planifiez son aide IA de bout en bout.

**Étape 1 — Choisissez le canal.** Choisissez-en un : un chatbot de site web, votre file de tickets, ou votre base de connaissances. Faites-en un, pas tous.

**Étape 2 — Définissez le but et la métrique.** Une réponse plus rapide ? Une résolution en libre-service plus élevée ? Moins de clients en colère ? Choisissez un nombre à mesurer.

**Étape 3 — Mesurez la référence de départ.** Quelle est ce nombre maintenant ? Temps de réponse moyen, taux de résolution, score de satisfaction. Écrivez-le.

**Étape 4 — Listez les questions courantes.** Récupérez le dernier mois de tickets et trouvez les 10 questions répétées principales. Ce sont ce que le bot et la base de connaissances devraient gérer.

**Étape 5 — Écrivez les réponses.** Pour chaque question courante, écrivez la réponse que vous voulez. Cela devient votre base de connaissances et l'entraînement de votre bot.

**Étape 6 — Fixez les règles de passage de relais.** Décidez exactement quand le bot passe à un humain : pas sûr, demandé, sensible. Écrivez les règles.

**Étape 7 — Ajoutez le routage par sentiment.** Si votre outil le prend en charge, configurez les tickets à sentiment négatif pour qu'ils remontent en haut de la file.

**Étape 8 — Lancez petit et mesurez.** Faites-le tourner sur une tranche du trafic d'abord. Comparez la métrique à la référence de départ. Ne passez à l'échelle que ce qui prouve qu'il résout réellement, pas juste dévie.

Faites un canal bien. La liste des questions courantes que vous construisez à l'étape 4 a de la valeur à elle seule — elle vous montre exactement ce qui confond vos clients, ce qui est utile même au-delà de l'assistance.

## Liste de contrôle

### 27.8 Liste de contrôle de la relation client et de l'assistance

Avant de lancer l'IA dans l'assistance, vérifiez ceci.

- [ ] **Vous avez mesuré la référence de départ** — temps de réponse, taux de résolution, satisfaction.
- [ ] **Le chatbot passe le relais à un humain facilement**, avec un contexte complet.
- [ ] **Vous divuliguez que c'est un bot** là où c'est requis et comme bonne pratique.
- [ ] **Le bot est entraîné sur vos vraies questions courantes**, pas des génériques.
- [ ] **Le bot admet quand il ne sait pas** au lieu de bluffer.
- [ ] **Les tickets sont routés automatiquement** vers la bonne équipe ou le bon agent.
- [ ] **Les clients urgents et contrariés sont priorisés** dans la file.
- [ ] **Le sentiment est un indice pour prêter attention**, pas un verdict sur le client.
- [ ] **Vous avez une seule base de connaissances** qui alimente le bot, la FAQ et les agents.
- [ ] **La base de connaissances est gardée fraîche** et revue régulièrement.
- [ ] **L'IA rédige des réponses et des articles** à partir des tickets résolus pour capturer le savoir.
- [ ] **Vous gardez une piste d'audit** sur chaque ticket.
- [ ] **Les données clients sont traitées de façon sécurisée** et suivent les règles de confidentialité (voir le Chapitre 10).
- [ ] **Un humain possède le résultat** — pas de responsabilité en boîte noire.
- [ ] **Vous mesurez la résolution et la satisfaction**, pas juste la déviation.
- [ ] **Vous réparez le processus d'assistance avant de l'automatiser.**

Si une case est vide, un client peut le sentir. Remplissez-la avant de laisser l'IA répondre à votre place.

## Points à retenir

- L'IA dans l'assistance raccourcit la file en répondant instantanément aux questions courantes et en routant les dures vers la bonne personne vite.
- Le cas TridentCare (une annonce de ServiceNow) a atteint 96 % d'automatisation de la planification sur 127 marchés, réduisant la planification manuelle de 50 % à 4,3 % et les temps d'attente des patients au-delà du SLA de 57 %, avec des humains supervisant au lieu de faire le travail.
- La fonctionnalité la plus importante du chatbot est un passage de relais propre à un humain avec un contexte complet — ne laissez jamais un bot bloquer une personne.
- Une base de connaissances fraîche et partagée devrait alimenter le bot, la FAQ et vos agents ; l'analyse de sentiment devrait prioriser la file, pas juger le client.
- Mesurez la résolution et la satisfaction, pas la déviation, et gardez un humain responsable de chaque résultat.

<!-- BEGIN agentbridge-examples -->

## Essayez avec AgentBridge

Voici à quoi ressemble le même travail avec AgentBridge. Chaque encadré montre le résultat fini et la seule ligne que vous tapez pour l'obtenir.

### Répondre à un email avec votre voix

![Une réponse email rédigée, prête à envoyer](../../assets/examples/quick-reply.png)
*Une réponse email rédigée, prête à envoyer*

**Ce que vous demandez :** `Réponds à ce client en le remerciant et en confirmant que nous expédions demain : [collez l'email]`

L'agent écrit une réponse amicale et professionnelle qui sonne comme vous. Vous la lisez une fois, appuyez sur envoyer, et passez à autre chose.

*Conseil : Configurez votre messagerie une fois avec /email. Après cela, lire et envoyer se font depuis le chat.*

---

### Faire le point sur votre boîte de réception

![Un court résumé de la boîte de réception avec les éléments urgents](../../assets/examples/inbox-summary.png)
*Un court résumé de la boîte de réception avec les éléments urgents*

**Ce que vous demandez :** `Résume mes emails non lus et dis-moi lesquels nécessitent une réponse aujourd'hui.`

L'agent lit votre courrier non lu et vous donne une courte liste : ce qui est urgent, ce qui peut attendre, et ce que vous pouvez ignorer. Vous vous attaquez aux vraies priorités d'abord.

*Conseil : Un résumé du matin peut être planifié pour que cela vous attende avec votre café.*

---

### Trouver un client rapidement

![Un enregistrement client récupéré sur demande](../../assets/examples/customer-lookup.png)
*Un enregistrement client récupéré sur demande*

**Ce que vous demandez :** `Trouve le cliente Maria Rossi et montre son contact et sa dernière commande.`

L'agent trouve le client et montre les coordonnées et la dernière commande, pour que vous puissiez aider sans le mettre en attente.

*Conseil : Demandez les trois dernières commandes si vous voulez le tableau complet.*

<!-- END agentbridge-examples -->
