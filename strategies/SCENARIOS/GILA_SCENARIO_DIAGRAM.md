# GILA_SCENARIO_DIAGRAM.md

Oddzielny diagram progresji dla scenariusza Gila.

## Diagram główny

```mermaid
flowchart TD
    A[00 CORE - Engineering, Capacitor & Rigging<br/>IMPROVED]
    B[01 CORE - Navigation<br/>STANDARD]
    C[02 CORE - Targeting<br/>STANDARD]
    D[03 CORE - PvP Heat<br/>STANDARD]
    E[10 COMBAT - Damage Mods & Weapon Fitting<br/>IMPROVED]

    A --> B --> C --> D --> E

    E --> S1[30 TANK - Shield Passive/Buffer<br/>STANDARD]
    S1 --> S2[31 TANK - Shield Active<br/>STANDARD]

    E --> M0[60 WEAPON - Missile Support<br/>STANDARD]
    M0 --> M1[61 MISSILE - Rockets & Light<br/>STANDARD]
    M0 --> M2[62 MISSILE - HAM & Heavy<br/>STANDARD]

    E --> D0[70 WEAPON - Drone Support<br/>STANDARD]
    D0 --> D1[71 DRONES - Light T2<br/>STANDARD]
    D0 --> D2[72 DRONES - Medium T2<br/>STANDARD]

    E --> C1[92 HULL - Cruiser - Caldari<br/>STANDARD]
    E --> G1[92 HULL - Cruiser - Gallente<br/>STANDARD]

    C1 --> GILA[GILA]
    G1 --> GILA
    S1 --> GILA
    M1 --> GILA
    M2 --> GILA
    D2 --> GILA
```

## Opcjonalne odnogi po drodze

```mermaid
flowchart LR
    A[Missile + Shield foundation] --> H[Hawk<br/>opcjonalnie]
    A --> S[Sunesis<br/>opcjonalnie]
    A --> C[Caracal<br/>najpraktyczniejszy przystanek]
    C --> G[Gila]
    H --> G
    S --> G
```

## Interpretacja

- **Caracal** to najpraktyczniejszy „formalny” przystanek.
- **Hawk** to ścieżka poboczna dla kogoś, kto chce również bardzo dobry mały missile hull.
- **Sunesis** to wygodny utility side-step, ale nie requirement.
- Prawdziwe serce Gili to:
  - `00 IMPROVED`
  - `30 STANDARD`
  - `60 STANDARD`
  - `70 STANDARD`
  - `72 STANDARD`
  - `92 Caldari STANDARD`
  - `92 Gallente STANDARD`
