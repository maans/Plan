# Plan · bibliotek med årsforløb

Plan-biblioteket samler færdige årsplaner, undervisningsforløb og skabeloner, som kan åbnes direkte fra **Hent demoforløb** i Plan.

Et forløb i biblioteket er en udgivelseskopi. Når en lærer vælger **Brug som lokal kopi**, opretter Plan et nyt, selvstændigt undervisningsforløb i browserens lokale lager. Lærerens ændringer bliver i den lokale kopi og ændrer ikke filen på GitHub.

---

## Sådan bruges biblioteket

Mappen `plan-library` skal ligge ved siden af Plans `index.html`:

```text
Plan/
├── index.html
├── plan.webmanifest
├── plan-assets/
└── plan-library/
    ├── catalog.json
    ├── README.md
    ├── dansk/
    ├── engelsk/
    ├── matematik/
    ├── science/
    ├── tysk/
    ├── andre-9/
    └── andre/
```

Plan leder som standard efter:

```text
./plan-library/catalog.json
```

Når filerne er lagt på GitHub Pages, åbnes biblioteket i Plan via:

**Åbn Plan → Hent demoforløb**

eller senere via:

**Forløbsnavnet øverst → Alle undervisningsforløb → Hent demoforløb**

---

## Hvad er et årsforløb i Plan?

Et undervisningsforløb består af tre niveauer:

1. **Undervisningsforløb** – for eksempel Dansk 2025–26
2. **Sessioner** – for eksempel Familien eller Frihed og flugt
3. **Tavler** – de konkrete arbejdsflader i hver session

Årsforløbspakken samler sessionernes rækkefølge, tavler, widgets, data, fælles kalender og de medier, der følger med.

Plan importerer ikke et demoforløb ind i det forløb, som allerede er åbent. Det bliver oprettet som et nyt forløb med sin egen identitet.

---

## Forløb i denne pakke

### Dansk 9.–10. klasse · årsplan 2025–26

- 6 sessioner
- 92 tavler
- 366 widgets
- fælles kalender
- tomme PDF-widgets til materialer, som brugeren selv skal hente
- faktabokse, arbejdsplaner og KaPardy-aktiviteter

Fil:

```text
dansk/dansk-2025-26/forloeb.json
```

### Fællessamlinger · årsforløb 2026–27

- 31 sessioner i kronologisk rækkefølge
- 428 tavler
- 1.189 widgets
- 192 datasæt
- 126 medier

Fil:

```text
andre/faellessamlinger-2026-27/forloeb.json
```

---

## Faggrupper

Plan viser disse overordnede valg:

- **Dansk**
- **Engelsk**
- **Matematik**
- **Science**
- **Tysk**
- **Andre 9.-klassefag**
- **Andre**

**Science** kan rumme naturfag, fysik/kemi, biologi og geografi.

**Andre 9.-klassefag** kan blandt andet rumme historie, samfundsfag, idræt/gymnastik, kristendom, musik og praktiske/kreative fag.

**Andre** bruges til tværfaglige forløb, skoleliv, fællessamlinger, kontaktgrupper og øvrige forløb.

Klassetrin, skoleår og emner lægges desuden i forløbets metadata, så Plan kan filtrere og søge.

---

## Tilføj et nyt årsforløb

### 1. Pak forløbet i Plan

Åbn **Datacenter → Årsforløb**, vælg de sessioner, der skal med, og brug **Pak / offload årsforløb**.

Den udgivne fil skal være en rigtig Plan-årsforløbspakke med formatet:

```text
tavle-next-course-package
```

### 2. Opret en mappe

Eksempel:

```text
plan-library/historie/historie-9-2026-27/
```

I den nuværende fagopdeling placeres historie under:

```text
plan-library/andre-9/historie/historie-9-2026-27/
```

### 3. Brug faste filnavne

```text
forloeb.json
README.md
kalender.ics      valgfri
forside.webp      valgfri
```

### 4. Tilføj forløbet i `catalog.json`

Eksempel:

```json
{
  "id": "historie-9-2026-27",
  "kind": "demo",
  "status": "published",
  "title": "Historie 9. klasse · årsplan 2026–27",
  "category": "andre-9",
  "subject": "Historie",
  "description": "Et helt skoleårs historieundervisning.",
  "schoolYear": "2026–27",
  "gradeLevels": ["9"],
  "tags": ["årsplan", "historie", "kilder"],
  "version": "1.0.0",
  "packageUrl": "./andre-9/historie/historie-9-2026-27/forloeb.json",
  "featured": false
}
```

---

## Demo eller skabelon?

Brug:

```json
"kind": "demo"
```

når forløbet indeholder et konkret eksempel med tavler, tekster, aktiviteter og eventuelt data.

Brug:

```json
"kind": "template"
```

når læreren selv skal fylde hovedparten af indholdet ud.

---

## Materialer og ophavsret

Biblioteket bør kun indeholde materialer, der må deles.

Når en tekst, bogside, artikel eller anden fil ikke kan følge med, kan årsforløbet i stedet have:

- en tom PDF-widget med en tydelig titel
- et link til materialets lovlige placering
- en note om, hvad læreren selv skal hente
- en faktaboks eller arbejdsvejledning, der kan bruges uden originalfilen

På den måde kan forløbets struktur og didaktiske plan deles, uden at beskyttede materialer kopieres ind i pakken.

---

## Kalender

En fælles kalender kan ligge som et fælles kalenderdatasæt inde i `forloeb.json`.

En ekstra `kalender.ics` kan vedlægges, når kalenderen også skal kunne åbnes i andre kalenderprogrammer. ICS-filen skal ikke importeres særskilt i Plan, hvis de samme aktiviteter allerede findes i årsforløbspakken.

---

## Gem, opdater og genudgiv

Et forløb i biblioteket er en udgivelseskopi. Brugeren arbejder altid videre i sin lokale kopi.

Når et bibliotekseksemplar opdateres:

1. behold samme `id`, hvis det er en ny version af samme forløb
2. hæv feltet `version`
3. opdater `updatedAt`
4. erstat `forloeb.json`
5. undgå automatisk at overskrive lærerens lokale kopi

En ny biblioteksversion bør kunne hentes som et nyt forløb eller senere sammenlignes med brugerens kopi.

---

## Sikkerhed og backup

Plan gemmer lærerens arbejdskopi lokalt i browseren. Biblioteket er ikke en backup af de ændringer, læreren laver efter import.

Brug derfor Plans årsforløbspakke eller nødbackup til at gemme en opdateret kopi i Filer, på skolens drev eller et andet sikkert sted.

---

## Filoversigt

- `catalog.json` – bibliotekets register
- `README.md` – denne vejledning
- fagmapperne – bibliotekets overordnede valgmuligheder
- `forloeb.json` – den konkrete årsforløbspakke
- `kalender.ics` – valgfri kalenderkopi
- `forside.webp` – valgfrit billede til bibliotekskortet

---

## Kort fortalt

Plan-biblioteket gør det muligt at:

- finde årsplaner efter fag
- se klassetrin, skoleår og emner før import
- hente et forløb som en selvstændig lokal kopi
- bevare sessionernes kronologiske rækkefølge
- genbruge tavler, widgets, data og kalender
- udgive nye eller opdaterede årsforløb uden at overskrive lærerens arbejde
