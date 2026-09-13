# CALDARI — Logistics training: Frigate → Destroyer fleet → Cruiser

> W tej wersji: `B` = BASIC, `S` = STANDARD, `I` = IMPROVED.

## Jak czytać ścieżki

Numery odnoszą się do aktualnej biblioteki **89 corp skillplanów**.

### Ważne: brak klasy Logistics Destroyer

EVE nie ma standardowej klasy **Logistics Destroyer** pomiędzy logi frigate i logi cruiser.
Dla flot destroyerowych normalną odpowiedzią są **T1/T2 Logistics Frigates**:
są szybkie, tanie i nadążają za frigate/destroyer gangiem.

Nie trzeba więc trenować `91 HULL - Destroyer`, żeby być logistykiem floty destroyerów.

Tactical Destroyery mają pojedyncze niszowe remote-rep możliwości (np. Confessor/Svipul w Defense Mode),
ale **nie traktujemy ich jako głównej corp ścieżki logi**.

### Problem obecnej biblioteki

Obecne 89 planów zawiera hull plans:
- `97 HULL - Logistics Frigates`
- `97 HULL - Logistics Cruisers`

ale **nie ma jeszcze pełnego LOGI SUPPORT planu** obejmującego remote repair, cap-chain i repair drones.
Dlatego poniżej podaję zarówno ścieżkę numerami, jak i skille, które trzeba dodać ręcznie / później zamienić na nowy corp plan.

### Wspólne supporty logi

Do wszystkich logi:

- `00 S` — cap/fitting jest krytyczny.
- `01 S` — logi musi utrzymywać range/transversal i nie zostawać z tyłu.
- `02`:
  - T1 frigate: `B` wystarczy, `S` lepsze;
  - T1 cruiser: **S**;
  - T2 Logistics Frigate: **S**;
  - T2 Logistics Cruiser: **I** jest bardzo sensowne (więcej locków + LRT V).
- `03 S` — dla PvP logi bardzo wartościowe: overheated reps/propmod mogą uratować flotę.

### Remote-repair skill thresholds

**Armor logi**
- `Remote Armor Repair Systems III` — sensowne minimum dla małych/T1 zastosowań.
- **IV** — właściwy standard, potrzebny do T2 large remote armor repairers.
- V — dedicated specialist / maksymalizacja capa.

**Shield logi**
- `Shield Emission Systems III` — Small Remote Shield Booster II.
- **IV** — Medium/Large Remote Shield Booster II i właściwy standard.
- V — dedicated specialist/capital.

**Cap-chain (Amarr/Caldari)**
- `Capacitor Emission Systems III` — można zacząć.
- **IV — minimum do poważnego cap-chain.**
- V — bardzo dobry cel dla dedicated Guardian/Basilisk.

**Repair drones**
- `Drones V`
- `Repair Drone Operation IV` — bardzo dobry standard.
- V — dedicated logi / T2 maintenance bots zależnie od dokładnej gałęzi.

### Hull levels logi

- T1 racial Frigate: **IV**, nie III, jeśli faktycznie latasz logi.
- `Logistics Frigates III` = tylko wejście; **IV = standard**, V specialist.
- T1 racial Cruiser: **IV**, bo bonus remote repair per level jest bardzo duży.
- `Logistics Cruisers III` = tylko etap treningu.
- **Logistics Cruisers IV = absolutne minimum do T2 cruiser logi.**
- **Logistics Cruisers V = wyjątkowo mocny cel**: ostatni poziom bardzo mocno poprawia realny koszt capa remote repów.


## Hulls

- T1 frigate: **Bantam** — remote shield.
- T2 frigate: **Kirin** — shield Logistics Frigate.
- T1 cruiser: **Osprey** — shield + cap-chain.
- T2 cruiser: **Basilisk** — shield + cap-chain.

---

## 1. T1 logi frigate — Bantam

`00 S → 01 S → 02 B/S → 30 B/S → 90 Caldari S`

+ `Shield Emission Systems III` minimum, **IV zalecane**
+ `Drones V`
+ `Repair Drone Operation III/IV`

`Caldari Frigate IV` jest realnym minimum do regularnego Bantama.

---

## 2. Logi dla destroyer gangów

Nie ma normalnego Caldari Logistics Destroyera.
Jackdaw nie ma pełnoprawnej logistycznej ścieżki remote-repair.

Standard:
- Bantam jako tani support,
- **Kirin** jako właściwy T2 logi dla szybkich frigate/destroyer fleetów.

Kirin:

`00 S → 01 S → 02 S → 30 S → 90 Caldari I → 97 Logistics Frigates S`

+ **`Shield Emission Systems IV`**
+ `Repair Drone Operation IV`

`97 LF III` = wejście; **LF IV = standard**.

---

## 3. T1 cruiser logi — Osprey

`00 S → 01 S → 02 S → 30 S → 92 Caldari S`

+ **`Shield Emission Systems IV`**
+ **`Capacitor Emission Systems IV`**
+ `Repair Drone Operation IV`

Osprey jest cap-chain logi. Cruiser III jest możliwy, ale **Cruiser IV** jest właściwym poziomem do floty.

---

## 4. T2 cruiser logi — Basilisk

`00 S → 01 S → 02 I → 30 S → 92 Caldari I → 97 Logistics Cruisers S`

+ `Shield Emission Systems IV/V`
+ **`Capacitor Emission Systems IV minimum, V bardzo zalecane`**
+ `Repair Drone Operation IV/V`

- Caldari Cruiser V obowiązkowe.
- **Logistics Cruisers IV absolutne minimum.**
- **Logistics Cruisers V bardzo mocny cel**.
- Basilisk cap-chain wymaga dobrych cap skills i poprawnej organizacji chaina.

## Źródła

- https://wiki.eveuniversity.org/Logistics
- https://wiki.eveuniversity.org/Skills:Shields
- https://wiki.eveuniversity.org/Skills:Spaceship_Command
