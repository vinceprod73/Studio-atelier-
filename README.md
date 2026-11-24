# Atelier HTML v4.0 PRO

**Studio IA multi-langages 100 % navigateur** — génère, édite, prévisualise et exporte du code professionnel en un clic.

[![Version](https://img.shields.io/badge/version-4.0%20PRO-fcee0a?style=flat-square)](https://github.com)
[![Licence](https://img.shields.io/badge/licence-MIT-00f0ff?style=flat-square)](LICENSE)
[![Navigateur](https://img.shields.io/badge/navigateur-Chrome%20%7C%20Firefox%20%7C%20Edge%20%7C%20Safari-39ff14?style=flat-square)](#)
[![Offline](https://img.shields.io/badge/mode-hors--ligne%20possible-ff003c?style=flat-square)](#)

Créé par **Vince Prod 73**

---

## Présentation

**Atelier HTML** est un studio de développement autonome qui tourne entièrement dans le navigateur.  
Il permet de créer, modifier, tester et exporter du code dans plus de **30 langages**, avec l’aide d’intelligences artificielles (gratuites ou locales).

Aucun serveur à installer, aucun compte obligatoire.  
Ouvre le fichier HTML et commence à coder.

### Points forts

- Génération de code complet et fonctionnel (pas de placeholders)
- Aperçu live pour les pages HTML (Bureau / Tablette / Mobile)
- Édition directe du code avec application immédiate
- Import de fichiers existants (glisser-déposer + fusion HTML/CSS/JS)
- Extraction séparée `index.html` + `style.css` + `app.js`
- Recherche d’inspirations open source (Codeberg + GitLab)
- Sauvegarde locale des projets dans le navigateur
- Auto-réparation intelligente en cas d’erreur détectée
- Mode hors-ligne avec secours local si aucune IA n’est joignable
- Modèles de démarrage riches (Kanban, analyseur CSV Python, config JSON…)

---

## Langages supportés

| Catégorie | Langages |
|-----------|----------|
| **Web** | HTML / CSS / JS, CSS pur, JSON, YAML, Markdown |
| **Script** | Python, JavaScript, TypeScript, PHP, Ruby, Lua, Bash, PowerShell |
| **Systèmes** | C, C++, C#, Rust, Go, Java, Kotlin, Swift |
| **Données & Science** | SQL, R, Julia |
| **Autres** | Dart, Scala, Haskell, Perl, Elixir, Clojure, Assembly (x86_64) |

---

## Moteurs IA supportés

| Fournisseur | Type | Clé API |
|-------------|------|--------|
| **IA Automatique** | Gratuit + secours local | Optionnelle (Pollinations) |
| **Ollama** | Local (`localhost:11434`) | Non |
| **LM Studio** | Local (`localhost:1234`) | Non |
| **llama.cpp** | Local (`localhost:8080`) | Non |
| **LocalAI** | Local (`localhost:8080`) | Non |
| **vLLM / SGLang** | Local (`localhost:8000`) | Non |
| **Google Gemini** | Cloud (gratuit) | Oui |
| **Groq** | Cloud (gratuit) | Oui |
| **OpenAI** | Cloud | Oui (`sk-...`) |

Le mode **IA Automatique** essaie d’abord les services gratuits en ligne, puis bascule automatiquement sur Ollama local, et enfin sur un générateur hors-ligne de secours.

---

## Démarrage rapide

### 1. Télécharger

```bash
git clone https://github.com/VOTRE-USERNAME/atelier-html-v4.git
cd atelier-html-v4
```

Ou télécharge simplement le fichier `atelier-html-v4-0-pro.html`.

### 2. Ouvrir

Double-clique sur le fichier HTML  
**ou** ouvre-le dans ton navigateur préféré :

```bash
# Exemple avec un serveur local simple (optionnel)
python -m http.server 8080
# Puis ouvre http://localhost:8080/atelier-html-v4-0-pro.html
```

### 3. Utiliser

1. Choisis un **langage** (ou clique sur **Coder Python**)
2. Décris ce que tu veux créer dans la zone de texte
3. Clique sur **Générer le code**
4. Édite, prévisualise, exporte ou sauvegarde

---

## Fonctionnalités détaillées

### Génération & édition
- Prompt en langage naturel (français ou anglais)
- Génération streaming en temps réel
- Éditeur de code intégré avec application immédiate
- Bouton **Relire & corriger** (analyse + correction IA)
- Historique d’annulation (`Annuler`)
- Mode rapide (génération plus compacte)

### Aperçu HTML
- Iframe sandboxed avec sonde d’erreurs runtime
- Modes **Bureau / Tablette / Mobile**
- Auto-réparation si erreur JavaScript détectée (jusqu’à 2 tentatives)

### Import
- Glisser-déposer d’un fichier
- Sélection multiple + fusion automatique HTML + CSS + JS
- Collage direct de code
- Détection automatique du langage

### Extraction (mode HTML)
- Sépare automatiquement :
  - Structure HTML (avec liens relatifs)
  - Feuille de style CSS
  - Logique JavaScript
- Téléchargement individuel ou des 3 fichiers

### Open Source
- Recherche sur **Codeberg** et **GitLab**
- Inspiration directe dans le prompt de génération

### Projets locaux
- Sauvegarde dans `localStorage` (jusqu’à 20 projets)
- Rechargement et téléchargement en un clic
- Compteur de projets visible dans l’interface

### Diagnostic
- Tests automatisés du catalogue multi-langages
- Vérification de la structure HTML
- Test de l’extracteur HTML/CSS/JS
- Test de connectivité IA
- Test de persistance locale

---

## Raccourcis clavier

| Raccourci | Action |
|-----------|--------|
| `Ctrl` + `Entrée` | Lancer la génération |
| `Échap` | Annuler le lancement automatique (4 s) |
| `Ctrl` + `Entrée` (dans l’éditeur) | Appliquer les modifications |

---

## Structure du projet

```text
atelier-html-v4/
├── atelier-html-v4-0-pro.html   # Application complète (tout-en-un)
├── README.md                    # Ce fichier
└── LICENSE                      # Licence MIT (recommandée)
```

Le fichier HTML contient :
- L’interface complète (CSS + HTML)
- Toute la logique JavaScript
- Les recettes spécialisées (jeux, quiz, dictionnaire, etc.)
- Les modèles de démarrage
- Le système de secours hors-ligne

---

## Notes techniques

- **Stockage local** : les projets et les clés API sont sauvegardés dans `localStorage` du navigateur.
- **Sécurité** : l’aperçu HTML tourne dans une iframe sandboxed (`allow-scripts allow-forms allow-modals`).
- **Hors-ligne** : si aucune IA n’est joignable, un générateur de secours produit un fichier minimal fonctionnel.
- **Pas de backend** : tout s’exécute côté client.

---

## Captures d’écran

> *Ajoute ici tes captures d’écran une fois le dépôt créé.*

```text
![Aperçu principal](docs/screenshot-main.png)
![Éditeur de code](docs/screenshot-editor.png)
![Import de fichiers](docs/screenshot-import.png)
![Extraction HTML/CSS/JS](docs/screenshot-extract.png)
```

---

## Contribution

Les contributions sont les bienvenues !

1. Fork le projet
2. Crée une branche (`git checkout -b feature/ma-fonctionnalite`)
3. Commit tes changements (`git commit -m 'Ajout de ma fonctionnalité'`)
4. Push (`git push origin feature/ma-fonctionnalite`)
5. Ouvre une Pull Request

---

## Licence

Ce projet est distribué sous licence **MIT**.

Tu es libre de l’utiliser, le modifier et le redistribuer, y compris à des fins commerciales, à condition de conserver la mention d’auteur.

```text
Copyright (c) 2025-2026 Vince Prod 73
```

---

## Crédits

- **Auteur** : Vince Prod 73
- **Inspiration** : les outils de développement modernes + l’IA générative
- **Moteurs IA** : Pollinations, Ollama, LM Studio, Gemini, Groq, OpenAI et autres compatibles OpenAI API

---

## Liens utiles

- [Ollama](https://ollama.com) — modèles locaux gratuits
- [LM Studio](https://lmstudio.ai) — interface locale pour LLMs
- [Google AI Studio](https://aistudio.google.com/apikey) — clé Gemini gratuite
- [Groq Console](https://console.groq.com/keys) — clé Groq gratuite
- [Codeberg](https://codeberg.org) — forge open source
- [GitLab](https://gitlab.com) — forge open source

---

**Atelier HTML v4.0 PRO** — Studio IA Multi-Langages & Autonome  
*Crée. Édite. Exporte. Sans friction.*
