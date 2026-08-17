# 👋 Portfolio — Théo Marme

Développeur **full-stack** avec 7 ans d'expérience (web, outils de pilotage, intégration de solutions IA). J'aime prendre un problème concret et le porter jusqu'à un outil qui fonctionne vraiment.

Ces projets personnels sont aussi mon **terrain d'expérimentation** : ils me servent à me former en continu aux **nouvelles technologies d'IA** (LLM appliqués, génération d'images, transcription audio) et à explorer des stacks que je n'utilise pas au quotidien (Rust, Tauri, Electron).

**Stacks principales :** Rust · Python · TypeScript / React · Node.js · Tauri · Electron
**Domaines :** applications desktop, full-stack web temps réel, IA / audio / 3D

> Ce dépôt est une **vitrine** : il présente mes projets. Le code de certains projets reste privé (données personnelles ou travail en cours) — je peux le présenter avec plaisir sur demande.

---

## ⭐ Projets phares

### 🏠 Marme Estate — Gestion de biens immobiliers
Application **desktop** complète pour gérer un parc locatif de bout en bout : locataires, loyers, charges, syndic, suivi de prêt bancaire (calcul automatique du taux et de l'assurance) et **rentabilité** (brute, nette, cash-on-cash).

- 🔐 Gestion documentaire **chiffrée** (AES-GCM côté client) : bail, DPE, photos
- 🤖 **Lecture de factures par IA** (catégorie / montant / date suggérés automatiquement)
- ☁️ Synchronisation cloud chiffrée entre utilisateurs de confiance
- ✅ ~40 tests automatisés, en usage réel

`Tauri v2` · `Rust` · `JavaScript (ES modules)` · `Vite` · `Supabase (Postgres / Auth / Storage / Edge Functions)` · `Vitest`
*Code privé (données sensibles) — démo sur demande.*

### 🎵 Hook Detector — Extraction de hook & génération de Reels
Outil pour musiciens qui **détecte automatiquement le passage le plus accrocheur** d'un morceau, puis en génère une vidéo verticale (9:16) prête à publier sur Instagram.

- 🎯 Analyse audio (similarité chroma + énergie RMS, calée sur le tempo) → 3-4 candidats classés
- 🎬 4 styles de Reel : image animée (effet parallaxe 2.5D), carte façon lecteur Spotify, vinyle, karaoké
- 🧠 **IA locale sur GPU** : Stable Diffusion XL (image), Whisper (paroles), Depth-Anything V2 (profondeur)
- 📱 Récupération de la vidéo sur mobile via QR code en réseau local

`Python` · `Flask` · `PyTorch (CUDA)` · `librosa` · `ffmpeg` · `OpenCV` · `Pillow`

### 🗂️ File Lab — Conversion & gestion de fichiers multi-formats
Application **desktop** tout-en-un qui **détecte automatiquement le type d'un fichier** et propose les conversions, compressions et modifications pertinentes. Multi-formats : PDF, images, Word / Excel / PowerPoint, audio et vidéo.

- 🔍 **Détection automatique** : on dépose un fichier, l'app suggère les bonnes actions
- 🔄 **Conversions** : images ↔ PDF, Office → PDF, PDF → Word / TXT / PNG, PNG / JPG / WebP entre eux, audio, extraction audio depuis vidéo
- 🗜️ **Compression** PDF (léger / moyen / fort), images et audio
- ✏️ **Édition PDF** : annotation, surlignage, dessin, signature, fusion, découpage, réorganisation des pages
- 🎙️ **Audio** : découpe, fusion, et enregistrement du son système
- 🖱️ Intégration au **menu contextuel Windows** pour convertir une image en un clic

`Tauri v2` · `Rust` · `React` · `TypeScript` · `pdf-lib` · `PDF.js` · `docx` · crate `image` · `FFmpeg` · `LibreOffice`

---

## 🖥️ Applications desktop

### 🎮 Warzone Audio Enhancer
Application de bureau qui applique un **égaliseur paramétrique** au son système pour mieux localiser les pas ennemis dans Call of Duty: Warzone : profils sonores + compresseur (Equalizer APO / VST), **overlay radar** transparent visualisant la direction des sons, capture audio loopback native, installeur packagé.

`Electron` · `Node.js` · `Equalizer APO` · `VST`

### 🎧 AudioConvert Desktop
Application de bureau pour télécharger et convertir des liens **YouTube / Bandcamp** en audio (MP3/WAV) ou vidéo (MP4) : aperçu automatique, playlists, choix de la qualité, découpage, envoi vers Spotify.

`Python` · `customtkinter` · `yt-dlp` · `FFmpeg` · packagé en `.exe` (PyInstaller)

### 🕹️ Manette Dashboard
Tableau de bord **temps réel** affichant toutes les entrées d'une manette Xbox (sticks, gâchettes, boutons, batterie), avec métriques dérivées prévues (stick drift, temps d'appui, heatmap).

`Rust` · `egui / eframe` · `XInput (Windows)`

---

## 🌐 Web & full-stack

### ♠️ Card Games Online
Plateforme pour **jouer à la belote en ligne** : comptes utilisateurs, parties en temps réel via WebSockets (serveur autoritaire / anti-triche), classements et historique. Architecture back-end complète en monorepo.

`Next.js` · `React` · `NestJS` · `TypeScript` · `Socket.io` · `PostgreSQL / Prisma` · `Redis` · `Docker`

### 🎲 Game Hub — Duels 1v1 temps réel
Plateforme légère hébergeant **trois mini-jeux en duel** (quiz de culture générale, Snake, taquin), jouables en solo, en salon privé (code partagé) ou contre un adversaire aléatoire.

`Node.js` (temps réel via Server-Sent Events) · `JavaScript` · données `JSON`

### 🎨 Watch Render
Service web local transformant le **plan 3D d'une montre en photo studio photoréaliste** : import CAO/mesh, choix des matériaux par pièce dans un aperçu rapide, rendu final en arrière-plan.

`Python` · `Flask` · `Blender` (rendu) · `FreeCAD` (conversion CAO)

---

## 🔧 Outils & scripts

| Projet | Description | Stack |
|--------|-------------|-------|
| **Disk Comparator** | Outil web local comparant les fichiers d'un PC avec un disque de sauvegarde (avancement en direct) | `Node.js` · `PowerShell` |
| **Legion TD Archiver** | Script d'arrière-plan sauvegardant automatiquement chaque replay Warcraft III | `Python` · `psutil` |
| **DOCX Translation** | Traduction d'un document Word en préservant intégralement la mise en page (manipulation OOXML) | `Python` · `lxml` |

---

*Chaque projet part d'un besoin réel. N'hésitez pas à me contacter pour une démo ou pour discuter du code.*

---

📫 **Me contacter :** [LinkedIn — Théo Marme](https://www.linkedin.com/in/theo-marme-4b547912a)
