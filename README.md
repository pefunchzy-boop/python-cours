# 🐍 Python, pas à pas

Une petite application web (un seul `index.html`, aucune installation) pour apprendre Python quand on débute. Elle fonctionne directement dans le navigateur, sur ordinateur comme sur mobile, et les fonctions IA tournent avec ta propre clé Gemini.

**Lien en ligne :** <https://pefunchzy-boop.github.io/python-cours/>

## ✨ Les 4 onglets

### 📘 Cours
6 leçons progressives : Variables, Conditions, Boucles, Listes et dictionnaires, Fonctions, Fichiers et erreurs. Chaque leçon contient :
- une explication simple de la notion,
- un exemple de code,
- un exercice à faire toi-même,
- et un tuteur IA avec qui discuter. Le tuteur ne donne jamais la solution : il pose des questions et donne des indices de plus en plus précis, pour que tu trouves tout seul.

### 📋 Commandes
Un aide-mémoire de toutes les commandes Python de base (print, boucles, listes, chaînes, dictionnaires, fichiers, classes…), classées par catégorie, avec une barre de recherche. Clique sur une commande pour la copier dans le presse-papier.

### 🐞 Debug
Colle un message d'erreur Python (le Traceback complet, ou juste la dernière ligne) et éventuellement ton code. L'IA t'explique ce que veut dire l'erreur, où ça coince, les causes probables, et une piste pour corriger.

### 🔍 Syntaxe
Colle ton code. L'app fait d'abord une vérification locale instantanée (deux-points manquants, `=` au lieu de `==`, parenthèses non refermées, tabulations mélangées aux espaces…), puis l'IA relit le code et signale les pièges classiques (variables non définies, types mélangés, boucles infinies…) sans te donner la correction toute faite.

## 🔑 Configuration

Les fonctions IA demandent une clé Gemini :
1. Onglet Cours → bouton « Clé Gemini ».
2. Colle ta clé (gratuite sur [Google AI Studio](https://aistudio.google.com/apikey)).
3. La clé est stockée uniquement sur ton appareil (localStorage), jamais envoyée ailleurs qu'à l'API Google. Choisis aussi le modèle dans le menu déroulant.

Sans clé, les leçons, l'aide-mémoire et la vérification syntaxique locale fonctionnent quand même.

## 🛠️ Technique

- Zéro dépendance : un fichier `index.html` unique, HTML + CSS + JavaScript vanilla.
- Mode sombre automatique selon les réglages de ton système.
- Historique de conversation avec le tuteur, remise à zéro possible.
- Appels à l'API Gemini (`generateContent`) directement depuis le navigateur avec ta clé.

## 🚀 Hébergement

Le site est publié sur GitHub Pages. Pour le mettre à jour, push simplement sur `main` : le contenu de la branche est servi tel quel (rien à compiler).
