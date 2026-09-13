# AMARR — Battleship training recommendations

> W tej wersji: `B` = BASIC, `S` = STANDARD, `I` = IMPROVED.

## Jak czytać ścieżki

Numery odnoszą się do aktualnej biblioteki **89 corp skillplanów**.

- `B` = BASIC
- `S` = STANDARD
- `I` = IMPROVED
- `94 [rasa]` = racial Battleship plan
- `97 Logistics Frigates / Cruisers` = odpowiedni T2 hull plan

### Wspólna baza combat Battleship

`00 S → 01 S → 02 S → 03 S → 10 S`

Dla Battleshipów nie polecam budowania pilota na samych BASIC supportach.

| Plan | Minimum do pierwszych prób | Zalecane regularnie | Uwagi |
|---|---|---|---|
| `00 Engineering, Capacitor & Rigging` | B | **S** | BS-y są bardzo wrażliwe na fitting/cap |
| `01 Navigation` | B | **S** | BS jest wolny; agility/warp/propmod nadal mają znaczenie |
| `02 Targeting` | B | **S** | BS ma wolny lock; Signature Analysis V z S jest bardzo wartościowe |
| `03 PvP Heat` | B | **S** dla PvP | PvE może trenować później |
| `10 Damage Mods & Weapon Fitting` | B | **S** | AWU IV/WU V są warte zrobienia przed drogim fitem |

### Hull level

- `94 B` = racial Battleship III. **Wystarczy do pierwszych prób / spokojnego PvE.**
- `94 S` = racial Battleship IV. **To jest zalecane minimum do regularnego latania Battleshipem.**
- `94 I` = racial Battleship V. Bób pod Maraudera/Black Ops, bardzo częste użycie konkretnej rasy albo maksymalizację bonusów.

### Large weapons

W obecnych planach weapon-family końcowy etap to `LARGE T2`.

Dla Battleshipa rozróżniamy:
- **PvE entry:** Large weapon IV + dobre meta/faction weapons może mieć sens przed T2.
- **regularny DPS / PvP:** `LARGE T2` jest właściwym celem.
- Nie odkładaj Battleship IV tylko po to, żeby natychmiast robić cały weapon IMPROVED. Najpierw hull IV + support STANDARD.


## Co polecam trenować

Pomijam Scorpion-like utility oddities. Dla Amarr jako główne DPS/PvE Battleshipy traktuję:

- **Apocalypse** — laser range/tracking, dobry PvE i ranged DPS.
- **Abaddon** — laser DPS + bardzo mocny armor tank/resists.
- Armageddon jest użyteczny, ale jego neutralizer/drone charakter jest bardziej specjalistyczny; nie robię z niego głównej ścieżki tego dokumentu.

---

## Apocalypse — laser / armor

### Pierwsze sensowne wejście PvE

`00 S → 01 B/S → 02 S → 10 I → 22 S → 50 S → 53 do Large Energy Turret IV → 94 Amarr B`

To jest przypadek, gdzie **Battleship III może wystarczyć na start**, jeśli:
- fit jest cap-stable albo poprawnie pulsed,
- masz dobre supporty,
- używasz sensownych meta/faction large lasers.

### Regularny Apocalypse

`00 S → 01 S → 02 S → 03 S → 10 I → 22 S → 50 S → 53 I → 94 Amarr S`

**Wymagane/rekomendowane wyżej niż minimum:**
- `94 S` — Amarr Battleship IV; nie zatrzymuj się na III na stałe.
- `50 S` — supporty turretów IV/V.
- `53 I` — mocny cel do regularnego DPS/PvP.
- `22 S` — dla PvE active armor.
- PvP buffer: zamień `22 S` na `21 S`.

`00 I` nie jest potrzebne, chyba że konkretny fit nie domyka CPU/PG/capa.

---

## Abaddon — laser / armor resist

### Ścieżka

`00 S → 01 S → 02 S → 03 S → 10 I → 21 S lub 22 S → 50 S → 53 I → 94 Amarr S`

Abaddon szczególnie korzysta z hull levelu, bo dostaje bonusy bojowe/tankowe per level.

**Nie polecam regularnego Abaddona na Battleship III.**

- Fleet/buffer: `21 S`.
- PvE/local tank: `22 S`.
- `94 S` — praktyczne minimum.
- `53 I` — docelowy DPS standard.
- `00 S` jest ważniejsze niż na wielu mniejszych hullach, bo Abaddon potrafi mocno cisnąć capacitor.

### Specialist

`94 I` ma sens:
- przed Marauder/Black Ops progression w tej rasie,
- jeśli Amarr BS jest główną platformą pilota,
- gdy każda porcja hull bonusu ma znaczenie w doctrine.

Nie robiłbym `50 I/53 I` przed `94 S`, dobrym tankiem i fitting supportami.

---

## Skrót

| Hull | Hull minimum | Hull zalecany | Tank | Broń |
|---|---|---|---|---|
| Apocalypse PvE entry | `94 B` | **`94 S`** | `22 S` | Large Energy IV na start, potem **`53 I`** |
| Apocalypse PvP | `94 S` | `94 S/I` | `21 S` | **`50 S + 53 I`** |
| Abaddon | `94 S` | `94 S/I` | `21 S` lub `22 S` | **`50 S + 53 I`** |

## Źródła weryfikacyjne

- https://wiki.eveuniversity.org/Battleship
- https://wiki.eveuniversity.org/Amarr_Basic_Ship_and_Skill_Guide
