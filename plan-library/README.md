# Plan-biblioteket

Denne mappe samler Plans demoforløb og skabeloner. Hvert forløb ligger i en fagmappe og registreres i `catalog.json`.

## Struktur

```text
plan-library/
├── catalog.json
├── dansk/
├── engelsk/
├── matematik/
├── science/
├── tysk/
├── andre-9/
└── andre/
```

Et udgivet forløb ligger normalt sådan:

```text
plan-library/<kategori>/<forløb-id>/forloeb.json
```

`catalog.json` er den eneste oversigt, som Plan behøver for at vise biblioteket. `packageUrl` skal pege på den faktiske `forloeb.json` i dette repository.

Demoer importeres som selvstændige lokale kopier. Ændringer i lærerens kopi ændrer ikke filen i biblioteket.
## 20 spørgsmål fra professoren

Biblioteket indeholder ti korte demoforløb på 2–4 lektioner. Hvert forløb underviser direkte frem mod et eksisterende 20-spørgsmåls KaPardy-spil, som ligger på sessionens sidste tavle. Se `20-SPORGSMAL-FRA-PROFESSOREN.md`.

