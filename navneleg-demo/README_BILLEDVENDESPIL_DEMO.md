# Plan demo · Billedvendespil

Denne pakke viser den rigtige arbejdsgang for navneleg og andre billedvendespil:

1. Plan henter et datasæt ind i sessionens dataliste.
2. Plan henter billederne ind i mediearkivet og viser dem som en billedmatrix.
3. Billedmatrixen kobles til datasættet.
4. Du kan åbne/rette datasættet.
5. Du trykker **Forvandl til billedvendespil** på billedmatrixen.
6. Den samme matrix bliver til et spil med **Tavlematrix** og **En ad gangen**.

## GitHub-mappestruktur

Læg filerne sådan her i din GitHub Pages-mappe:

```text
/
├─ index.html
└─ navneleg-demo/
   ├─ demo-index.json
   ├─ students/
   │  ├─ elevstamdata_navneleg_demo.csv
   │  ├─ elevstamdata_navneleg_demo.xlsx
   │  └─ photos/
   ├─ fruit-vegetables/
   │  ├─ frugt_groent_flersproget_demo.csv
   │  ├─ frugt_groent_flersproget_demo.xlsx
   │  └─ photos/
   ├─ periodic-table/
   │  ├─ periodisk_tabel_demo.csv
   │  ├─ periodisk_tabel_demo.xlsx
   │  └─ photos/
   └─ planets/
      ├─ planeter_demo.csv
      ├─ planeter_demo.xlsx
      └─ photos/
```

`index.html` skal ligge i samme mappe som `navneleg-demo/`. Ellers kan appen ikke finde `navneleg-demo/demo-index.json` og demoernes billeder.

## Sådan tester du

1. Pak ZIP-filen ud.
2. Læg indholdet i en GitHub Pages-mappe.
3. Åbn `index.html` via GitHub Pages.
4. Tryk **Billedspil** i Plan-værktøjslinjen.
5. Vælg en demo:
   - **Navneleg · opdigtede elever**
   - **Frugt og grønt · sprog**
   - **Periodisk tabel · de første 25**
   - **Planeter og rumobjekter**
6. Plan opretter først en billedmatrix og et datasæt i sessionen.
7. Tryk **Forvandl til billedvendespil** nederst på billedmatrixen.

## Egne billeder

Vælg **Importer egne billeder** i Billedspil-modalens nederste kort.

Plan gør så dette:

1. Importerer billedstakken til mediearkivet.
2. Opretter et datasæt ud fra filnavnene.
3. Opretter en billedmatrix.
4. Lader dig rette bagsideteksterne.
5. Lader dig forvandle matrixen til billedvendespil.

Den generiske model er:

```text
billeder → billedmatrix
filnavne → datasæt
billedmatrix + datasæt → billedvendespil
```

## Bemærkninger

Billederne er syntetiske demo-illustrationer og indeholder ingen rigtige elever eller persondata.

Ved lokal åbning direkte fra filsystemet kan browserens sikkerhed blokere `fetch()` af demo-filer. Brug GitHub Pages eller en lille lokal webserver.


## Opdateret arbejdsgang

Billedvendespil findes nu i **Tilføj indhold** og i en **Billedmatrix' •••-menu**. Den faste værktøjslinje bruges ikke. Datasættet har en `Forside`-kolonne, så læreren præcist kan styre, hvad der må stå på forsiden. I præsentation og maksimeret visning skjules kontrolpaneler, så matrixen står roligt på tavlen.
