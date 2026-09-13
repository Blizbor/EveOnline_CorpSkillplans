# MINMATAR — Battleship training recommendations

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

Minmatar ma trzy sensowne T1 Battleship paths:

- **Maelstrom** — projectile + active shield; bardzo naturalny PvE/artillery BS.
- **Tempest** — projectile, elastyczny shield/armor.
- **Typhoon** — missiles + drones, elastyczny damage selection.

---

## Maelstrom — projectile / active shield

### Entry PvE

`00 S → 01 S → 02 S → 10 I → 30 S → 31 S → 50 S → 52 do Large Projectile Turret IV → 94 Minmatar B`

### Regularny Maelstrom

`00 S → 01 S → 02 S → 03 S → 10 I → 30 S → 31 S → 50 S → 52 I → 94 Minmatar S`

Maelstrom ma bonus do shield boostera, więc:

- **`31 S` jest ważny**, nie ozdobny.
- `30 S` pełna baza shield.
- `94 S` Battleship IV.
- `52 I` docelowo dla arty/AC.
- przy artillery szczególnie ważne są dobre common turret supporty (`50 S`).

---

## Tempest — projectile / elastyczny tank

`00 S → 01 S → 02 S → 03 S → 10 I → 50 S → 52 I → 94 Minmatar S`

Tank wybierz według konkretnego fita:

- shield: `30 S`;
- armor: `21 S`;
- active shield: `30 S + 31 S`;
- active armor: `22 S`.

Nie trenuj obu tanków tylko dlatego, że Tempest może oba.

### Entry

`94 B + Large Projectile IV` jest akceptowalne do pierwszych prób.

### Regularnie

**`94 S + 50 S + 52 I`**.

Tempest jest jednym z hullów, gdzie pilot z dobrymi supportami i właściwym fitem zyskuje więcej niż pilot z przypadkowymi V.

---

## Typhoon — missiles + drones

### Entry

`00 S → 01 S → 02 S → 10 I → wybrany tank S → 60 S → 63 do Cruise/Torp IV → 70 B/S → 94 Minmatar B`

### Regularny Typhoon

`00 S → 01 S → 02 S → 03 S → 10 I → wybrany tank S → 60 S → 63 S → 70 S → 94 Minmatar S`

Drony:
`71 S + 72 S`
są dobrym dodatkiem.

`73` rób tylko wtedy, gdy konkretny fit naprawdę opiera się mocniej na heavy/sentry; Typhoon nie powinien opóźniać T2 large missiles dla pełnej dronowej ścieżki.

Tank:
- PvE shield: `30 S + 31 S`;
- armor: `21/22 S` zależnie od fita.

**Nie trenuj projectile tylko dlatego, że Typhoon jest Minmatarem.**
To missile Battleship path.

---

## Skrót

| Hull | Hull minimum | Hull zalecany | Tank | Broń |
|---|---|---|---|---|
| Maelstrom | `94 B` | **`94 S`** | **`30 S + 31 S`** | Large Projectile IV → **`52 I`** |
| Tempest | `94 B` | **`94 S`** | wybrany `21/22/30/31` | **`50 S + 52 I`** |
| Typhoon | `94 B` | **`94 S`** | wg fita | **`60 S + 63 S`**, drony support |

## Źródła weryfikacyjne

- https://wiki.eveuniversity.org/Battleship
- https://wiki.eveuniversity.org/Maelstrom
- https://wiki.eveuniversity.org/Minmatar_Basic_Ship_and_Skill_Overview
