# EVE Online — modularne corp skillplany

Wersja: **2026-09-05**
Liczba szablonów planów w paczce: **100**

## Cel

Ta biblioteka zastępuje jeden wielki "generic must have" zestawem modułów.
Pilot bierze wspólne CORE, a potem tylko tank, broń, scout/cyno i hulle,
których faktycznie potrzebuje.

Główna zasada:

- **READY** — funkcjonalny, bez rażących dziur.
- **STANDARD** — poziom, który corp może uczciwie nazwać "dobrym pilotem" danej roli.
- **SPECIALIST** — kosztowne V tylko tam, gdzie bonus/prerequisite uzasadnia czas.
- Nie każdy plan ma wszystkie trzy nazwy; system broni może mieć do 5 milestone'ów,
  a plan binarny (np. Covert Cyno) tylko jeden.

## Struktura

- 00–04 — CORE
- 10 — combat fitting / damage mods
- 20–22 — armor
- 30–31 — shield
- 50–53 — turrets
- 60–63 — missiles
- 70–74 — drones
- 80–82 — scout
- 83–85 — cyno
- 90–99 — hull progression

Tactical Destroyery są celowo wchłonięte do racial planów `91 HULL - Destroyer`,
żeby nie marnować 4 dodatkowych corp-plan slots. `82 SCOUT - Covert Operations`
zastępuje osobny duplikat `97 HULL - Covert Ops`.

Specjalistyczny rigging został celowo "wchłonięty" przez właściwe plany.
`04 CORE - Rigging Foundation` zawiera tylko Mechanics/Jury Rigging.

## Jak używać plików

Każdy katalog planu ma:

- `PLAN.md` — opis, dependencies i milestone'y.
- `READY.txt`, `STANDARD.txt`, `SPECIALIST.txt` albo inne pliki milestone'ów —
  czyste kolejki z jedną umiejętnością/poziomem na linię.

Pliki `.txt` używają formatu typu:

    Navigation I
    Navigation II
    Navigation III
    Navigation IV

który można kopiować do skill queue. W EVE Corporate Skill Plan milestone metadata
ustawia się w edytorze planu — zwykły tekst kolejki nie przenosi nazw milestone'ów.

## Ważne: limit corp planów

CCP pozwala korporacji zapisać maksymalnie **100 corporation skill plans**.
Paczka zawiera **dokładnie 100 szablonów**, czyli mieści się w aktualnym limicie corp.
W praktyce warto publikować tylko używane doktryny/role i zostawić kilka slotów na przyszłe EWAR/logi/boosting plany.

Najprostsza polityka:
1. wrzuć wszystkie 00–85, których corp faktycznie używa;
2. z 90–99 publikuj tylko aktywne doktryny / używane rasy / używane klasy;
3. resztę trzymaj w tym ZIP-ie jako library/template.

## Cross-plan dependencies

Plany są modułowe. Nie dubluję wszędzie całego CORE.
Przykładowo:
- Gallente armor blaster cruiser: 00 + 01 + 02 + 03 + 04 + 10 + 20 (+21/22) + 50 + 51 + 92 Gallente.
- Caldari shield HAM cruiser: 00 + 01 + 02 + 03 + 04 + 10 + 30 + 60 + 62 + 92 Caldari.
- Scout combat prober: 00 + 01 + 02 + 03 + 04 + 80 + 81; opcjonalnie 82.
- BLOPS hunter: Scout + 82 + 85 + właściwy hull.
- JF cyno alt: 00 + 01 + 83 + odpowiedni hull dla Industrial Cyno.
- Hard cyno: 84 + Force Recon albo Black Ops hull.
- Drone pilot: 00 + 01 + 02 + 03 + 04 + 10 + wybrany tank + 70 + potrzebne 71–74.

## Co jest świadomie pominięte

Ta paczka nie próbuje jeszcze robić osobnych bibliotek:
- EWAR (TD/damp/ECM/paint/tackle),
- Logistics/remote repair support,
- Command Burst / fleet boosting support,
- Fighters,
- Capital weapon systems i capital tank,
- Hacking/Archaeology jako "explorer" (Scout służy skanowaniu),
- Industry/production/reprocessing.

Hull plans 97/99 zawierają prerequisites do wejścia w klasę, ale to **nie znaczy**,
że pilot po samym hull planie jest gotowym logi/dread/carrierem. Broń/tank/role
pozostają modułami.

## Ważne decyzje projektowe

- `CPU Management V`, `Power Grid Management V`, `Capacitor Systems Operation V`
  są STANDARD, bo oddziałują praktycznie na każdy combat ship.
- `Advanced Weapon Upgrades IV` jest STANDARD; V jest SPECIALIST/prerequisite.
- `Long Range Targeting V` nie jest generic core — jest SPECIALIST i prerequisite
  określonych klas, np. Logistics Cruisers.
- `Tactical Shield Manipulation IV` jest naturalnym shield stopem; V jest SPECIALIST.
- `Repair Systems IV` jest armor-active STANDARD; V specialist.
- `Thermodynamics IV` jest PvP STANDARD.
- W scanningu Rangefinding ma najwyższy priorytet; Acquisition rośnie w Combat Probing.
- Covert Cyno jest binarne: wymaga Cynosural Field Theory V.
- Hard cyno nie jest już "Ibis cyno": aktualnie zwykły generator wymaga Force Recon/Black Ops.

## Current-data caveats (2026-09-05)

1. **Mining Barge**: aktualna tabela Spaceship Command pokazuje tymczasowy revert
   prerequisite z Mining Destroyer III z powrotem na Mining Frigate III.
2. **Gallente Titan**: aktualny EVE Ref/ship requirement pokazuje Gallente Battleship III,
   natomiast jedna tabela umiejętności EVE University nadal pokazuje Gallente Battleship V.
   Paczka używa III zgodnie z aktualnym EVE Ref. Przed wielomiesięcznym titan trainingiem
   sprawdź prerequisite w kliencie.
3. **Command Carriers** są uwzględnione jako aktualna klasa 2026.
4. CCP zmienia czasem prerequisites; przed publikacją planów capital/T2 w corpie warto
   zrobić szybki sanity check w aktualnym kliencie.

## Źródła użyte do weryfikacji

- CCP Support — Skill Plans and How They Work:
  https://support.eveonline.com/hc/en-us/articles/4406388028178-Skill-Plans-and-How-They-Work
- EVE University — Skills: Spaceship Command:
  https://wiki.eveuniversity.org/Skills:Spaceship_Command
- EVE University — Skills: Engineering:
  https://wiki.eveuniversity.org/Skills:Engineering
- EVE University — Skills: Navigation:
  https://wiki.eveuniversity.org/Skills:Navigation
- EVE University — Skills: Drones:
  https://wiki.eveuniversity.org/Skills:Drones
- EVE University — Skills: Scanning:
  https://wiki.eveuniversity.org/Skills:Scanning
- EVE University — Skills: Missiles:
  https://wiki.eveuniversity.org/Skills:Missiles
- EVE University — Skills: Rigging:
  https://wiki.eveuniversity.org/Skills:Rigging
- EVE University — Cynosural Field:
  https://wiki.eveuniversity.org/Cynosural_Field
- EVE Ref — bieżące type requirements do punktowych kontroli.
