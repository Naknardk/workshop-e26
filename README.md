# Diversitetsbarometeret

Hvor mangfoldig er din arbejdsplads?

I dette miniprojekt bygger I et online barometer, hvor en arbejdsplads kan taste sine
egne tal ind og se, hvor den ligger i forhold til sammenlignelige arbejdspladser i
Danmark. Barometeret skal også fungere som et almindeligt opslagsværktøj for alle, der
vil vide, hvordan køn, alder og herkomst er fordelt på tværs af brancher, regioner og
størrelser.

Projektet bygger på rapporten *Mod diversitet på arbejdspladsen* (Qvist & Larsen).
Barometeret er ikke et selvstændigt produkt, men en måde at gøre rapportens
resultater brugbare for den enkelte arbejdsplads.

## Hvad barometeret skal kunne

**1. Sammenlign din arbejdsplads.** Brugeren angiver branche, antal ansatte, sektor og
region, og derefter arbejdspladsens andel af kvinder, seniorer og medarbejdere med
indvandrerbaggrund. Barometeret svarer med, hvor arbejdspladsen ligger i fordelingen
blandt de sammenlignelige — ikke blandt alle.

**2. Slå op.** Uden at taste noget ind skal man kunne se, hvordan de tre andele
fordeler sig i en given branche, region eller størrelsesgruppe.

## Definitioner

Barometeret bruger rapportens definitioner, så tallene kan sammenlignes:

| Begreb | Definition |
|---|---|
| Stilling | Et *novemberjob*: det job, en person har sidste arbejdsdag i november (Danmarks Statistik) |
| Senior | 55 år eller derover |
| Indvandrerbaggrund | Indvandrere og efterkommere efter Danmarks Statistiks definition |
| Branche | Danmarks Statistiks branchekode DB07 |
| Periode | 2012 til 2022 |

## Data

I får **ikke** oplysninger om de enkelte arbejdspladser. Rapporten bygger på
registerdata fra Danmarks Statistik, og den slags data må ikke forlade Danmarks
Statistiks forskningsmaskiner. Det, der kommer til at ligge i `data/`, er aggregerede
tal (fordelinger for grupper af arbejdspladser) der er gjort så grove, at ingen
enkelt arbejdsplads kan genkendes i dem.

Det er ikke en teknisk begrænsning, men en del af opgaven: et barometer, der kan
bruges til at identificere enkelte arbejdspladser, er et dårligt barometer.

## Teknik

- **Python** til al beregning
- **Quarto** til hjemmesiden: forside, barometer, opslag og rapportens hovedfund
- **GitHub Pages** til at publicere det hele

Barometeret kommer til at køre direkte i browseren. Det betyder, at de tal, en
arbejdsplads taster ind, aldrig bliver sendt nogen steder hen. De bliver på brugerens
egen computer.

## Sådan kommer I i gang

### 1: Skriv dig ind som samarbejdspartner — hver for sig

1. **Fork** dette repository: *Fork* øverst til højre → *Create fork*.
2. **Clone** *din egen fork* i VS Code.
3. Kopiér `samarbejdspartnere/_skabelon.md` til `samarbejdspartnere/<dit-brugernavn>.md`.
   Små bogstaver, ingen mellemrum, ingen æ, ø eller å.
4. Udfyld filen, commit med en god besked, og push.
5. På din fork på GitHub: *Contribute* → *Open pull request*.

Når din pull request er merget, står du på listen over samarbejdspartnere.

### 2: Sæt gruppens projekt op i studiegruppen

GitHub tillader kun én fork pr. konto. I har allerede hver jeres, så én af dem skal
være gruppens.

1. **Vælg, hvis fork der skal være gruppens.**
2. Den person: gå til sin fork → *Sync fork* → *Update branch*. Nu er forken
   identisk med originalen, med alle samarbejdspartnere.
3. Samme person: *Settings* → *Collaborators* → tilføj resten af gruppen.
4. **De andre:** slet jeres egen fork — *Settings* → *Delete this repository*. Den har
   gjort sit arbejde, og så kan I ikke komme til at clone den forkerte.
5. **De andre:** acceptér invitationen, der kommer på mail, og clone **gruppens fork**.
6. Skriv jer ind i `GRUPPE.md` **én ad gangen**: pull, tilføj jeres linje, commit, push.

Herfra sender I ikke pull requests tilbage til dette repository. Gruppens fork er
jeres projekt, og det er den, I publicerer fra. Kommer der nyt her, fx
referencetallene, henter I det med *Sync fork*.

## Undervejs

Barometeret bliver bygget i trin, der følger kurset. 

## Kilde

Qvist, J. F. & Larsen, C. A. *Mod diversitet på arbejdspladsen.*
