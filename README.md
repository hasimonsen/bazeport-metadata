# BazePort Metadata Addons

**BazePort Metadata Addons** er et samleprosjekt som inneholder to uavhengige Chrome-utvidelser for **BazePort Management Studio**.  
Utvidelsene integrerer med [The Movie Database (TMDb)](https://www.themoviedb.org/) og gjør det mulig å hente og fylle ut metadata for både filmer og TV-serier raskt, presist og konsistent.

- 🎬 **Movies Addon** → [hasimonsen/bazeport-movies-metadata](https://github.com/hasimonsen/bazeport-movies-metadata)  
- 📺 **TV Series Addon** → [hasimonsen/bazeport-tv-series-metadata](https://github.com/hasimonsen/bazeport-tv-series-metadata)  

Begge prosjektene er utviklet separat for å reflektere forskjellene mellom film- og seriehåndtering i BazePort, men er samlet i dette hovedrepoet via **Git submodules** for enhetlig struktur og enkel distribusjon.

---

## 🌟 Nøkkelfunksjoner
- Automatisk parsing av filnavn (inkludert sesong- og episodenummer for serier).  
- Integrasjon mot **TMDb API** for uthenting av:
  - Offisielle titler
  - Produksjonsår
  - Beskrivelser (overview)
  - Plakater og bakgrunnsbilder  
- Direkte utfylling i BazePort Management Studio sine skjemaer.  
- Mulighet for både automatisert utfylling og manuell overstyring.  
- Betydelig tidsbesparelse og redusert risiko for feil i metadataregistrering.

---

## 📂 Repository-struktur
```

bazeport-metadata/
├── movies/   -> [https://github.com/hasimonsen/bazeport-movies-metadata](https://github.com/hasimonsen/bazeport-movies-metadata)
└── tv/       -> [https://github.com/hasimonsen/bazeport-tv-series-metadata](https://github.com/hasimonsen/bazeport-tv-series-metadata)

````

- `movies/` → Chrome-utvidelsen for filmer  
- `tv/` → Chrome-utvidelsen for TV-serier  
- Begge oppdateres uavhengig, men distribueres samlet her.

---

## 🚀 Kom i gang

### Klon hele prosjektet (inkludert submodules)
```bash
git clone --recurse-submodules https://github.com/hasimonsen/bazeport-metadata.git
````

### Oppdater submodules til siste versjon

```bash
git submodule update --remote --merge
```

---

## 🔧 Installasjon i Chrome

Hver utvidelse kan installeres separat i Chrome:

1. Last ned repoet (eller bare ønsket submodule).
2. Åpne Chrome og naviger til `chrome://extensions/`.
3. Aktiver **Developer Mode** (øverst til høyre).
4. Klikk **Load unpacked** og velg mappen (`movies/` eller `tv/`).
5. Utvidelsen er nå tilgjengelig i nettleseren.

---

## 💡 Bruksscenario

* Når en film eller serieepisode lastes opp i **BazePort Management Studio**, vises en verktøylinje fra addon.
* Addon foreslår metadata basert på filnavn, eller lar brukeren søke manuelt.
* Informasjon hentes fra TMDb og fylles inn automatisk:

  * For filmer: tittel, årstall, beskrivelse, plakat.
  * For serier: tittel, sesong, episode, beskrivelse, plakat.
* Resultatet er en raskere, enklere og mer pålitelig arbeidsflyt.

---

## 🎯 Hvorfor to addons?

* **Filmer** krever kun enkel metadata (tittel, årstall, beskrivelse).
* **TV-serier** krever mer kompleks logikk (sesong- og episodenummer, episodebeskrivelser).

Derfor er prosjektene bygget som to separate utvidelser, men de samles her for å gi et helhetlig rammeverk.

---

## 🗺 Roadmap

* [ ] Flerspråklig metadata-støtte basert på TMDb-oversettelser.
* [ ] Bedre fallback-mekanismer når TMDb ikke returnerer resultater.
* [ ] Automatisk valg av best passende plakat/bakgrunnsbilde.
* [ ] Forbedret logging, feilhåndtering og brukerfeedback.

---

## 🤝 Bidrag

Bidrag ønskes!

* Opprett en *issue* eller *pull request* i dette repoet for generelle forbedringer.
* For addon-spesifikke saker:

  * 🎬 [Movies Repo](https://github.com/hasimonsen/bazeport-movies-metadata)
  * 📺 [TV Series Repo](https://github.com/hasimonsen/bazeport-tv-series-metadata)

---

## 📜 Lisens

Distribuert under [MIT License](LICENSE).
