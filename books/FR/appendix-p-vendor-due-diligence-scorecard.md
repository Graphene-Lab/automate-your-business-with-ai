# Annexe P — Tableau d'évaluation d'un fournisseur d'IA

Utilisez-le pour comparer les fournisseurs avec des chiffres, pas à l'intuition. Chaque critère a une **pondération** (à quel point il compte pour vous). Notez chaque fournisseur de **1 à 5**. Le total pondéré donne un seul chiffre à comparer. Remplissez un tableau par fournisseur, puis placez-les côte à côte.

## Comment noter

- **Pondération** = à quel point le critère est important. Les pondérations font 100 au total. Changez-les pour les adapter à votre entreprise.
- **Note** = de 1 (mauvais) à 5 (excellent) selon la façon dont le fournisseur remplit le critère.
- **Score pondéré** = pondération × (note ÷ 5). Cela garde le total sur 100.

> **Score pondéré = Pondération × (Note ÷ 5)**
> **Total = somme de tous les scores pondérés (sur 100)**

## Tableau vierge

**Fournisseur :** ______________________  **Date :** ____________  **Noté par :** ____________

| Critère | Pondération | Note (1–5) | Score pondéré | Notes |
|---|---|---|---|---|
| Sécurité | 20 |  |  |  |
| Confidentialité et conformité | 20 |  |  |  |
| Transparence | 10 |  |  |  |
| Tarifs | 15 |  |  |  |
| Support | 15 |  |  |  |
| Sortie et dépendance (lock-in) | 15 |  |  |  |
| Références et réputation | 5 |  |  |  |
| **Total** | **100** |  |  |  |

## Ce que signifie chaque critère

- **Sécurité** — MFA, contrôle d'accès, journaux d'audit, notification de violation, protection contre les attaques.
- **Confidentialité et conformité** — conformité au RGPD, données non utilisées pour entraîner des modèles partagés, localisation des données, accord de traitement des données proposé.
- **Transparence** — Réponses claires, honnête sur les limites, ouvert sur les sous-traitants et les changements de modèle.
- **Tarifs** — Clairs, prévisibles quand vous grandissez, pas de frais cachés, prix de renouvellement équitable.
- **Support** — Vrais canaux, délais de réponse écrits, intégration, promesse de disponibilité.
- **Sortie et dépendance (lock-in)** — Résiliation facile, export des données dans un format utilisable, premier contrat court, vous gardez la propriété.
- **Références et réputation** — Avis ou références d'entreprises comme la vôtre, ancienneté suffisante pour être tenu responsable.

## Exemple rempli

**Fournisseur :** InvoiceFlow AI (exemple)  **Date :** 2026-09-15  **Noté par :** Propriétaire

| Critère | Pondération | Note (1–5) | Score pondéré | Notes |
|---|---|---|---|---|
| Sécurité | 20 | 4 | 16 | MFA oui, journaux d'audit oui, notification de violation 72 h. |
| Confidentialité et conformité | 20 | 3 | 12 | Accord de traitement proposé, mais données stockées hors UE — à revoir. |
| Transparence | 10 | 4 | 8 | Docs claires, honnête sur les limites. |
| Tarifs | 15 | 3 | 9 | Clair pour l'instant, mais le renouvellement bondit de 40 %. |
| Support | 15 | 5 | 15 | Chat 24h/24, réponse en 2 h, bonne intégration. |
| Sortie et dépendance (lock-in) | 15 | 2 | 6 | Export CSV oui, mais dépendance (lock-in) de 12 mois avec frais. |
| Références et réputation | 5 | 4 | 4 | Bons avis d'entreprises similaires. |
| **Total** | **100** |  | **70** | Bon produit, faible sur la sortie et la localisation des données. |

**Lecture de l'exemple :** 70/100 est un fournisseur correct avec deux vrais problèmes — la localisation des données (confidentialité) et une dépendance coûteuse (sortie). Le propriétaire ne doit pas signer le contrat de 12 mois tel quel. Corrigez les conditions de sortie et confirmez la localisation des données, ou cherchez ailleurs.

## Comment lire le total

| Total | Signification |
|---|---|
| 85–100 | Candidat solide. Passez à un projet pilote. |
| 70–84 | Bien, mais corrigez d'abord les points peu notés. |
| 55–69 | Faible. Demandez plus ou cherchez ailleurs. |
| En dessous de 55 | Rejetez. Trop de lacunes. |

## La règle d'arbitrage

Un total élevé peut cacher un défaut fatal. **Ignorez le total et partez si l'un de ceux-ci obtient 1 :**

- **Sécurité = 1** — Ils ne peuvent pas protéger vos données.
- **Confidentialité et conformité = 1** — Ils vont mal utiliser ou mal traiter vos données.
- **Sortie et dépendance (lock-in) = 1** — Vous ne pouvez pas récupérer vos données ni partir.

Ce ne sont pas des compromis. Un prix formidable ne répare pas un fournisseur qui ne vous laisse pas partir ou qui divulgue vos données.

## Comparer deux fournisseurs côte à côte

Mettez ensemble les totaux et les drapeaux d'arbitrage :

| Critère | Fournisseur A | Fournisseur B |
|---|---|---|
| Total (sur 100) | 70 | 66 |
| Un drapeau d'arbitrage (Séc/Conf/Sortie = 1) ? | Non | Oui (Sortie = 1) |
| Décision | Projet pilote pour A | Rejeter B — impossible de sortir |

Ici le fournisseur A gagne même avec un petit écart de total, parce que le fournisseur B échoue à la règle d'arbitrage.

## Conseils

- **Définissez les pondérations avant de noter.** Décidez d'abord ce qui compte, pour que la note ne soit pas pliée pour convenir à un fournisseur que vous aimez.
- **Notez avec des preuves**, pas avec du charme. Utilisez les réponses de l'Annexe K et la liste de contrôle de l'Annexe B.
- **Notez chaque fournisseur de la même façon.** La cohérence est ce qui rend les totaux comparables.
- **Renez après l'essai.** L'usage réel change souvent les chiffres.
