---
name: aifit-systeemcheck
description: >-
  Systeemcheck voor AI FiT Leiderschap. Test of de app, de gekoppelde map, de browser,
  de Chrome-extensie en computer use werken, leest de specificaties van de laptop af en
  geeft een eerlijk oordeel: haalt dit apparaat de vijf weken, is het nog van deze tijd,
  en wat kan beter. Gebruik bij "Doe de systeemcheck van AI FiT Leiderschap", "ben ik
  klaar voor AI FiT", "kan mijn laptop dit aan", en direct na het installeren van
  github.com/hpamike/aifit-starterskit. NIET voor algemene IT-support buiten dit programma.
---

# Systeemcheck AI FiT Leiderschap

**Instructie voor de assistent, Claude of ChatGPT.** De deelnemer heeft in zijn werkboek
("Vooraf: installeren", stap 1 en 2) de app geïnstalleerd en de instellingen zelf
aangezet. Jij zet niets aan. Jij **test** wat er staat, **leest zijn laptop af** en geeft
een **eerlijk oordeel** met tips.

Reken op een kwartier en zeg dat aan het begin.

## Drie regels die overal gelden

1. **Getest of gehoord.** Zeg bij alles hoe je het weet. "Ik heb gecontroleerd" zeg je
   alleen als je het zelf hebt gezien. Wat hij vertelt, noteer je als gehoord.
2. **Verzin niets.** Geen menupaden, geen eisen en geen specificaties die je niet hebt
   gelezen. Weet je iets niet zeker, zeg dat dan.
3. **Slecht nieuws zonder omhaal.** Noem wat het kost en wat hij eraan kan doen. Een
   oude laptop is geen schande, maar wel een middag wachten in week 3.

## Stap 0: Waar draai je?

Bepaal dit eerst. Het bepaalt hoe je zijn laptop afleest.

| Omgeving | Zo herken je het | Specificaties aflezen |
|---|---|---|
| **Claude Cowork** met computer use | `uname` in je shell geeft `Linux` terwijl hij op een Mac of Windows werkt, en je hebt computer-use-gereedschap | Zelf, via de schermen van zijn systeem (route A in deel 2) |
| **Claude Cowork** zonder computer use, **Claude Chat**, **ChatGPT** | Geen computer use | Via één schermafbeelding van hem (route B in deel 2) |
| **Claude Code** (tabblad Code) | Je shell draait op zijn eigen computer: `uname` geeft `Darwin`, of je zit in PowerShell op Windows | Zelf, met de commando's onder "Alleen in Claude Code" in deel 2 |

**De systeemcheck vraagt de deelnemer nooit om Terminal of PowerShell te openen.** Dat is
voor deze doelgroep te technisch, en het is ook niet nodig. De enige uitzondering is de
optionele extra check aan het eind, en alleen als hij dat zelf wil.

**Gebruik in Cowork nooit de cijfers van je eigen shell.** Die gaan over de afgeschermde
omgeving, niet over zijn laptop. Een vergissing hier levert een oordeel op over een
computer die hij niet heeft.

Begin zo:

> Ik loop in een kwartier je hele opstelling na. Eerst test ik of alles werkt wat je in
> je werkboek hebt aangezet. Daarna lees ik je laptop af en vertel ik eerlijk of hij de
> vijf weken aankan, of hij nog van deze tijd is, en wat je kunt verbeteren. Ik verander
> niets aan je computer.

---

## Deel 1: De keten

Loop de onderdelen af en zeg per regel wat je deed.

| Onderdeel | Zo test je het | Blokkeert |
|---|---|---|
| **Map gekoppeld** | Noem wat je in `AIFiT Leiderschap` ziet, of "de map is leeg" | Week 1 |
| **Code uitvoeren en bestanden maken** (Settings → Capabilities) | Schrijf een klein testbestand in zijn map, lees het terug en gooi het weg. Lukt weggooien niet, laat het dan staan en noem de naam | Week 1 |
| **Browser** (Preferred browser: Chrome) | Open een publieke pagina (bijvoorbeeld `https://aifit.nu`) en zeg wat je ziet, en in welke browser je dat deed | Niets |
| **Chrome-extensie** (Claude in Chrome) | Laat hem in Chrome een tabblad openen, bijvoorbeeld `https://aifit.nu`. Lees de titel van dat tabblad terug. Heb je geen gereedschap dat in zijn Chrome kan kijken, dan is de extensie niet geïnstalleerd, niet ingelogd of niet verbonden. Laat hem dan in Chrome het puzzelstukje openen en kijken of "Claude" erbij staat en of hij is ingelogd | Niets. Zonder extensie kopieert hij in week 3 zelf heen en weer |
| **Computer use** (Settings → General) | Twee tests. Eén: maak een schermafbeelding en zeg wat je ziet. Twee: vraag toestemming en open zelf een onschuldig programma, zoals Rekenmachine, en sluit het weer. Lukt kijken maar niet bedienen, dan heeft hij het half aangezet of nog geen toegang gegeven voor dat programma. Krijg je niets, dan staat het uit, hoe zeker hij ook is | Niets. Zonder computer use lees je zijn specificaties via hem |

Het venster van de app zelf (Settings) kun je niet uitlezen, ook niet met computer use.
Daar test je het effect, niet de knop. Faalt een test, noem dan de instelling uit de
eerste kolom; dat is de plek in zijn werkboek waar hij moet terugkijken.

Vraagt de app tijdens een test om toestemming (voor een programma, een website of zijn
map), zeg dan wat je wilt doen en waarom. **Laat hem zelf op toestaan klikken; doe dat
nooit voor hem.**

**In Claude Chat of ChatGPT** bestaan map, schrijven en computer use niet in deze vorm.
Markeer ze als "niet van toepassing hier" en zeg in één zin dat de sessies met Claude
Cowork worden gedemonstreerd. Doet hij het programma met ChatGPT, dan zie je in deel 3
wat dat per week betekent.

---

## Deel 2: De specificaties

Je hebt nodig: besturingssysteem en versie, model en bouwjaar, processor, werkgeheugen,
vrije en totale schijfruimte, accuconditie, op Windows of virtualisatie aanstaat, en of
Chrome, git en (bij ChatGPT) Codex er staan.

Zeg vooraf in één zin wat je gaat doen: *"Ik open een paar schermen in je
systeeminstellingen om je laptop af te lezen. Ik verander niets en sluit alles weer."*
Vraag de app om toestemming, en laat hem zelf op toestaan klikken.

**Neem geen serienummer, Apple-account of accountnaam over** in je rapport, ook al staan
ze op hetzelfde scherm.

### Route A: zelf aflezen met computer use

**Mac**, in Systeeminstellingen. Open de panelen via het menu **Weergave** van
Systeeminstellingen; dat is betrouwbaarder dan klikken in de zijbalk.

| Paneel | Wat je afleest |
|---|---|
| **Info** | Model en jaar (bijvoorbeeld "13-inch, M4, 2025"), chip, geheugen, macOS-versie |
| **Opslag** | Gebruikt en totaal; reken het vrije deel uit. Staat er "Berekenen…", wacht dan even |
| **Batterij** → ⓘ naast Batterijconditie | Conditie (Normaal of Onderhoud aanbevolen) en maximumcapaciteit |

Daarna Chrome, Codex en Xcode: die zie je in de **lijst met geïnstalleerde apps** van je
computer-use-gereedschap, zonder iets te openen. Let op: de Codex-app kan als "ChatGPT"
in de lijst staan (bundel `com.openai.codex`).

**Git op de Mac** zie je niet in de app-lijst. Kijk in **Finder → Ga → Ga naar map** en
vul het pad in. Finder stelt alleen paden voor die bestaan. Komt het pad als suggestie
terug, dan staat git er. Kijk in deze volgorde:

1. `/Library/Developer/CommandLineTools/usr/bin/git` (de Command Line Tools, de gewone route)
2. Xcode in de app-lijst (die heeft git ingebouwd)
3. `/opt/homebrew/bin/git` (git via Homebrew)

Sluit het venster daarna met **Sluit** of Escape. Lukt het invullen niet na twee
pogingen, noteer git dan als ⚪ "niet gecontroleerd". Week 5 vangt het op. **GitHub
Desktop telt niet:** de git daarin werkt alleen binnen dat programma.

**Windows**, in Instellingen en Taakbeheer:

| Waar | Wat je afleest |
|---|---|
| **Instellingen → Systeem → Info** | Processor, geïnstalleerd RAM, Windows-editie, versie en build |
| **Instellingen → Systeem → Opslag** | Gebruikt en vrij op de C-schijf |
| **Taakbeheer → Prestaties → CPU** | "Virtualisatie: Ingeschakeld" of "Uitgeschakeld" |

Chrome, Codex en git zie je in de **lijst met geïnstalleerde apps**; git staat er als
"Git Bash" of "Git". De accuconditie toont Windows niet op een scherm. Vraag alleen hoe
lang hij op de accu werkt, en noteer het als gehoord.

Dat computer use op Windows precies zo werkt als op een Mac, is niet getest. Lukt het
aflezen niet, ga dan naar route B.

Sluit alle vensters die je hebt geopend weer.

### Route B: één schermafbeelding van hem

Zonder computer use, in Chat of in ChatGPT, laat je hem één scherm openen en er een
schermafbeelding van plakken. Geef de stappen één voor één:

- **Mac:** Appelmenu → **Over deze Mac**. Druk **⌘ Shift 4**, dan de **spatiebalk**, en
  klik op het venster. De afbeelding staat op het bureaublad; sleep die in de chat.
- **Windows:** Start → **Instellingen → Systeem → Info**. Druk **Windows Shift S**, kies
  venster en klik op Instellingen. Plak met **Ctrl V** in de chat.

Daaruit lees je model, chip of processor, geheugen en versie. Vraag de rest in gewone
woorden en noteer het als gehoord:

- *"Hoeveel ruimte is er nog vrij? Dat staat in Instellingen onder Opslag."*
- *"Gaat je accu nog een werkdag mee?"*
- *"Heb je Chrome?"*

Git noteer je in route B als ⚪ "niet gecontroleerd"; dat komt in week 5.

### Alleen in Claude Code

Heb je zelf een shell op zijn computer, voer dan dit uit. **Geef het nooit aan de
deelnemer.**

- Mac: `sw_vers; sysctl -n machdep.cpu.brand_string hw.memsize; df -h /System/Volumes/Data; system_profiler SPHardwareDataType SPPowerDataType | grep -E "Model Name|Chip|Memory:|Cycle Count|Condition|Maximum Capacity"; xcode-select -p >/dev/null 2>&1 && git --version || echo "git: niet geinstalleerd"`
- Windows (PowerShell): `Get-ComputerInfo -Property OsName,OsVersion,CsProcessors,CsTotalPhysicalMemory,HyperVisorPresent; Get-PSDrive C; git --version`

### Zo lees je de uitkomst

- **Bouwjaar.** Op de Mac staat het jaar in Info. Op Windows leid je het af uit de
  processor. Weet je het niet zeker, zeg dan "ongeveer" of "onbekend".
- **Accu (Mac).** Bij "Onderhoud aanbevolen" of een maximumcapaciteit onder 80% is de accu
  op.

---

## Deel 3: Het oordeel

Geef het oordeel in vier lagen, in deze volgorde.

### 3a. Harde eisen: kan het überhaupt?

Cowork vraagt **macOS 14 (Sonoma) of nieuwer**, of **Windows 10 build 19041 of nieuwer
met werkende hardwarevirtualisatie** (bron: installatiepagina Claude Desktop,
geraadpleegd 10-09-2026). Op Windows is daarbij het `.msix`-pakket nodig. Wie met een
ouder `.exe`-bestand installeerde, heeft Claude Desktop zonder Cowork. **Verzin geen eis
die hier niet staat.**

Zit hij daaronder, dan is bijwerken de enige route. Kan dat niet, dan haalt deze laptop
het programma niet. Zeg dat meteen.

Twijfel je, laat hem dan de officiële readiness-check draaien. Die weegt zwaarder dan jouw
inschatting. Geef alleen de link voor zijn platform:

- Mac: `https://claude.ai/api/desktop/darwin/universal/cowork-readiness-check/latest/redirect`
- Windows x64: `https://claude.ai/api/desktop/win32/x64/cowork-readiness-check/latest/redirect`
- Windows Arm: `https://claude.ai/api/desktop/win32/arm64/cowork-readiness-check/latest/redirect`

### 3b. Per week: haalt hij de vijf weken?

Geef geen rapportcijfer. De vraag is of hij deze vijf weken doorkomt, en de weken vragen
verschillende dingen.

| Week | Wat het vraagt | Waar het knelt |
|---|---|---|
| 1, 2 en 4 | Praten, schrijven, één browsertabblad | Vrijwel nergens, als de app draait |
| 3 | Claude en vijf browsergereedschappen tegelijk open (Perplexity, NotebookLM, Gemini, Gamma, Lovable) | **Geheugen.** Met 8 GB gaat het zwoegen, met minder wordt het een middag wachten |
| 5 | Claude Code bouwt een dashboard en zet het via GitHub online | **Schijfruimte en git.** Onder 20 GB vrij is krap, onder 10 GB moet hij eerst opruimen. Zonder git komt er in week 5 een download van ongeveer een gigabyte bij |

### 3b-2. Vibecoden

In week 5 bouwt hij in Claude Code (of Codex, als hij met ChatGPT werkt) een dashboard als
één `index.html`. Dat zet hij via GitHub online op Vercel. De systeemcheck kijkt alleen
naar wat niet vanzelf goedkomt:

- **Bouwomgeving.** Opent het tabblad **Code** in de Claude-app bij hem? Of is de
  Codex-app of `codex` gevonden (bij ChatGPT)? Zit je zelf in Claude Code, dan is dit
  getest; anders is het gehoord. Claude Code hoort bij Pro of hoger, Codex bij een betaald
  ChatGPT-abonnement. Zeg niet meer over abonnementen dan je zeker weet.
- **Git.** Kijk of het er staat (zie deel 2). Op Windows kan hij het nu al zelf
  installeren met een gewoon installatieprogramma. Op de Mac gaat installeren via een
  commando; dat doet Claude Code in week 5, en de deelnemer klikt alleen op Installeren.
- **Schijfruimte.** Zie 3b.

**Wat je niet controleert:** de accounts (GitHub, Vercel, de gereedschappen van week 3),
de GitHub CLI, naam en e-mail in git, en Homebrew of winget. Dat regelt de deelnemer in
de opwarming van de week waarin hij het nodig heeft, met zijn werkboek erbij. Begint hij
er zelf over, zeg dan: *"Dat komt vanzelf in de opwarming van week 5."*

**Werkt hij met ChatGPT,** zeg dan eerlijk dat de begeleiding en de demonstraties op Claude
zijn gebouwd. Week 1, 3 en 4 gaan met ChatGPT prima. Week 2 (een eigen assistent als
Claude Skill) doet hij met de dichtstbijzijnde variant in ChatGPT, en week 5 met Codex
in plaats van Claude Code. Dat lukt, maar met minder hulp uit het materiaal. Zeg niet welke variant precies
werkt als je dat niet zeker weet.

### 3c. Is dit apparaat nog van deze tijd?

Dit is het eerlijke oordeel waar hij om vroeg, los van het programma. Gebruik deze
ijkpunten en **zeg erbij dat het jouw ijkpunten zijn voor 2026, geen eis van Anthropic of
OpenAI.**

| | Loopt achter | Prima | Van deze tijd |
|---|---|---|---|
| Werkgeheugen | 8 GB of minder | 16 GB | 16 GB of meer |
| Processor (Mac) | Intel | M1 of M2 | M3 of nieuwer |
| Processor (Windows) | Te oud voor Windows 11 | Draait Windows 11 | Recent, ongeveer 2023 of later |
| Opslag | Minder dan 256 GB, of geen SSD | 256 GB SSD | 512 GB SSD of meer |
| Besturingssysteem | Krijgt geen updates meer | Krijgt nog updates | Nieuwste versie |
| Leeftijd | Ouder dan zes jaar | Drie tot zes jaar | Jonger dan drie jaar |
| Accu | Op (zie deel 2) | Gaat een werkdag mee | Gaat ruim een werkdag mee |

Twee feiten die je mag noemen als ze voor hem gelden:

- **Windows 10** krijgt na 13 oktober 2026 ook via het verlengde programma (ESU) geen
  beveiligingsupdates meer. Draait hij Windows 10, dan is overstappen op Windows 11 geen
  luxe maar onderhoud.
- **Intel-Macs.** Apple heeft aangekondigd dat macOS 26 (Tahoe) de laatste versie voor
  Intel-Macs is. Na die versie komen er dus geen grote updates meer.

Vat het samen in één zin. Bijvoorbeeld: *"Je laptop is vijf jaar oud en heeft 8 GB: voor
dit programma gaat het, maar hij loopt achter op wat AI-werk in 2026 vraagt."*

### 3d. Tips om te verbeteren

**Geef alleen tips die voor zijn apparaat gelden, maximaal vijf**, in volgorde van kosten.
Noem per tip wat het oplevert.

- **Gratis, vandaag nog:**
  - Besturingssysteem en Chrome bijwerken.
  - Ruimte vrijmaken tot minstens 20 GB vrij: op de Mac via Systeeminstellingen →
    Algemeen → Opslag, op Windows via Instellingen → Systeem → Opslag.
  - Programma's uitzetten die bij het opstarten meestarten.
  - Ongebruikte browserextensies verwijderen.
  - Eén keer per week opnieuw opstarten.
- **Gratis, op de dag van week 3:** sluit alles wat je niet nodig hebt en werk in één
  Chrome-venster met de vijf tabbladen.
- **Goedkoop:**
  - Een externe SSD voor archief, foto's en oude projecten. Zet de map
    `AIFiT Leiderschap` daar niet op; die hoort op de interne schijf.
  - Een nieuwe accu als die op is.
- **Vervangen:** alleen als het besturingssysteem geen updates meer krijgt of als 8 GB
  samengaat met een processor uit de kolom "loopt achter". Adviseer dan minimaal 16 GB
  en 512 GB SSD. Noem geen merken of prijzen tenzij hij erom vraagt.

Raad hem nooit aan om voor dit programma een nieuwe laptop te kopen als week 3 het
enige knelpunt is. Een andere laptop lenen voor die ene middag is dan het eerlijke advies.

---

## Afsluiten

Geef het rapport als **één tabel: criterium, status, oordeel.** Gebruik altijd deze
rijen, in deze volgorde. Ontbreekt een rij in de tabel, dan lijkt hij te zijn vergeten.

**Status:**
- 🟢 **Groen:** in orde, er hoeft niets te gebeuren.
- 🟠 **Oranje:** het werkt, maar het kost iets (tijd, traagheid). Er is een
  aandachtspunt.
- 🔴 **Rood:** het blokkeert. Zonder oplossing lukt minstens één week niet.
- ⚪ **Wit:** niet gecontroleerd of niet van toepassing. Zeg in het oordeel waarom.

Zet in de kolom oordeel wat je zag of hoorde, met *(getest)* of *(gehoord)* erachter.

**Bij elke oranje of rode rij hoort handelingsperspectief.** Dat is altijd concreet: wat
hij doet, waar, en hoe lang het duurt of wat het kost. Dus niet *"meer geheugen zou
helpen"*, maar *"sluit in week 3 alles behalve Chrome en Claude; dat scheelt merkbaar"*.
Kan hij er niets aan doen, zeg dan wat het betekent en hoe hij eromheen werkt. Een oranje
of rode rij zonder actie is niet af.

| # | Criterium | 🟢 Groen | 🟠 Oranje | 🔴 Rood | Wat hij doet bij 🟠 of 🔴 |
|---|---|---|---|---|---|
| **Instellingen** | | | | | |
| 1 | Map `AIFiT Leiderschap` gekoppeld | Gezien | — | Niet gekoppeld | Map aanmaken, dan in Cowork onder het chatvenster de map kiezen. Werkboek, Vooraf stap 2 |
| 2 | Code uitvoeren en bestanden maken | Testbestand geschreven en gelezen | — | Schrijven lukt niet | Settings → Capabilities, aanzetten, nieuw gesprek starten en opnieuw testen |
| 3 | Browser | Pagina geopend in Chrome | Geopend, maar niet in Chrome | Geen pagina te openen | Oranje: Settings → Cowork → Preferred browser op Chrome. Rood: internet en webtoegang nakijken; lukt dat niet, schermafbeelding naar de begeleider |
| 4 | Chrome-extensie | Tabblad meegelezen | Niet geïnstalleerd, niet verbonden of niet ingelogd | — | Chrome Web Store, "Claude in Chrome" toevoegen, puzzelstukje, inloggen. Vijf minuten |
| 5 | Computer use | Kijken en bedienen werkt | Alleen kijken, of uit | — | Settings → General → Enable computer use. Bij alleen kijken: de toegang voor het programma toestaan als de app daarom vraagt |
| **Apparaat** | | | | | |
| 6 | Besturingssysteem | Actueel en krijgt updates | Haalt de eis, maar is verouderd of krijgt binnenkort geen updates meer | Onder de harde eis uit 3a | Bijwerken via Software-update (Mac) of Windows Update. Reken op een uur, doe het niet op de dag van een sessie. Kan het niet, zie rij 12 |
| 7 | Virtualisatie (Windows) | Taakbeheer: Virtualisatie Ingeschakeld | — | Uitgeschakeld | Aanzetten in het BIOS/UEFI. Dat verschilt per merk: zoek op "[merk en model] virtualisatie inschakelen" of vraag de IT-afdeling. Werkgever-laptop: altijd via IT |
| 8 | Processor | M3 of nieuwer, of recente x64/Arm | M1 of M2, of ouder maar Windows 11-geschikt | Intel-Mac, of te oud voor Windows 11 | Oranje: niets nodig voor dit programma. Rood: werkt nog, maar dit is het eerste apparaat om te vervangen; zie 3d |
| 9 | Werkgeheugen | 16 GB of meer | 8 GB | Minder dan 8 GB | Sluit in week 3 alles behalve Chrome en Claude, en werk in één venster. Rood: leen voor week 3 een andere laptop |
| 10 | Vrije schijfruimte | 20 GB of meer | 10 tot 20 GB | Minder dan 10 GB | Opruimen via Systeeminstellingen → Algemeen → Opslag (Mac) of Instellingen → Systeem → Opslag (Windows). Begin bij Downloads en grote video's. Doel: 20 GB vrij vóór week 5 |
| 11 | Accu | Gaat een werkdag mee | Capaciteit 80 tot 85% | Onderhoud aanbevolen, onder 80%, of (extra check) meer dan 1000 cycli | Neem de lader mee naar elke sessie. Rood: accu laten vervangen, bij Apple of een reparateur |
| 12 | Leeftijd apparaat | Jonger dan drie jaar | Drie tot zes jaar | Ouder dan zes jaar | Oranje: niets nodig voor dit programma. Rood: plan vervanging; adviseer minimaal 16 GB en 512 GB SSD |
| **Vibecoden** | | | | | |
| 13 | Claude Code of Codex | Aanwezig | Onbekend | Niet beschikbaar op zijn abonnement | Oranje: open het tabblad Code één keer en zeg wat je ziet. Rood: abonnement ophogen vóór week 5, of week 5 meekijken met een tafelgenoot |
| 14 | Git | Geïnstalleerd | Niet geïnstalleerd, of niet gecontroleerd | — | Mac: niets nu; in week 5 start Claude Code de installatie en klik jij op **Installeren** (ongeveer een gigabyte). Windows: kan nu al via `https://git-scm.com/download/win`, gewoon doorklikken met de standaardkeuzes |

**Rood komt alleen voor bij rij 1, 2, 3, 6, 7, 10 en 13, plus rij 8, 9, 11 en 12 als het
apparaat echt tekortschiet.** Zo blijft rood zeldzaam en betekent het iets.

Zo zien rijen in het rapport eruit:

| Criterium | Status | Oordeel en wat te doen |
|---|---|---|
| Werkgeheugen | 🟠 | 8 GB *(getest)*. Prima voor week 1, 2, 4 en 5. **Doe:** sluit in week 3 alles behalve Chrome en Claude |
| Git | 🟢 | Versie 2.50 *(getest)* |
| Chrome-extensie | 🟠 | Niet verbonden *(getest)*. **Doe:** klik in Chrome op het puzzelstukje en log in bij Claude, vijf minuten |
| Vrije schijfruimte | 🔴 | 7 GB vrij *(getest)*. Week 5 lukt zo niet. **Doe:** ruim via Opslag minstens 13 GB op; begin bij Downloads |

**Onder de tabel** zet je drie korte dingen:

1. **De samenvatting in één regel per kleur,** bijvoorbeeld: *"10 groen, 2 oranje, 1 rood,
   1 niet van toepassing."* Witte rijen tel je apart; tel ze nooit mee als groen.
2. **De zin uit 3c:** is dit apparaat nog van deze tijd?
3. **Tips om te verbeteren** uit 3d, maximaal vijf. Wat al in de tabel staat als actie,
   herhaal je hier niet. Hier komt alleen wat verder gaat dan de rode en oranje rijen.

Sluit af met één van deze twee, en niet met iets ertussenin.

**Klaar.** Er staat geen enkele rode rij. *"Je laptop en je instellingen zijn klaar voor
AI FiT Leiderschap."* Staat er oranje, voeg dan toe: *"Let op de oranje punten."*

**Nog niet klaar.** Er staat minstens één rode rij. Noem de rode rijen (maximaal drie), in
volgorde, met per stuk wat het kost en wat hij eraan kan doen. Oranje alleen maakt nooit
"nog niet klaar". Kom je er samen niet uit, zeg dan dat hij een schermafbeelding naar de
begeleider kan sturen.

**Kun je schrijven in zijn map,** zet het rapport (de tabel en wat eronder staat) dan in
`AIFiT Leiderschap/SYSTEEMCHECK-UITSLAG.md`, met de datum erbij. Dan hoeft hij hem in de
eerste sessie niet te onthouden.

Staat er geen rood, zet dan direct onder het rapport de **optionele extra check** (zie
hieronder), met het commando en de stappen erbij.

Onderbroken? Dan typt hij later:

```
Doe de systeemcheck van AI FiT Leiderschap.
```

---

## Optioneel: de extra check via Terminal

**Staat er geen rode rij in het rapport, geef deze check dan meteen, in hetzelfde bericht,
direct onder het rapport.** Wacht niet tot hij erom vraagt. Staat er wel rood, los dat
dan eerst op; de extra check komt daarna.

Geef alleen het commando voor zijn eigen platform, met de stappen erbij, in deze vorm:

> **Optioneel: een extra check van twee minuten.** Hiermee lees ik twee dingen af die
> niet op de schermen staan: het aantal laadcycli van je accu en de versie van git.
> Overslaan is helemaal prima; je bent al klaar.
>
> 1. Druk op **⌘ spatie**, typ **Terminal** en druk op **Enter**.
> 2. Klik op de kopieerknop rechtsboven in het grijze blok hieronder.
> 3. Klik in het Terminal-venster, plak met **⌘ V** en druk op **Enter**.
> 4. Zeg hier "klaar". Ik lees de uitkomst af en werk je rapport bij.
>
> [het codeblok voor zijn platform]
>
> Dit commando leest alleen. Het verandert niets en verstuurt niets.

Op **Windows**: stap 1 wordt *"Klik op Start, typ **PowerShell** en druk op **Enter**"*, en
plakken gaat met **Ctrl V**.

Met computer use zet je het commando daarnaast op zijn klembord. Zeg dan bij stap 2: *"Het
staat al op je klembord; deze stap kun je overslaan."*

Zegt hij nee, of reageert hij er niet op, ga dan niet overtuigen. Het rapport is af.

**Wat het toevoegt:** het aantal laadcycli (Mac), de git-versie (of git ontbrak in route
B), en op Windows de exacte vrije ruimte en of de hypervisor actief is.

**Vrije ruimte op de Mac haal je niet uit Terminal.** `df` toont daar de systeemschijf en
geeft een veel te laag getal. Houd het getal uit Systeeminstellingen → Opslag aan.

**Als hij "klaar" zegt:**

1. **Lees de uitkomst.** Met computer use lees je het Terminal-venster zelf af. Je mag
   daar kijken en klikken, maar niet typen; dat hoort zo. Zonder computer use plakt hij de
   uitkomst terug, of een schermafbeelding.
2. **Werk de betreffende rijen in het rapport bij** en zeg wat er veranderde.
3. **Zeg dat hij Terminal weer mag sluiten.**

Verschijnt er op de Mac toch een venster over "command line developer tools", laat hem
dan op **Annuleer** klikken. Installeren komt in week 5.

**Mac:**

```bash
sw_vers; sysctl -n machdep.cpu.brand_string; echo "$(( $(sysctl -n hw.memsize) / 1073741824 )) GB geheugen"; system_profiler SPHardwareDataType SPPowerDataType 2>/dev/null | grep -E "Model Name|Chip|Memory:|Cycle Count|Condition|Maximum Capacity"; if xcode-select -p >/dev/null 2>&1; then git --version; else echo "git: niet geinstalleerd"; fi
```

**Windows:**

```powershell
$o=Get-CimInstance Win32_OperatingSystem; $c=Get-CimInstance Win32_ComputerSystem; $p=@(Get-CimInstance Win32_Processor)[0]; "$($o.Caption) build $($o.BuildNumber)"; "$($c.Manufacturer) $($c.Model)"; "$($p.Name)"; "{0:N0} GB geheugen" -f ($c.TotalPhysicalMemory/1GB); Get-PSDrive C | % {"{0:N0} GB vrij van {1:N0} GB" -f ($_.Free/1GB),(($_.Used+$_.Free)/1GB)}; "Hypervisor actief: $($c.HypervisorPresent)"; if(Get-Command git -EA 0){git --version}else{"git: niet geinstalleerd"}
```

Bij **Cycle Count** boven 1000 wordt de accu rood (rij 11). Bij **Hypervisor actief: True**
werkt virtualisatie.

---

## Als hij ernaar vraagt

**Een API-sleutel?** Nee. *"Je hebt geen API-sleutel nodig. Alles loopt via de app waar je
nu in zit, op je gewone abonnement. Een API-sleutel is bedoeld voor programmeurs die iets
automatisch laten draaien, en dat doen we hier niet."* Dat geldt ook voor week 5.

**Git, een terminal of programmeergereedschap?** Tot en met week 4 heeft hij dat niet
nodig. In week 5 wel, en dat wordt dan begeleid: de accounts, de GitHub CLI en inloggen
komen in de opwarming van week 5. Programmeerkennis is niet nodig, en hij hoeft zelf geen
Terminal te openen. Op Windows mag git nu al geïnstalleerd worden (rij 14).

**Een netwerkschijf (Windows)?** Die moet een stationsletter hebben om als map te koppelen.
Een pad als `\\server\share` werkt niet. Beter nog is een gewone lokale map.
