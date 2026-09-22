# Chapitre 20 — Mettre en place l'IA en toute sécurité

## En mots simples

Quand vous faites entrer l'IA dans votre entreprise, vous laissez un nouveau travailleur manipuler vos données. Comme tout travailleur, ce nouveau travailleur doit être digne de confiance, surveillé et borné. Ce chapitre parle de faire cela — comment utiliser l'IA sans fuiter les données de vos clients, vos finances ou vos secrets.

La sécurité n'est pas un produit que l'on achète. C'est un ensemble d'habitudes que l'on construit. Le but est simple : **concevez vos automatisations pour que, même quand quelque chose tourne mal, vos données restent protégées.** Cette idée a un nom — **la sécurité dès la conception** — et elle signifie que vous pensez à la sécurité au départ, pas en après-coup après une violation.

Une bonne analogie est une maison. Vous ne laissez pas la porte d'entrée grande ouverte parce que « rien de mauvais n'est encore arrivé ». Vous verrouillez les portes, vous limitez les pièces où les invités peuvent entrer, vous mettez une lumière sur minuteur, et vous avez un plan si vous rentrez chez vous et trouvez une fenêtre ouverte. La sécurité de l'IA, c'est la même réflexion en couches : contrôler qui entre, protéger ce qui est à l'intérieur, surveiller ce qui se passe, et savoir quoi faire si quelque chose casse.

Ce chapitre couvre les habitudes de base : concevoir des automatisations sûres, contrôler qui peut faire quoi, chiffrer les données pour qu'elles soient illisibles pour les voleurs, surveiller et journaliser ce que l'IA fait, planifier le jour où quelque chose tourne mal, et former votre personnel — parce que le facteur humain est la première ligne de défense.

Une vérité honnête dès le départ : aucun système n'est parfaitement sûr. Le but n'est pas la perfection ; c'est de faire de votre entreprise une cible difficile, et jamais une cible facile. La plupart des attaques visent la cible facile. Une sécurité bonne et simple vous fait passer de facile à difficile.

## Un peu d'histoire

**Années 1970–1980 : la sécurité démarre à la périphérie.** La sécurité informatique des débuts se concentrait sur garder les étrangers dehors — pare-feu, mots de passe, salles de serveurs verrouillées. Le modèle était un château : murs solides, tout ce qui est à l'intérieur est sûr. Cela a fonctionné tant que les gens n'avaient pas besoin de se connecter et de partager, ce qui a fissuré les murs.

**Années 1990 : la périphérie se dissout.** Internet et l'e-mail ont fait que la donnée a commencé à bouger. Le modèle du château s'est brisé. Virus et intrusions arrivaient par les connexions mêmes qui rendaient les affaires possibles. La sécurité devait suivre la donnée, pas seulement garder la porte.

**Années 2000 : le « moindre privilège » et la défense en profondeur.** La réflexion sur la sécurité s'est déplacée vers l'intérieur. Le principe du **moindre privilège** — donner à chaque utilisateur et programme seulement l'accès strictement nécessaire, rien de plus — est devenu central. Ainsi que la **défense en profondeur** : beaucoup de couches qui se chevauchent, pour que si l'une échoue, une autre attrape la menace.

**Années 2010 : « supposer la violation ».** Les experts ont compris qu'on ne peut pas toujours garder les attaquants dehors. Le nouvel état d'esprit était de *supposer* qu'un intrus est peut-être déjà à l'intérieur, et de se concentrer sur limiter ce à quoi il peut accéder et le repérer vite. Journalisation, surveillance et réponse rapide sont devenus aussi importants que les murs.

**Années 2020 : l'IA ajoute une nouvelle surface d'attaque.** L'IA apporte de nouvelles façons d'être nuisible — des astuces qui trompent l'IA elle-même, l'empoisonnement de données, et le risque de nourrir des données sensibles dans des outils que vous ne contrôlez pas. (Ces menaces spécifiques sont traitées au [Chapitre 6](ch06-cybersecurity-in-the-ai-era.md).) Les anciens principes — moindre privilège, défense en profondeur, supposer la violation — s'appliquent toujours, désormais appliqués à un nouveau type de travailleur.

L'arc : d'un château à un seul mur à beaucoup de couches qui supposent que le mur peut être franchi. La leçon n'a jamais changé : protégez la donnée elle-même, pas seulement la porte.

## Curiosité

### 20.7 L'entreprise qui a repéré une attaque dans un journal que personne ne regardait

*L'entreprise spécifique de cette histoire est illustrative — une composition réaliste, pas une firme nommée. Le schéma derrière est réel et bien documenté.*

Imaginez une entreprise de taille moyenne qui avait un système de journalisation — un registre de tout ce qui se passait sur son réseau. Les journaux tournaient en permanence, enregistrant fidèlement chaque connexion, chaque fichier consulté, chaque requête inhabituelle. Pendant des mois, personne ne les lisait. Ils étaient là, comme une caméra de sécurité que personne ne regarde.

Puis un jour, un nouveau technicien, en faisant le ménage, a jeté un œil aux journaux et a vu quelque chose d'étrange : un programme cherchait à joindre une adresse extérieure à des heures bizarres, tirant des données lentement et régulièrement. Il faisait cela depuis des semaines. Personne n'avait remarqué parce que personne ne regardait. Quand ils ont enfin regardé, ils ont trouvé un intrus qui avait été tranquillement à l'intérieur bien plus longtemps que quiconque l'imaginait.

La leçon inconfortable n'est pas que l'entreprise était négligente. C'est que **la preuve était là tout du long — et elle a été ignorée.** L'entreprise avait investi dans la caméra mais pas dans le fait de la regarder.

Ce schéma n'est pas de la fiction. Le rapport annuel d'IBM *Cost of a Data Breach* a constaté, année après année, que les violations mettent longtemps à être détectées — de l'ordre de **deux cents jours** en moyenne dans les éditions récentes — et qu'une grande part sont d'abord remarquées par quelqu'un hors de l'entreprise, pas par la surveillance de l'entreprise elle-même. Les journaux et les signaux existent souvent. Ce qui manque, c'est une personne qui les regarde.

Pour vos automatisations IA, la leçon est directe : **un journal que personne ne lit n'est pas une sécurité.** Si vous collectez des registres de ce que votre IA fait, désignez quelqu'un pour regarder vraiment, et mettez des alertes pour que les signaux importants trouvent un humain au lieu d'attendre d'être découverts.

## Un exemple d'entreprise réel

*Ce qui suit est une composition illustrative de schémas réels courants, pas une seule entreprise nommée.*

Un petit commerçant en ligne voulait que l'IA rédige des e-mails de support client. La façon facile et risquée était de donner à l'IA un accès complet à toute la base de données clients — noms, adresses, historique de paiement — et de la laisser lire ce dont elle avait besoin. Le patron a marqué une pause et a fait les choses de la façon plus sûre.

Ils ont donné à l'IA un accès en **lecture seule** à seulement les détails de commande nécessaires pour répondre à une question d'expédition — pas les dossiers de paiement, pas le dossier client complet. Ils ont configuré pour que l'IA puisse rédiger mais qu'un humain appuie sur envoyer. Ils ont activé un journal qui enregistrait chaque commande que l'IA touchait. Ils ont dit à l'équipe de support ce que l'IA pouvait et ne pouvait pas voir, et leur ont demandé de signaler tout ce qui leur paraissait étrange.

Au bout de trois semaines, le journal a montré qu'il avait été demandé à l'IA — par un client malin — de révéler l'adresse d'un autre client en se faisant passer pour cette personne. L'IA avait refusé, parce qu'elle n'avait pas reçu accès à cette donnée dès le départ. La tentative a échoué sans dommage, et le journal l'a capturée pour que l'équipe apprenne que l'astuce existait.

Si le patron avait pris la voie facile et donné à l'IA toute la base de données, la même astuce aurait peut-être fonctionné. La conception sûre — moindre accès, humain sur l'envoi, un journal surveillé — a transformé une violation potentielle en non-événement. Voilà à quoi ressemble la sécurité dès la conception en pratique.

## Comment faire

### 20.1 Principes de sécurité dès la conception : comment concevoir une automatisation qui n'expose pas de donnée

La sécurité dès la conception signifie que vous intégrez la sécurité dans l'automatisation dès le premier croquis. Posez ces questions avant de construire quoi que ce soit :

- **De quelle donnée cette automatisation a-t-elle vraiment besoin ?** Utilisez le moins possible. Si elle a seulement besoin d'un numéro de commande, ne lui donnez pas le dossier client entier.
- **Quel est le pire qui pourrait arriver si elle fuit ou est trompée ?** Imaginez la panne. Concevez pour que le pire cas soit petit.
- **Où va la donnée ?** Connaissez chaque système que la donnée touche, surtout hors de votre contrôle. Ne nourrissez pas de donnée sensible dans un outil que vous ne pouvez pas justifier.
- **Un humain peut-il l'arrêter ?** Intégrez un bouton d'arrêt d'urgence — un moyen de couper l'automatisation instantanément si elle se comporte mal.
- **Est-ce qu'elle tombe en mode sûr ?** Si quelque chose casse, l'automatisation doit s'arrêter et protéger, pas s'ouvrir. Une porte qui se verrouille quand le courant lâche est « à sécurité positive ».

Le principe central est le **moindre privilège** : accès minimal, portée minimale, donnée minimale. Une automatisation qui n'a jamais eu accès à la donnée sensible ne peut pas la fuiter, aussi astucieuse que soit l'attaque. Concevez l'accès hors du jeu, et le risque part avec lui.

### 20.2 Contrôle d'accès : qui peut faire quoi

Le contrôle d'accès, c'est simplement décider qui est autorisé à faire quoi, et l'appliquer. C'est la serrure de chaque pièce, pas seulement de la porte d'entrée.

Trois règles simples :

- **Donnez à chaque personne et à chaque outil seulement l'accès que leur travail exige.** Un outil de support qui répond à des questions d'expédition a besoin des données de commande, pas des données de paie. Un membre junior du personnel ne devrait pas avoir le même accès que le patron.
- **Séparez les fonctions.** La personne qui met en place l'IA ne devrait pas être la seule à pouvoir approuver ses actions, ni la seule à pouvoir voir les journaux. Répartissez les clés pour qu'aucun compte unique compromis ne puisse tout faire.
- **Passez les accès en revue quand les gens changent.** Quand du personnel arrive, bouge ou part, mettez à jour leur accès le jour même. Un vieil accès qui traîne est l'une des façons les plus courantes dont les violations arrivent.

Utilisez les outils que vos systèmes ont déjà — rôles utilisateurs, permissions et contrôles de connexion. Activez l'**authentification à deux facteurs** (une deuxième étape au-delà du mot de passe, comme un code sur votre téléphone) partout où vous le pouvez. Cela arrête la plupart des attaques par mot de passe volé.

### 20.3 Chiffrement : protéger la donnée en transit et au repos

Le **chiffrement** signifie brouiller la donnée pour que seule une personne avec la bonne clé puisse la lire. Pour un voleur, une donnée chiffrée ressemble à du charabia. Elle protège la donnée dans deux états :

- **En transit** — la donnée qui se déplace entre des endroits, comme un e-mail ou un téléversement de fichier. Le chiffrement ici signifie qu'un voleur qui écoute le câble voit des ordures. Cherchez « https » et les connexions sécurisées.
- **Au repos** — la donnée qui reste immobile, comme des fichiers sur un disque ou des enregistrements dans une base de données. Le chiffrement ici signifie qu'un voleur qui dérobe le disque dur ne peut toujours pas le lire.

Pour une petite entreprise, les étapes pratiques sont simples : utilisez des outils qui chiffrent par défaut (la plupart des services réputés le font), vérifiez que les connexions sont sûres (https), et demandez directement à tout fournisseur : « Ma donnée est-elle chiffrée en transit et au repos ? » Un fournisseur sérieux répond oui et explique comment. S'ils ne le peuvent pas, c'est un avertissement.

Une mise en garde : le chiffrement protège la donnée des étrangers. Il ne protège pas de quelqu'un qui a la clé et en fait un mauvais usage. C'est pourquoi le contrôle d'accès (20.2) et le chiffrement fonctionnent ensemble — le chiffrement cache la donnée, le contrôle d'accès limite qui détient la clé.

### 20.4 Surveillance et journalisation : toujours savoir ce que l'IA fait

Un **journal** est un registre de ce qui s'est passé : qui a fait quoi, quand, sur quelle donnée. La **surveillance** consiste à regarder ces journaux, en direct ou régulièrement, pour repérer les ennuis.

Pourquoi c'est important pour l'IA : une automatisation IA agit sur votre donnée toute la journée. Sans journal, vous ne pouvez pas dire ce qu'elle a touché, ce qu'elle a modifié, ou si elle a été trompée. Avec un journal, vous avez un registre à vérifier et une piste qu'un attaquant ne peut pas cacher.

Rendez la journalisation utile :

- **Journalisez les actions importantes** — quelle donnée l'IA a lue, ce qu'elle a écrit, ce qu'elle a envoyé, et toute requête qu'elle a refusée.
- **Mettez des alertes** pour que les signaux importants trouvent un humain. Ne faites pas fixer un écran à quelqu'un ; faites crier le système quand quelque chose d'inhabituel se produit.
- **Regardez vraiment.** Comme l'histoire de curiosité le montre, un journal que personne ne lit n'est pas une sécurité. Désignez quelqu'un pour passer en revue, même brièvement, selon un calendrier régulier.
- **Gardez les journaux en sûreté** pour qu'un intrus ne puisse pas les effacer.

La surveillance transforme un système silencieux en un système visible. Vous ne pouvez pas protéger ce que vous ne pouvez pas voir.

### 20.5 Plans de réponse aux incidents : quoi faire si quelque chose tourne mal

Quelque chose finira par tourner mal. La question n'est pas « si » mais « quand », et à quel point vous êtes prêt. Un **plan de réponse aux incidents** est un plan écrit pour le jour du malheur, fait un jour calme pour ne pas improviser dans la panique.

Un plan simple a cinq étapes :

1. **Détecter.** Comment saurez-vous que quelque chose ne va pas ? (Une alerte, un signalement du personnel, une plainte de client.)
2. **Confiner.** Comment arrêtez-vous les dégâts maintenant ? (Couper l'automatisation, couper la connexion, verrouiller le compte.)
3. **Évaluer.** Qu'a été exposé ou endommagé ? Vérifiez les journaux.
4. **Réparer et récupérer.** Réparez la cause et restaurez un fonctionnement normal et sûr.
5. **Signaler et apprendre.** Dites aux gens qui doivent savoir — et sachez à qui vous êtes légalement tenu de dire. (Les lois sur la vie privée comme le RGPD ont des obligations de signalement ; voir [Chapitre 10](ch10-privacy-and-gdpr.md).) Puis écrivez ce qui s'est passé et comment l'empêcher la prochaine fois.

Écrivez le plan sur une page. Nommez qui fait quoi. Gardez les contacts d'urgence prêts. Faites un rapide exercice une fois par an pour que chacun connaisse sa partie. Un plan répété transforme une crise en un événement gérable.

### 20.6 Formation du personnel : le facteur humain est la première défense

La serrure la plus solide peut être défaite par une seule personne négligente. Votre personnel est à la fois votre plus gros risque et votre meilleure défense. La formation les transforme du point faible en première ligne.

Qu'enseigner, en termes simples :

- **Reconnaître les astuces.** Les attaquants trompent les gens avec de faux e-mails, des demandes urgentes et des appels « je suis de l'informatique, donnez-moi votre mot de passe ». Apprenez au personnel à les repérer et à en douter.
- **Manipuler la donnée avec soin.** Qui a le droit de voir quoi, et pourquoi. Ne partagez jamais de donnée client hors des canaux approuvés.
- **Signaler, ne pas cacher.** Rendez sûr et attendu le fait de signaler une erreur ou une demande étrange. Un membre du personnel qui signale tôt un e-mail suspect sauve l'entreprise. Celui qui le cache laisse un petit problème grossir.
- **Connaître les limites de l'IA.** Le personnel doit savoir ce que l'IA peut et ne peut pas voir, et ne jamais lui demander de faire quelque chose hors de ses limites sûres.
- **Hygiène des mots de passe et des connexions.** Mots de passe forts, authentification à deux facteurs, pas de partage de logins.

Gardez la formation courte, régulière et pratique — pas un cours annuel unique. Un rappel mensuel de cinq minutes et un canal de signalement clair font plus qu'un long cours annuel dont personne ne se souvient.

## Éthique et responsabilité

La sécurité est un devoir éthique, pas seulement technique.

**Protégez les gens dont vous détenez la donnée.** Clients, employés et partenaires vous ont fait confiance avec leurs informations. Une violation fait du mal à de vraies personnes. Traiter cette donnée en sécurité est une question d'honnêteté et de soin.

**Signalez honnêtement quand les choses tournent mal.** Si vous devez notifier des clients ou des régulateurs, faites-le rapidement et véridiquement. Cacher une violation est pire que la violation elle-même, éthiquement et légalement.

**N'utilisez pas la sécurité comme une excuse pour cacher.** « Nous sommes sûrs » ne devrait jamais vouloir dire « vous ne pouvez pas vérifier ». Responsabilité et transparence vont ensemble.

**Équilibrez sécurité et utilisabilité.** Une sécurité si lourde que personne ne peut travailler est contournée, et une sécurité contournée n'est pas du tout une sécurité. Faites du chemin sûr le chemin facile.

**Formez avec respect, pas avec blâme.** Quand quelqu'un fait une erreur, enseignez, ne punissez pas. Une culture du blâme cache les erreurs ; une culture de l'apprentissage les fait surface tôt.

Sécurisez votre donnée comme vous voudriez que la vôtre soit protégée.

## Erreurs à éviter

**Trop d'accès.** Donner à l'IA ou au personnel plus d'accès que nécessaire. Utilisez le moindre privilège.

**Pas d'humain sur l'envoi.** Laisser l'IA agir seule sur des messages destinés au client. Gardez une vérification humaine.

**Nourrir de la donnée sensible dans des outils non vérifiés.** Coller de la donnée client dans un outil que vous ne pouvez pas justifier. Sachez où va la donnée.

**Un journal que personne ne lit.** Collecter des registres et ne jamais regarder. Désignez quelqu'un et mettez des alertes.

**Pas de plan d'incident.** Improviser le jour du malheur. Écrivez le plan un jour calme.

**Partager les logins.** Un compte partagé par beaucoup de gens détruit la responsabilité. Donnez à chacun le sien.

**Pas d'authentification à deux facteurs.** Laisser les comptes ouverts aux mots de passe volés. Activez le 2FA partout.

**Ignorer les changements de personnel.** Un vieil accès qui traîne après le départ de quelqu'un. Mettez à jour l'accès le jour où les rôles changent.

**Blâmer au lieu de former.** Punir les erreurs pour que les gens les cachent. Enseignez et encouragez le signalement.

**Supposer que le fournisseur est sûr.** Faire confiance sans demander. Demandez aux fournisseurs au sujet du chiffrement et de l'accès.

**La sécurité en après-coup.** Construire l'automatisation d'abord et penser à la sécurité plus tard. Intégrez la sécurité dès le départ.

**Pas de bouton d'arrêt d'urgence.** Pas de moyen d'arrêter l'automatisation vite quand elle se comporte mal. Construisez l'interrupteur d'arrêt.

## Exercice pratique

### 20.8 Exercice : écrivez votre plan de sécurité IA

Écrivez un plan de sécurité d'une page pour une automatisation IA que vous utilisez ou prévoyez d'utiliser. Remplissez chaque ligne.

**1. L'automatisation.** Nommez-la et dites quelle donnée elle touche.

**2. Moindre accès.** Listez exactement de quelle donnée elle a besoin. Coupez tout le reste. Écrivez l'accès que vous accorderez réellement.

**3. Vérification humaine.** Où est l'humain dans la boucle ? Que peut faire l'IA seule, et quoi a besoin d'une personne pour approuver ?

**4. Emplacement de la donnée.** Où va la donnée ? Listez chaque système, surtout hors de votre contrôle. Notez ceux que vous ne pouvez pas justifier et retirez-les.

**5. Chiffrement.** La donnée est-elle chiffrée en transit et au repos ? Vérifiez avec chaque fournisseur et écrivez la réponse.

**6. Contrôle d'accès.** Qui peut faire quoi ? Listez les rôles. Notez où vous activerez l'authentification à deux facteurs.

**7. Journalisation.** Que journaliserez-vous ? Qui regardera, et à quelle fréquence ? Que déclenchera une alerte ?

**8. Bouton d'arrêt d'urgence.** Comment le coupez-vous instantanément ? Écrivez les étapes exactes.

**9. Plan d'incident.** Écrivez les cinq étapes — détecter, confiner, évaluer, réparer, signaler — avec des noms pour qui fait chacune. Notez toute obligation légale de signalement (voir [Chapitre 10](ch10-privacy-and-gdpr.md)).

**10. Formation du personnel.** Qu'enseignerez-vous à l'équipe à propos de cette automatisation, et comment signaleront-ils un problème ?

Mettez-le sur une page. Partagez-le avec les personnes concernées. Gardez-le là où vous pouvez le trouver le jour du malheur. Un plan écrit un jour calme vaut dix fois un plan que vous inventez dans une crise.

## Liste de contrôle

### 20.9 Liste de contrôle : les 15 questions de sécurité

Avant de laisser une automatisation IA toucher de la vraie donnée, répondez à ces quinze questions. Chacune doit être un « oui » clair.

- [ ] **1. Moindre accès :** L'automatisation a-t-elle seulement la donnée dont elle a vraiment besoin, et rien de plus ?
- [ ] **2. Humain sur l'envoi :** Un humain vérifie-t-il tout ce qui atteint un client ?
- [ ] **3. Emplacement de la donnée :** Est-ce que je connais chaque système que la donnée touche, y compris hors de mon contrôle ?
- [ ] **4. Outils vérifiés :** Ai-je refusé de nourrir de la donnée sensible dans un outil que je ne peux pas justifier ?
- [ ] **5. Chiffrée en transit :** La donnée est-elle chiffrée pendant qu'elle se déplace entre les systèmes ?
- [ ] **6. Chiffrée au repos :** La donnée est-elle chiffrée pendant qu'elle est stockée ?
- [ ] **7. Logins individuels :** Chaque personne a-t-elle son propre login, sans partage ?
- [ ] **8. Authentification à deux facteurs :** Le 2FA est-il activé pour les comptes importants ?
- [ ] **9. Fonctions séparées :** La mise en place, l'approbation et la revue des journaux sont-elles réparties entre plusieurs personnes ?
- [ ] **10. Revue des accès :** Est-ce que je mets à jour l'accès le jour où le personnel arrive, bouge ou part ?
- [ ] **11. Journalisation :** Est-ce que j'enregistre ce que l'IA lit, écrit, envoie et refuse ?
- [ ] **12. Journaux surveillés :** Quelqu'un passe-t-il vraiment en revue les journaux, avec des alertes pour les signaux importants ?
- [ ] **13. Bouton d'arrêt d'urgence :** Puis-je couper l'automatisation instantanément, et est-ce que je sais comment ?
- [ ] **14. Plan d'incident :** Ai-je un plan écrit et nommé pour détecter, confiner, évaluer, réparer et signaler ?
- [ ] **15. Personnel formé :** L'équipe a-t-elle été enseignée à repérer les astuces et signaler les problèmes en sûreté ?

Si une réponse est « non », l'automatisation n'est pas prête. Réparez-la avant de passer en production. La sécurité n'est pas un produit que l'on achète une fois ; c'est quinze questions auxquelles on continue de répondre oui.

## Points clés

- La sécurité dès la conception signifie intégrer la sécurité dès le départ — moindre accès, un humain sur l'envoi, et un bouton d'arrêt d'urgence — pour que le pire cas reste petit.
- Un journal que personne ne lit n'est pas une sécurité : collectez des registres, mettez des alertes, et désignez quelqu'un pour regarder vraiment.
- Le chiffrement cache la donnée des étrangers (en transit et au repos), tandis que le contrôle d'accès limite qui détient la clé — vous avez besoin des deux fonctionnant ensemble.
- Écrivez votre plan de réponse aux incidents un jour calme : détecter, confiner, évaluer, réparer, signaler, apprendre — avec des noms attachés à chaque étape.
- Le facteur humain est la première défense : formez le personnel à repérer les astuces et signaler en sûreté, et faites du chemin sûr le chemin facile.
