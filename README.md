# Extension Antispoil Multi-Plateforme

> **Naviguez sur le web sans crainte d'être spoilé !**  
> Une extension navigateur ultra-légère en JavaScript qui masque et floute automatiquement les contenus sensibles (titres, miniatures, vidéos, posts) en fonction de vos mots-clés.

> 🚧 **Statut du projet :** **En cours de développement (WIP)**. Les fonctionnalités de base (floutage, défloutage, stockage local des tags) sont opérationnelles. L'extension est régulièrement enrichie de nouvelles optimisations de détection DOM.

---

## 📌 Présentation

**Extension web conçue pour protéger les utilisateurs contre les divulgâches (spoilers) de séries, films, jeux vidéo ou événements sportifs sur leurs réseaux sociaux et sites préférés (YouTube, Twitter/X, Reddit, Facebook, sites d'actualités...).

Grâce à un système d'analyse en temps réel du DOM, l'extension floute instantanément les éléments contenant vos tags sensibles tout en vous laissant la possibilité de **déflouter un contenu d'un simple clic ou survol** si vous souhaitez le révéler.

---

## ✨ Fonctionnalités

- 🏷️ **Gestion de Tags Personnalisés** : Ajoutez ou supprimez vos mots-clés facilement depuis le popup de l'extension (ex: `Avengers`, `GTA 6`, `House of the Dragon`).
- 👁️ **Floutage Intelligent (Blur & Unblur)** : 
  - Floutage automatique des titres, paragraphes, cartes, vidéos et miniatures (thumbnails).
  - **Action pour révéler** : Cliquez ou survolez un élément flouté pour afficher temporairement le contenu.
- 🌐 **Multi-Plateforme & Universel** : Conçu pour fonctionner dynamiquement sur n'importe quel site web (compatible Chromium & Firefox).
- ⚡ **Ultra-Léger & Performant** : Développé en **Pure JavaScript (Vanilla JS)** sans aucun framework lourd ni dépendance externe.
- 🔒 **Respect de la Vie Privée** : Vos tags sont stockés à 100% en local (`chrome.storage` / `browser.storage`). Aucune donnée n'est envoyée vers un serveur distant.

---

## 🛠️ Stack Technique

| Composant | Technologie / API | Rôle |
| :--- | :--- | :--- |
| **Langage** | **Vanilla JavaScript (ES6+)** | Logique métier, manipulation du DOM et stockage |
| **API WebExtensions** | `chrome.storage` / `browser.storage` | Sauvegarde locale des tags utilisateur |
| **Analyse DOM** | `MutationObserver` | Détection dynamique des nouveaux contenus injectés (scroll infini) |
| **UI & Style** | **HTML5 & CSS3** | Interface du popup et filtres CSS de floutage (`backdrop-filter` / `filter`) |

---
