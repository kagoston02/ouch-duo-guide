# #OUCH 
#### *0 to hero step by step duo chimps guide*

---

## Towers:

#### Hero
- Sauda
- (Churchill)

#### Water Towers
- Monkey Sub 2-5-0
- Monkey Sub 2-0-5
- Monkey Buccaneer 5-2-0
- Monkey Buccaneer 2-5-0

#### Support

- Village
- Ice Monkey 0-5-0

#### Other

- ninja


## Defense Timeline 


```mermaid
---
config:
  theme: 'base'
---
gitGraph
    commit id: "R6"
    branch Sauda
    commit id: "cuts shi"

    checkout main
    branch Sub-Commander


    checkout main
    commit id: "R7"
    commit id: "R8"

    checkout Sub-Commander
    commit id: "Twin"

    checkout main
    commit id: "R9"

    branch Sub-Ballistic

    checkout main
    commit id: "R14"

    checkout Sub-Commander
    commit id: "Airburst"

    checkout main
    commit id: "R16"

    checkout Sub-Commander
    commit id: "Advanced"

    checkout main
    commit id: "R18"

    checkout Sub-Ballistic
    commit id: "Longer Range"

    checkout main
    commit id: "R19"

    checkout Sub-Ballistic
    commit id: "Barbed"

    checkout main
    commit id: "R20"

    checkout Sub-Ballistic
    commit id: "Heat"

    checkout main
    commit id: "R22"

    checkout Sub-Ballistic
    commit id: "Advanced Intel"

    checkout main
    commit id: "R26"

    checkout Sub-Commander
    commit id: "Triple"

    checkout main
    commit id: "R27"

    branch ninja

    commit id: "exists"

    checkout main
    commit id: "R28"

    branch buccaneer

    checkout main
    commit id: "R31"

    checkout buccaneer
    commit id: "Hot + Faster"

    checkout main
    commit id: "R32"

    checkout buccaneer
    commit id: "Double"

    checkout main
    commit id: "R34"

    checkout buccaneer
    commit id: "Cannon"

    checkout main
    commit id: "R36"

    checkout Sub-Ballistic
    commit id: "Ballistic MISSILEl"

    checkout main
    commit id: "R39"

    checkout buccaneer
    commit id: "PIRATE!!!" type:HIGHLIGHT

    checkout main
    commit id: "R40 M.O.A.B." type:HIGHLIGHT
    commit id: "R44"

    branch carrier

    checkout main
    commit id: "R46"

    checkout carrier
    commit id: "Destroyer"

    checkout main
    commit id: "R47"

    branch village

    checkout main
    commit id: "R49"

    checkout village
    commit id: "jungle D. + Camo"





```

## Defese Architecture


```mermaid
architecture-beta
    group map[Ouch Defense Architecture]
    
    group ma[Advanced Intel] in map
    group su[Support assets] in map

    service d[Destroyer 5 2 0] in ma
    service command[Sub Commander 2 0 5] in ma
    service bm[Ballistic Missile 2 5 0] in ma
    service p[Pirate 2 5 0] in ma
    service ninja[Ninja] in ma

    service village[Village] in su
    service ice[Ice Monkey] in su

    d:R -- L:command
    command:T <--> B:bm
    command:R -- L:p
    d:R -- L:bm
    bm:R -- L:p
    ninja:L --> R:command

    ice:L --> R:village


    
```