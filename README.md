Supert 🙌 Da lager vi et oppdatert **README-utkast for hovedrepoet** der `movies/` og `tv/` ikke bare peker til mapper, men direkte til GitHub-repoene dine. Dette gjør dokumentasjonen mye mer nyttig og profesjonell.

---

# 📑 Oppdatert README.md (hovedrepo)

```markdown
# BazePort Metadata Addons

Dette er et **samle-repo** for to uavhengige Chrome-utvidelser som automatiserer metadata-innhenting i **BazePort Management Studio**.  
Begge utvidelsene benytter [The Movie Database (TMDb)](https://www.themoviedb.org/) som kilde, og gjør det enklere å legge til riktige titler, årstall, beskrivelser og bilder når filmer og serier skal lastes opp i BazePort.

- 🎬 **Movies Addon** → [hasimonsen/bazeport-movies-metadata](https://github.com/hasimonsen/bazeport-movies-metadata)  
- 📺 **TV Addon** → [hasimonsen/bazeport-tv-series-metadata](https://github.com/hasimonsen/bazeport-tv-series-metadata)  

Disse prosjektene er bygget som to separate addons, men samles her via **Git submodules** for enklere administrasjon.

---

## ✨ Funksjoner
- Automatisk parsing av filnavn (tittel, sesong, episode, årstall).  
- Integrasjon mot **TMDb API** for å hente:
  - Offisiell tittel
  - Årstall
  - Beskrivelse/overview
  - Bildeplakater og bakgrunnsbilder (poster/backdrop)
- Utfylling direkte i **BazePort Management Studio** sine skjemaer.  
- Valgfrihet mellom manuell søk, forslag eller automatisk utfylling.  
- Raskere og mer nøyaktig metadata-registrering sammenlignet med manuell oppslag.

---

## 📂 Repo-struktur
```

bazeport-metadata/
├── movies/   -> peker til [https://github.com/hasimonsen/bazeport-movies-metadata](https://github.com/hasimonsen/bazeport-movies-metadata)
└── tv/       -> peker til [https://github.com/hasimonsen/bazeport-tv-series-metadata](https://github.com/hasimonsen/bazeport-tv-series-metadata)

````

---

## 🚀 Kom i gang

### 1. Klone hele prosjektet (med submodules)
```bash
git clone --recurse-submodules https://github.com/hasimonsen/bazeport-metadata.git
````

### 2. Oppdatere submodules

Hvis Movies eller TV får nye commits:

```bash
git submodule update --remote --merge
```

---

## 🔧 Installasjon i Chrome

Hver addon kan lastes inn separat i Chrome:

1. Last ned repoet eller kun ønsket addon (`movies/` eller `tv/`).
2. Åpne **Chrome** → skriv `chrome://extensions/` i adressefeltet.
3. Slå på **Developer mode** (øverst til høyre).
4. Klikk **Load unpacked** og velg enten `movies/`- eller `tv/`-mappen.
5. Addon blir nå tilgjengelig i nettleseren.

---

## 🛠️ Typisk bruk

* Last opp en film eller tv-serie i **BazePort Management Studio**.
* Addon viser en liten verktøylinje.
* Den foreslår metadata hentet fra TMDb basert på filnavn.
* Du kan godkjenne eller endre søket manuelt.
* Felt som tittel, år, beskrivelse og bilder fylles ut automatisk.
* Ferdig! 🚀

---

## 🎯 Hvorfor to addons?

Film- og seriehåndtering i BazePort er forskjellig:

* **Filmer** trenger kun tittel, år og beskrivelse.
* **TV-serier** krever sesong/episode-informasjon, og har mer kompleks parsing av filnavn.

Derfor er addonene bygget separat, men vedlikeholdes side om side.

---

## 📌 Roadmap

* [ ] Bedre støtte for flere språk (TMDb har oversettelser).
* [ ] Forbedret fallback når TMDb ikke finner match.
* [ ] Mulighet for automatisk bildevalg (poster/backdrop).
* [ ] Bedre logging og feilhåndtering.

---

## 🤝 Bidra

Pull requests og forslag er velkomne!

* For problemer eller funksjonsønsker relatert til filmer → bruk [Movies-repoet](https://github.com/hasimonsen/bazeport-movies-metadata).
* For problemer eller funksjonsønsker relatert til tv-serier → bruk [TV-repoet](https://github.com/hasimonsen/bazeport-tv-series-metadata).

---

## 📜 Lisens

Alle prosjektene distribueres under [MIT License](LICENSE).

```

---

✅ Dette README-et er klart til å kopieres inn i hovedrepoet ditt.  
Det peker **direkte til GitHub-repoene** for Movies og TV og beskriver prosjektet utfyllende.  

👉 Vil du at jeg også lager ferdige **README-filer for Movies- og TV-repoene**, som inneholder fokusert dokumentasjon og peker tilbake til hovedrepoet?
```
