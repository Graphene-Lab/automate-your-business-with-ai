# Annexe M — Ressources, lectures et outils recommandés

Une liste courte et honnête d'outils et de lectures. Ce ne sont **pas** des publicités. Ce sont de vrais projets, nommés, que vous pouvez vérifier vous-même. La plupart sont open source, ce qui signifie que vous pouvez voir comment ils fonctionnent et que vous n'êtes pas lié à une seule entreprise.

**Une note sur le niveau de compétence :** Certains outils ici demandent une personne technique (un partenaire informatique, un développeur ou un collaborateur à l'aise avec la technique). Vous n'avez pas besoin de les faire tourner vous-même. Lisez-les pour savoir ce qui est possible et pour parler intelligemment avec celui qui les met en place.

**Vérifié :** Chaque outil et chaque livre ci-dessous a été contrôlé sur son propre site web ou son dépôt de code en **septembre 2026**. Les outils évoluent vite — revérifiez avant d'adopter.

## Faire tourner l'IA en local (sur vos propres machines)

Faire tourner des modèles en local signifie que l'IA travaille sur votre propre ordinateur ou serveur. Vos données ne quittent pas votre machine. C'est l'option la plus privée.

- **Ollama** — `ollama.com`. Un outil gratuit et open source pour faire tourner des modèles d'IA ouverts sur votre propre ordinateur. Les modèles locaux ne coûtent rien et gardent les données sur votre machine. C'est le point de départ le plus simple pour une IA locale, et il sert souvent de moteur derrière d'autres outils.
- **Thunderbolt** — `thunderbolt.io` (code : `github.com/Thunderbird/thunderbolt`). Un **client d'IA** open source et auto-hébergeable de MZLA Technologies, la filiale de Mozilla qui fait aussi Thunderbird. Annoncé en avril 2026 et sous licence Mozilla Public License 2.0. Sa promesse est « une IA que vous contrôlez : choisissez vos modèles, possédez vos données, éliminez la dépendance (lock-in) ». Il fonctionne sur web, Windows, macOS, Linux, iOS et Android, et marche avec des modèles locaux, sur site ou dans le cloud. Pour l'usage local, il pointe vers Ollama ou llama.cpp. **Statut :** en phase précoce et sous audit de sécurité — considérez-le comme prometteur, pas terminé.
- **llama.cpp** — un moteur open source bien connu qui fait tourner de grands modèles sur du matériel informatique ordinaire, y compris votre propre ordinateur portable. C'est le moteur technique sur lequel d'autres construisent. Mentionné ici parce que Thunderbolt le recommande pour une inférence locale gratuite.

**Quand choisir le local :** vous traitez des données sensibles, vous voulez éviter les frais par message, ou vous avez besoin que l'IA fonctionne sans envoyer de données. La contrepartie : vous payez le matériel et la mise en place, et les modèles locaux sont généralement plus petits que les plus gros modèles du cloud.

## Construire des automatisations (connecter l'IA à votre travail)

Ces outils vous permettent d'intégrer l'IA à de vraies tâches — lire des documents, répondre à des tickets, déplacer des données entre applications.

- **Haystack** — `haystack.deepset.ai` (code : `github.com/deepset-ai/haystack`). Un framework open source de **deepset** (Allemagne) pour construire des applications d'IA, en particulier des pipelines **RAG**. RAG (« génération augmentée par récupération ») signifie que l'IA consulte vos propres documents avant de répondre, donc elle répond à partir de vos faits, pas de suppositions. Gratuit à installer (`pip install haystack-ai`) ; un support entreprise payant est optionnel. Convient mieux à une équipe avec un développeur.
- **n8n** — `n8n.io`. Une plateforme d'automatisation **fair-code** (le code est public sur GitHub) qui vous permet de construire des workflows sur un canevas visuel et de vous connecter à plus de 500 applications. Elle construit aussi des agents IA et des systèmes RAG, avec des validations humaines dans la boucle. Vous pouvez l'auto-héberger ou utiliser leur cloud. « Fair-code » signifie que le code est ouvert à la lecture et à l'auto-hébergement, mais ce n'est pas une licence open source standard — vérifiez les conditions si vous prévoyez de le revendre.

**Quand les choisir :** vous voulez que l'IA agisse sur vos données à travers plusieurs applications, pas seulement discuter. Haystack sert à construire des pipelines d'IA sur mesure ; n8n sert à connecter des applications et à automatiser des étapes avec l'IA dedans.

## Pour aller plus loin (lectures)

- **Headcount Zero: How to Build an AI-Run Company with Paperclip** — par **Anthony David Adams**. Un livre open source (sur GitHub, licence CC BY-NC-SA 4.0) sur la gestion d'une entreprise où les agents IA font la plupart du travail et où un petit nombre d'humains jugent le résultat. Il couvre l'idée de « l'entreprise d'une seule personne », le fonctionnement des agents IA, l'économie d'un effectif réduit, et la façon de gouverner l'IA avec des interrupteurs d'arrêt (kill-switch). Lisez-le pour la vision audacieuse — puis appliquez-la avec la prudence que ce livre enseigne : gardez les humains aux commandes de ce qui compte.
- **Les chapitres de ce livre eux-mêmes** — la meilleure « lecture complémentaire » est souvent les chapitres que vous avez survolés. Relisez le chapitre sur les risques avant tout lancement, et le chapitre sur les données avant de connecter un outil à de vraies données clients.
- **La documentation des fournisseurs et des projets** — pour tout outil ci-dessus, lisez la documentation et la licence du projet avant d'adopter. Elles vous disent ce qui est gratuit, ce qui est payant, et ce à quoi vous consentez.

## Comment choisir, en trois questions

1. **Où les données doivent-elles rester ?** Si elles ne doivent pas quitter vos machines, regardez les outils locaux (Ollama, Thunderbolt, llama.cpp).
2. **Avez-vous une aide technique ?** Si oui, Haystack et n8n ouvrent le plus de portes. Si non, commencez par un outil hébergé simple et un petit projet pilote.
3. **Pouvez-vous partir plus tard ?** Préférez les outils qui vous permettent d'exporter vos données et de changer de modèle. Évitez tout ce qui enferme vos données.

## Une mise en garde sur les listes comme celle-ci

Les outils montent et retombent. Un nom ici peut changer, fusionner ou disparaître en un an. C'est normal dans l'IA. Les **principes** de ce livre — garder les données privées, garder un humain dans la boucle, mesurer les résultats, éviter la dépendance (lock-in) — survivent à n'importe quel outil. Utilisez cette liste comme une carte, pas comme une promesse.
