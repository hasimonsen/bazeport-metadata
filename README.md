# BazePort Metadata Addons

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Chrome](https://img.shields.io/badge/Chrome-Extension-green)](https://chrome.google.com/webstore/)

**BazePort Metadata Addons** is a parent project that hosts two independent Chrome extensions for **BazePort Management Studio**.  
These addons integrate with [The Movie Database (TMDb)](https://www.themoviedb.org/) to automatically retrieve and populate metadata for both **movies** and **TV series**, ensuring speed, consistency, and accuracy in content registration.

---

## ✨ Key Features

- 🔎 **Automatic filename parsing** (season & episode detection for series).  
- 🎬 **TMDb API integration** for:
  - Official titles  
  - Release year  
  - Descriptions (overview)  
  - Posters & backdrops  
- ⚡ **Direct autofill** into BazePort Management Studio forms.  
- 🛠 **Manual override support** where automation isn’t enough.  
- 📉 **Reduced errors & significant time savings** in metadata entry.  

---

## 📂 Repository Structure

```text
bazeport-metadata/

````

Each extension is versioned independently but distributed together here.

---

## 🚀 Getting Started

Clone the project including its submodules:

```bash
git clone --recurse-submodules https://github.com/hasimonsen/bazeport-metadata.git
```

Update submodules to the latest versions:

```bash
git submodule update --remote --merge
```

---

## 🔧 Installation in Chrome

Each extension can be installed separately:

1. Download this repo (or only the desired submodule).
2. Open Chrome and go to `chrome://extensions/`.
3. Enable **Developer Mode**.
4. Click **Load unpacked** and select either `movies/` or `tv/`.
5. The extension will appear in Chrome.

---

## 💡 Usage

When uploading a movie or TV episode in **BazePort Management Studio**, the addon toolbar becomes available:

* Parses filenames automatically for suggested metadata.
* Fetches additional details from TMDb.
* Autofills fields such as title, year, description, poster.

**Examples:**

* **Movies:** title, year, description, poster.
* **TV Series:** show title, season, episode, description, poster.

The result: **faster workflows, less manual typing, fewer errors.**

---

## 🔖 Versioning & Releases

* Both addons follow **semantic versioning** (`MAJOR.MINOR.PATCH`).

* Releases are bundled under this parent repo for easier distribution and testing.

* Chrome Web Store submissions use the version defined in each submodule’s `manifest.json`.

* Parent repo versions (tags) may reflect combined milestone releases, e.g. **BazePort Metadata Addons 2.1.4*

---

## 🗺 Roadmap

* 🌍 Multilingual metadata support via TMDb translations.
* 🛡 Improved fallback when TMDb has no results.
* 🖼 Smarter poster/backdrop selection.
* 📊 Enhanced logging, error handling, and user feedback.

---

## ⚠️ Disclaimer

This project is an **independent open-source initiative**.
It has **no official connection, affiliation, or endorsement** from:

* **BazePort (Baze Technology AS)**
* **The Movie Database (TMDb)**

The software only provides tools to assist with metadata handling.
You are solely responsible for ensuring compliance with all relevant terms, conditions, and API usage policies.

---

## 📜 License

Distributed under the [MIT License](LICENSE).
© 2025 – BazePort Metadata Addons
