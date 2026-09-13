# EVE Corp Skillplans

Modularna biblioteka **89 corp skillplanów** przygotowana do publikacji na GitHub.

## Poziomy

Każdy plan ma dokładnie trzy poziomy:

- **BASIC** — wejście w rolę / najniższy rozsądny próg,
- **STANDARD** — poziom zalecany do regularnego używania,
- **IMPROVED** — dalsze rozwinięcie bez bezmyślnego trenowania wszystkich supportów na V.

W każdym katalogu planu znajdują się:

- `README.md` — opis planu,
- `BASIC.txt` — czysta kolejka do importu,
- `STANDARD.txt`,
- `IMPROVED.txt`.

## Filozofia level V

`IMPROVED` **nie oznacza „all V”**.

Level V pozostaje w planie tylko wtedy, gdy:
- jest prerequisite do modułu/hulla/skilla, który dany plan obiecuje,
- jest wymagany przez dalszą progresję,
- albo jest świadomym wyjątkiem roli, np. Logistics.

Pozostałe V gracz wybiera sam. Szczegóły:
[`NIGDY_NA_LEVEL_5.md`](NIGDY_NA_LEVEL_5.md).

## Struktura

- `00–03` — core/support
- `10` — weapon fitting/damage mods
- `21–22` — armor
- `30–31` — shield
- `50–53` — turrets
- `60–63` — missiles
- `70–73` — drones
- `80` — Scout
- `83` — Cyno
- `90–99` — hull progression

Pełny spis: [`INDEX.md`](INDEX.md).

## Strategie treningu

Do repo dołączone są wcześniej opracowane rekomendacje ścieżek:

- [`strategies/T1_TO_HAC`](strategies/T1_TO_HAC) — cztery rasy, T1 Frigate → Destroyer → Cruiser → HAC,
- [`strategies/BATTLESHIPS`](strategies/BATTLESHIPS) — cztery rasy, praktyczne DPS/PvE Battleships,
- [`strategies/LOGISTICS`](strategies/LOGISTICS) — cztery rasy, logi frigate / destroyer-gang support / cruiser.

## Import do EVE

Pliki `.txt` są kumulacyjne i mają format:

```text
Navigation I
Navigation II
Navigation III
Navigation IV
```

Skopiuj cały wybrany plik (`BASIC`, `STANDARD` albo `IMPROVED`) i użyj w edytorze planu opcji importu skilli ze schowka.

## Uwaga

Skill requirements w EVE mogą być zmieniane przez CCP. Długie ścieżki T2/capital warto przed rozpoczęciem sprawdzić również w aktualnym kliencie.


## Dodatkowe dokumenty

- [`docs/T2_MODULE_UNLOCKS.md`](docs/T2_MODULE_UNLOCKS.md) — praktyczna ściąga z progów skillowych odblokowujących ważne moduły T2,
- [`strategies/SCENARIOS`](strategies/SCENARIOS) — praktyczne scenariusze rozwoju, obecnie z dodanym scenariuszem do Gili,
- [`diagrams`](diagrams) — diagramy progresji dla broni, tanków i scenariuszy.

## Korekta filozofii planu 00

Po aktualizacji:
- `CPU Management V`
- `Power Grid Management V`
- `Capacitor Management V`
- `Capacitor Systems Operation V`

trafiają do `00 IMPROVED`, bo są zbyt praktyczne, żeby traktować je jako „opcjonalny luksus”.
