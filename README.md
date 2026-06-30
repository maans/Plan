# Plan

![Plan](plan-assets/plan-icon.svg)

**Plan er lærerens lokale arbejds- og præsentationsmiljø til hele undervisningsforløb.**

Her kan du samle årsplaner, sessioner, tavler, oplæg, PDF’er, billeder, video, lyd, lister, elevoplysninger, grupper, aktiviteter, kalender og noter i ét sammenhængende forløb.

Plan bruges direkte i browseren. Appen kræver hverken login, elevkonti eller en central server. Arbejdet gemmes lokalt på enheden, og læreren bestemmer selv, hvad der vises, deles og gemmes.

Plan bygger videre på den fleksible tavleform fra Tavle, men sætter **undervisningsforløbet** i centrum: fra årsplan og sessioner til konkrete tavler, widgets, data og medier.

---

## Åbn Plan

### Brug Plan online

Åbn Plan direkte i browseren:

https://plan.måns.dk/

### Brug Plan lokalt

Plan kan også bruges som en lokal browserapp:

1. Hent Plan-pakken fra GitHub.
2. Pak filerne ud.
3. Åbn `index.html` i en moderne browser.

Pakken skal som minimum bevare `index.html`, `plan-assets`, `plan.webmanifest`, biblioteket med demoforløb og de øvrige mapper, som følger med appen.

På iPad kan Plan føjes til hjemmeskærmen og bruges som en selvstændig browserapp.

---

## Sådan er Plan bygget op

Plan organiserer undervisningen i fire niveauer:

1. **Undervisningsforløb** – for eksempel *Dansk 2026–27*
2. **Sessioner** – for eksempel *Familien*, *Frihed og flugt* eller *Mundtlig prøve*
3. **Tavler** – de konkrete arbejdsflader i en session
4. **Widgets** – tekst, billeder, PDF, data, aktiviteter og andet indhold på tavlen

Et undervisningsforløb kan derfor rumme både den langsigtede plan, rækkefølgen mellem sessionerne og det materiale, der skal bruges i den enkelte undervisningstime.

Når Plan åbner, kan du fortsætte det senest brugte forløb, gå til næste session, vælge en anden session eller åbne oversigten over alle undervisningsforløb.

---

## Planlæg et helt undervisningsforløb

Et forløb kan blandt andet indeholde:

- årsplan og fælles kalender
- sessioner i kronologisk rækkefølge
- starttavler og dagsprogrammer
- lærerens oplæg og instruktioner
- opgaver, links og PDF-materialer
- billeder, video og lyd
- elev-, gruppe- og tavleoverblik
- aktiviteter og repetition
- opsamling, evaluering og noter
- reserveindhold og alternative veje

Tavlerne kan bruges som sider i et forløb, men de er samtidig frie arbejdsflader. Widgets kan flyttes, ændres i størrelse, roteres, låses, skjules, minimeres og maksimeres.

Plan kan derfor tilpasses, mens undervisningen er i gang, uden at læreren er bundet til en fast præsentation.

---

## Gennemfør undervisningen fra samme sted

Når indholdet er klar, kan Plan skifte mellem forskellige arbejdsformer:

- **Redigering** bruges til at opbygge og ændre tavlen.
- **Præsentation** skjuler redigeringsgrejet og giver en roligere fælles visning.
- **Fokus** fremhæver én widget ad gangen.
- **Maksimering** lader én widget fylde arbejdsfladen.
- **Tavleskift** fører gennem sessionens tavler.
- **Widgetvælgeren** gør det hurtigt at finde og fokusere et bestemt element.

Plan kan derfor bruges til både forberedelse, fælles gennemgang, aktivitet, individuel samtale og evaluering.

---

## Få materialer hurtigt ind

Du kan vælge eller trække én eller mange filer ind i Plan. Appen forsøger selv at vælge en passende widgettype.

Det kan blandt andet være:

- billeder
- video
- lyd
- PDF-filer
- regneark og CSV-filer
- tekstfiler
- kalenderfiler
- HTML-apps
- backup- og forløbspakker

### Billeder, video og lyd

En enkelt mediefil åbnes som en almindelig widget.

Når flere filer af samme type importeres samlet, kan Plan samle dem i en matrix:

- **Billedmatrix**
- **Videomatrix**
- **Lydmatrix**

Medier kan afspilles eller vises direkte i matrixen. Et enkelt medie kan desuden åbnes i en stor visning, hvor du kan bladre med knapper, piletaster eller swipe.

Plan indlæser kun de medier, der er nødvendige for den aktuelle side, så store samlinger belaster appen mindst muligt.

I **Datacenter → Medier** kan enkelte filer hentes igen. Medier fra andre undervisningsforløb er beskyttet mod utilsigtet sletning.

### PDF

PDF-filer åbnes som PDF-widgets med sidevisning, formularfelter, links, scrolling og kantbladring.

PDF kan bruges til:

- opgaveark og prøveoplæg
- formularer
- elevbesvarelser
- afstemning og dataindsamling
- fælles gennemgang
- materialer, der skal bevare deres oprindelige layout

### HTML-apps

Plan kan indlejre selvstændige HTML-apps som blandt andet:

- Plan
- Tavle
- Skriv
- Tjek
- TiddlyWiki
- andre lokale eller webbaserede HTML-apps

HTML-apps kan bruges som aktive værktøjer inde i en tavle og kan minimeres og gendannes uden at miste deres aktuelle tilstand.

---

## Arbejd med lister, data og Datacenter

Plan kan bruge regneark, CSV-filer, lister og fælles data som grundlag for mange forskellige arbejdsgange.

Du kan blandt andet:

- vise et datasæt som DataWidget
- oprette lister ud fra data
- genbruge samme kilde i flere widgets
- filtrere, sortere og sammensætte data med DataRemix
- bruge navnelister i Grupper og Lykkehjulet
- oprette elevkort og elevkortmatricer
- danne grupper og gruppetavler
- oprette tavler fra en liste
- samle tavler som TavleKort
- koble kalenderdata og ICS-filer
- se forbindelser mellem objekter, visninger og datakilder

**Datacenter** samler arbejdet i faner for blandt andet:

- Sessioner
- Sessionsdata
- Fælles data
- Datakilder
- DataRemix
- Relationer
- Medier
- Gendannelse
- Lager

Datacenter åbner med `D`. Piletasterne bruges til faner og scrolling, `Enter` vælger, og `Esc` går tilbage eller lukker.

Plan viser som udgangspunkt kun data og medier fra den aktuelle session eller det aktuelle undervisningsforløb. Delte eller fremmede filer beskyttes mod utilsigtet sletning.

---

## Elevkort, grupper og levende overblik

Plan kan bygge videre på elev- og gruppedata uden at kræve et særskilt elevsystem.

### Elevkort

Fra et egnet elevstamdatasæt kan du oprette:

- enkelte Elevkort
- en Elevkortmatrix
- elevtavler
- elevnoter
- noteoversigter

Elevkort kan vise elevens egne oplysninger samt fanerne **Elev**, **Mor**, **Far** og **Notater**. Tekniske identifikatorer bruges internt, men vises ikke i den almindelige brugerflade.

### Grupper

GruppeWidget kan:

- hente deltagere fra en liste eller et datasæt
- danne grupper
- låse bestemte deltagere eller roller
- oprette tomme grupper
- dele en eksisterende gruppe
- oprette gruppetavler
- vise grupperne som matrix eller i Gruppegalaksen

GruppeWidgetten er hovedkilden. Når medlemmer, roller eller gruppenavne ændres, kan de tilknyttede Gruppekort og gruppetavler følge med.

### TavleKort og matricer

Plan kan samle mange relaterede elementer i oversigter:

- Elevkortmatrix
- Gruppekortmatrix
- TavleKortmatrix
- Billed-, video- og lydmatricer
- Gruppegalaksen

Kortene er kompakte i oversigten og kan åbnes i en større detaljevisning med tastatur- og swipe-navigation.

---

## Brug aktiviteter i undervisningen

Plan rummer flere aktiviteter, som kan bruges direkte på tavlen:

- **KaPardy** til quiz, repetition og holdkonkurrence
- **Grupper** til gruppedannelse og gruppearbejde
- **Lykkehjulet** til tilfældige eller lærerbestemte valg
- **Afstemning** til fælles respons og anonym PDF-baseret indsamling
- **Ordsky** til idéer, begreber og opsamling
- **Timer og stopur** til arbejdsperioder, sekvenser og mellemtider
- **Kalender** til dagsprogram, ugeplan og årsplan

Aktiviteterne kan bruge data og lister, som allerede findes i forløbet, så de samme oplysninger ikke skal skrives ind flere gange.

KaPardy bevarer kompatibilitet med ældre spilbanker, hvor første svar efter spørgsmålet er korrekt, og de tre næste er forkerte. Svarene blandes ved spilstart.

---

## Kalender, årsplan og bibliotek

Kalenderen kan bruges til:

- dagsprogram
- ugeskema
- månedsoverblik
- skoleår og forløbsplan
- rejser og projektuger
- arrangementer og særlige skoledage

Kalenderdata kan oprettes direkte, hentes fra et datasæt eller importeres fra en `.ics`-fil.

Plan har desuden et bibliotek med færdige undervisningsforløb og skabeloner.

Åbn biblioteket via:

**Plan-ikonet eller forløbsnavnet → Alle undervisningsforløb → Hent demoforløb**

Et bibliotekseksemplar importeres som en selvstændig lokal kopi. Lærerens ændringer påvirker ikke filen i biblioteket.

Bibliotekets tekniske opbygning og vejledning til udgivelse af nye forløb findes i:

```text
plan-library/README.md
```

---

## Gem, genbrug og flyt indhold

Plan gemmer arbejdet lokalt i browseren.

Du kan blandt andet bruge:

- **Backup** til den aktuelle session
- **Backup+** når tilknyttede data og medier skal med
- **Backup++** til flere sessioner
- **Årsforløbspakker** til et helt undervisningsforløb
- **Sessionpakker** til at sende udvalgte tavler til en anden session
- **Papirkurv** til slettede widgets
- **Gendannelsespunkter** til tidligere tilstande
- **Tavleshots** til øjebliksbilleder af tavler
- **Lagerredning** ved gemme- eller pladsmangel

Plan kontrollerer lagringen før skift mellem større undervisningsforløb. Hvis browseren ikke kan gemme, bliver det aktuelle forløb stående åbent, og Lagerredning tilbyder nødbackup, oprydning og nyt gemmeforsøg.

Der findes to slags brugere: dem, der tager backup før oprydning – og dem, der bagefter ville ønske, de havde gjort det.

---

## Lærerens lokale arbejdsrum

Plan er først og fremmest lærerens eget undervisningsmiljø.

Det betyder:

- ingen login
- ingen elevkonti
- ingen central database
- ingen indbygget aflevering eller beskedsystem
- indhold, data og medier gemmes lokalt i browseren
- læreren bestemmer, hvad der vises, deles og gemmes

Materialer kan udleveres eller modtages gennem skolens eksisterende tjenester.

Plan er ikke afhængig af, at eleverne bruger Plan på deres egne enheder.

---

## Kompatibilitet med Tavle

Plan er et nyt produktnavn og en ny, mere sammenhængende forløbsmodel, men arbejdsfladerne hedder fortsat **tavler**.

Plan bevarer så vidt muligt kompatibilitet med indhold fra den klassiske Tavle, herunder:

- tavler og widgets
- sessioner
- data og medier
- PDF
- KaPardy-spil og spilbanker
- Backup- og importformater

Ved import kan Plan omforme ældre indhold til den nye model uden unødige navne- eller formatbrud.

---

## Hjælp i appen

Den indbyggede **Hjælp** er den praktiske vejledning til Plan.

Her finder du blandt andet hjælp til:

- undervisningsforløb, sessioner og tavler
- widgets og filimport
- billeder, video, lyd og mediematricer
- PDF og data
- elev-, gruppe- og tavlekort
- Gruppegalaksen
- aktiviteter
- Datacenter
- backup, Lagerredning og gendannelse
- tastatur, touch og præsentation

Hjælpen kan betjenes med tastaturet:

- `←` og `→` skifter hjælpeafsnit
- `↑` og `↓` scroller
- `Enter` åbner eller vælger
- `B` skifter tema
- `Esc` lukker eller går tilbage

README-filen er den korte introduktion. Hjælp i appen er vejledningen, mens du arbejder.

---

## Browserapp og iPad

Plan indeholder webapp-manifest og appikoner, så den kan bruges som browserapp og føjes til hjemmeskærmen på iPad og andre understøttede enheder.

Plan er udviklet med fokus på:

- touch og mus
- tastatur og SmartBoard
- lokal lagring
- store undervisningsforløb
- kontrolleret indlæsning af data og medier
- arbejde uden krav om login

---

## Filoversigt

Pakken indeholder blandt andet:

- `index.html` – selve Plan
- `README.md` – denne introduktion
- `plan.webmanifest` – webapp-manifest
- `plan-assets/` – logo, ikoner og øvrige appfiler
- `plan-library/` – bibliotek med undervisningsforløb
- `plan-library/catalog.json` – bibliotekets register
- `plan-library/README.md` – vejledning til biblioteket

---

## Kort fortalt

**Plan – tavler til overblik og læring** samler lærerens:

- årsplaner og undervisningsforløb
- sessioner og tavler
- materialer og PDF’er
- billeder, video og lyd
- lister, data og relationer
- elev- og gruppeoverblik
- aktiviteter
- kalender
- præsentation
- backup, gendannelse og genbrug

i én lokal browserapp, der kan tilpasses undervisningen, mens den foregår.
