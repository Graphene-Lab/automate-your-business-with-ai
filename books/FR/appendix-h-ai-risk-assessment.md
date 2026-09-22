# Annexe H — Évaluation des risques liés à l'IA

Avant de lancer un projet d'IA, demandez-vous ce qui pourrait mal tourner et à quel point ce serait grave. Ce tableau rend les risques visibles pour que vous puissiez les réduire, pas les ignorer. Remplissez-le avec votre équipe. Faites-le tôt, et reprenez-le souvent.

## Comment noter

Notez chaque risque sur deux échelles :

- **Vraisemblance** — À quel point est-ce probable ? **Faible / Moyenne / Élevée**
- **Impact** — À quel point est-ce grave si cela arrive ? **Faible / Moyen / Élevé**

Combinez-les en un **Niveau de risque** :

| | Impact faible | Impact moyen | Impact élevé |
|---|---|---|---|
| **Vraisemblance élevée** | Moyen | Élevé | **Critique** |
| **Vraisemblance moyenne** | Faible | Moyen | Élevé |
| **Vraisemblance faible** | Faible | Faible | Moyen |

Traitez **Critique** et **Élevé** comme des points à corriger avant le lancement.

## Modèle vierge

| Risque | Ce qui pourrait mal tourner | Vraisemblance | Impact | Niveau de risque | Mesure d'atténuation | Responsable |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Exemples remplis

| Risque | Ce qui pourrait mal tourner | Vraisemblance | Impact | Niveau de risque | Mesure d'atténuation | Responsable |
|---|---|---|---|---|---|---|
| Mauvaises données dans l'IA | Le personnel colle des données personnelles de clients dans un outil public | Élevée | Élevé | **Critique** | Liste d'outils approuvés uniquement ; bloquer les outils publics sur les appareils de l'entreprise ; formation | Responsable informatique |
| Résultat erroné utilisé | L'IA rédige une facture avec un montant faux, envoyée au client | Moyenne | Élevé | Élevé | Revue humaine avant l'envoi ; contrôle automatique des totaux | Comptable |
| Biais dans les décisions | Un outil de recrutement favorise un groupe à cause de données d'entraînement faussées | Moyenne | Élevé | Élevé | L'humain décide ; examiner les résultats pour l'équité ; éviter un recrutement entièrement automatisé | Responsable RH |
| Fuite chez le fournisseur | Le prestataire est piraté et les données clients sont exposées | Faible | Élevé | Moyen | Liste de contrôle du fournisseur ; chiffrer les données ; clause contractuelle de notification de violation | Responsable informatique |
| Surdépendance | Le personnel arrête de vérifier et fait aveuglément confiance à l'IA | Moyenne | Moyen | Moyen | Garder la signature humaine ; audits ponctuels ; formation sur les limites | Manager d'équipe |
| Injection de prompt | Un document cache des instructions qui trompent l'IA | Moyenne | Moyen | Moyen | Traiter le texte extérieur comme non fiable ; limiter ce que l'IA peut en faire | Responsable informatique |
| Dépendance (lock-in) | Impossible de quitter le fournisseur ou d'exporter les données | Faible | Moyen | Moyen | Clause d'export des données dans le contrat ; garder une copie | Dirigeant |
| Dépassement de budget | L'usage augmente et la facture grimpe | Moyenne | Moyen | Moyen | Définir des alertes d'usage ; revoir le plan chaque mois ; plafonner le coût par tâche | Dirigeant |
| Dérive du modèle | Le prestataire change le modèle et la qualité du résultat baisse | Moyenne | Moyen | Moyen | Contrôler ponctuellement le résultat chaque semaine ; garder des cas de test pour comparer | Manager d'équipe |

## Guide des colonnes

- **Risque** — Un nom court pour le risque.
- **Ce qui pourrait mal tourner** — Le scénario concret, pas une inquiétude vague.
- **Vraisemblance / Impact** — Faible / Moyen / Élevé.
- **Niveau de risque** — D'après la grille ci-dessus.
- **Mesure d'atténuation** — Ce que vous ferez pour baisser la vraisemblance ou l'impact.
- **Responsable** — La seule personne qui fait en sorte que la mesure soit appliquée.

## Risques liés à l'IA à envisager

Utilisez cette liste pour faire naître vos propres lignes :

- [ ] Données personnelles ou sensibles divulguées à un outil extérieur.
- [ ] Résultat incorrect cru sans revue.
- [ ] Biais ou injustice dans les décisions automatisées.
- [ ] Violation de sécurité chez le fournisseur.
- [ ] Injection de prompt depuis des documents non fiables.
- [ ] IA fantôme (shadow AI) — personnel utilisant des outils non approuvés.
- [ ] Surdépendance et perte de compétences.
- [ ] Dépassement de budget à mesure que l'usage croît.
- [ ] Dépendance (lock-in) à un seul prestataire.
- [ ] Non-conformité au RGPD ou à l'AI Act (règlement européen sur l'IA).
- [ ] Confiance du client perdue après une erreur visible.
- [ ] Changements silencieux du modèle et baisse de la qualité du résultat.

## Quand refaire cette évaluation

Reprenez le tableau quand l'un de ces événements se produit :

- Vous ajoutez un nouvel outil, une nouvelle source de données ou un nouveau processus.
- L'usage augmente beaucoup, ou l'outil touche plus de personnes.
- Un incident ou un quasi-accident survient.
- Une loi ou une exigence client change.
- Un fournisseur change ses conditions, son modèle ou l'endroit où il stocke les données.

## Deux façons de réduire un risque

Chaque mesure d'atténuation agit sur l'un de deux leviers :

- **Baisser la vraisemblance** — rendre l'événement fâcheux moins probable. Exemple : une liste d'outils approuvés uniquement rend une fuite de données moins probable.
- **Baisser l'impact** — rendre les dégâts plus petits si cela arrive. Exemple : une revue humaine fait qu'une facture erronée est repérée avant d'atteindre le client.

Un bon plan agit souvent sur les deux. Pour chaque risque, demandez-vous : « Qu'est-ce qui rend cela moins probable, et qu'est-ce qui limite le dommage si cela arrive quand même ? »

Si un risque reste **Critique** même après atténuation, ne lancez pas. Supprimez l'étape risquée ou repensez le processus.

## Règles

- Chaque risque Critique ou Élevé a besoin d'une mesure d'atténuation **et** d'un responsable avant le lancement.
- Une mesure d'atténuation sans responsable n'est pas une mesure d'atténuation.
- Refaites cette évaluation à chaque étape — les risques évoluent.
- Si un risque Critique ne peut pas être réduit, ne lancez pas. Dites-le.
