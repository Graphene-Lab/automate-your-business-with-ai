# Annexe D — Inventaire des données

On ne peut pas protéger des données qu'on ne trouve pas. Cet inventaire liste chaque élément de données important que votre entreprise détient, où il se trouve, et qui peut y accéder. Remplissez-le avant de connecter un quelconque outil d'IA. Si une donnée ne figure pas sur cette liste, ne la donnez pas à l'IA.

## Comment l'utiliser

1. Parcourez vos outils : e-mail, disques, comptabilité, CRM, systèmes RH, tableurs.
2. Ajoutez une ligne par élément de données (une liste clients, un fichier de paie, un dossier de contrats).
3. Marquez chaque élément **Personnel** (se rapporte à une personne) ou **Sensible** (catégories particulières — voir plus bas).
4. Vérifiez l'accès : qui peut l'ouvrir aujourd'hui, et qui *devrait* le pouvoir.
5. Relisez-le avant tout projet d'IA. Cette liste vous dit ce qui est sûr à utiliser et ce qui ne l'est pas.

## Modèle vierge

| Élément de données | Lieu de stockage | Responsable | Personnel / Sensible ? | Qui peut y accéder | État de la sauvegarde | Conservation |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Exemple rempli

| Élément de données | Lieu de stockage | Responsable | Personnel / Sensible ? | Qui peut y accéder | État de la sauvegarde | Conservation |
|---|---|---|---|---|---|---|
| Liste de contacts clients | CRM (cloud) | Responsable des ventes | Personnel (noms, e-mails, téléphones) | Équipe commerciale (modification), Finance (lecture) | Quotidienne, hors site | Tant que actif + 3 ans |
| Fichier de paie | Disque partagé, dossier « RH » | Responsable RH | Sensible (salaire, pièce d'identité, banque) | RH uniquement | Hebdomadaire, hors site | 10 ans (légal) |
| Contrats fournisseurs | Armoire papier + dossier scanné | Dirigeant | Ni l'un ni l'autre (confidentiel commercial) | Dirigeant, Finance | Partielle (scans seulement) | Durée du contrat + 6 ans |

## Où chercher les données

Parcourez chacun de ces endroits. Les données se cachent en pleine vue :

- [ ] Boîtes e-mail partagées et messageries personnelles.
- [ ] Disques partagés et dossiers réseau.
- [ ] Outils cloud : CRM, comptabilité, RH, outils de projet.
- [ ] Tableurs et pièces jointes (souvent le plus désordonné).
- [ ] Dossiers papier, armoires et copies scannées.
- [ ] Sauvegardes et anciens exports.
- [ ] Outils de discussion et historique des messages.
- [ ] Téléphones et ordinateurs portables du personnel.
- [ ] Outils tiers auxquels le personnel s'est inscrit de son propre chef (copies fantômes).

## Ce qui compte comme « Sensible »

Sous le RGPD, ces catégories particulières exigent une attention supplémentaire. Marquez-les clairement :

- Données de santé
- Origine raciale ou ethnique
- Opinions politiques
- Croyances religieuses ou philosophiques
- Appartenance syndicale
- Données génétiques et biométriques (pour l'identification)
- Vie sexuelle ou orientation sexuelle

Traitez aussi comme sensible, même sans être une « catégorie particulière » : coordonnées bancaires, numéros de pièce d'identité, mots de passe, données d'enfants, et tout ce qui pourrait nuire à une personne en cas de fuite.

## Guide des colonnes

- **Élément de données** — Un nom simple pour la chose (pas le nom du fichier).
- **Lieu de stockage** — Système et emplacement : outil cloud, chemin du disque, armoire papier.
- **Responsable** — Une seule personne redevable de cet élément.
- **Personnel / Sensible ?** — Personnel, Sensible, ou Ni l'un ni l'autre.
- **Qui peut y accéder** — Rôles ou personnes, et s'ils peuvent lire ou modifier.
- **État de la sauvegarde** — À quelle fréquence elle est sauvegardée, et où. Notez s'il n'y a **pas** de sauvegarde.
- **Conservation** — Combien de temps vous le gardez, et pourquoi (règle légale ou besoin commercial).

## Signaux d'alerte à corriger maintenant

- [ ] Données sensibles sans responsable.
- [ ] Données sensibles que n'importe qui dans l'entreprise peut ouvrir.
- [ ] Données importantes sans sauvegarde.
- [ ] Données conservées « pour toujours » sans raison.
- [ ] Données personnelles dans un outil que vous ne contrôlez pas (IA fantôme, e-mail personnel).
- [ ] La même donnée à plusieurs endroits sans copie maîtresse.

## Règles de bon sens pour la conservation

- Ne gardez les données que le temps nécessaire. Plus long n'est pas plus sûr — c'est plus de risque.
- Vérifiez les durées légales minimales : les registres fiscaux et de paie ont souvent des années fixes. Demandez à votre comptable.
- Pour les données clients, gardez-les tant que la relation est active, puis une courte période annoncée.
- Supprimez ou anonymisez les données dont vous n'avez plus besoin. Ne les laissez pas s'accumuler.
- Écrivez la raison de chaque durée de conservation, pour que personne n'ait à deviner plus tard.

## Garder l'inventaire à jour

- Relisez-le tous les 6 mois, et avant tout nouveau projet d'IA.
- Ajoutez une ligne le jour où un nouvel outil ou une nouvelle source de données apparaît.
- Nommez un responsable par élément ; les responsables garantissent l'honnêteté.
- Traitez-le comme un document vivant, pas corvée unique.

## Règle pour les projets d'IA

Avant que la moindre donnée n'entre dans un outil d'IA, vérifiez cet inventaire. Si un élément est **Sensible**, il vous faut une raison claire, un outil sûr, et souvent une AIPD. Dans le doute, laissez-le de côté.
