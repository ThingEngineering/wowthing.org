---
title: Legion World Quests
description: >
  Useful world quests for leveling battle pets
weight: 4
---

Addons:

- [Rematch](https://www.curseforge.com/wow/addons/rematch) for a lot of good stuff
- [FixRematch](https://www.curseforge.com/wow/addons/fixrematch) so that Rematch actually works
- [Pet Battle Scripts](https://www.curseforge.com/wow/addons/pet-battle-scripts) to mostly automate repetitive battles

## Dalaran

### Fight Night: Amalia

Ranishu Runt + Voidskimmer
Fight duration: ~1:25
Rare chance of failing, but fast and safe for level 1 pets
This fight rarely requires bandages!

### Fight Night: Bodhi Sunwayver

Servant of Demidos + Mechanical Pandaren Dragonling
Fight duration: ~1:30
Fast, reliable and safe for level 1 pets

### Fight Night: Sir Galveston

Court Scribe + Surger
Fight duration: ~1:05
Fast, reliable and safe for level 1 pets

### Fight Night: Tiffany Nelson

> [!TIP] Ichabod `[ANY]` / Obsidian Warwhelp `[ANY]`
>
> Level 1 safe. Needs bandages. ~55s. 4 battles with Safari Hat.
>
> ```text
> Fight Night: Tiffany Nelson:2VGC:112635G:1223455:ZL:N:-----BEGIN PET BATTLE SCRIPT-----\nchange(#2) [ round=2 ]\nchange(#1) [ self(#3).played ]\nuse(Reaping Hook:2469)\nuse(Flame Breath:501) [ round=3 & enemy(#1).dead ]\nuse(Time Bomb:602)\nuse(Armageddon:1025)\nuse(Claw:429)\nchange(#3)\n-----END PET BATTLE SCRIPT-----
> ```

---

## Azsuna

### Training with the Nightwatchers

Tiny Snowman + Twilight Whelpling P/S
Fight duration: ~1:35
Reliable and safe for level 1 pets

---

## Highmountain

### Snail Fight!

> [!TIP] Leveling Pet / Xu-Fu `[ANY]` / Leveling Pet
>
> Level 1 safe. No bandages but small chance of failing.
>
> ```text
> Snail Fight!:3639:ZL:212417I:ZL:N:-----BEGIN PET BATTLE SCRIPT-----\nquit [ self(#2).dead ]\nstandby [ round=1 ]\nchange(#2) [ !self(#2).active ]\nchange(#3) [ enemy(#1).dead & !self(#3).played ]\nif [ enemy(#3).active ]\n    use(Feed:1016) [ self.aura(Prowl:543).exists ]\n    use(Prowl:536) [ self.hp>723 & self.ability(Feed:1016).duration<2 ]\n    use(Feed:1016)\n    use(Bite:110)\nendif\nuse(Prowl:536)\nuse(Feed:1016) [ self.aura(Prowl:543).duration=1 ]\nuse(Bite:110) [ !self.aura(Prowl:543).exists & enemy.hpp<100 & !enemy(#2).active ]\nuse(Bite:110) [ enemy.ability(Headbutt:376).usable ]\nstandby\n-----END PET BATTLE SCRIPT-----
> ```

### Tiny Poacher, Tiny Animals

Father Winter's Helper + Mechanical Pandaren Dragonling
Fight duration: ~1:30
Fast and safe for level 1 pets, but there is a chance the strategy might fail to enemy crits

### Training with Bredda

Rebuilt Mechanical Spider + Microbot XD
Fight duration: ~1:50
Reliable and safe for level 1 pets

---

## Stormheim

### [Jarrun's Ladder](https://www.wow-petguide.com/Strategy/22340/Jarruns_Ladder)

> [!TIP] Anomalus `[ANY]` / Kunchong Hatchling `[P/P]`
>
> Level 1 safe. Needs bandages. ~1m30s. 4 battles with Safari Hat.
>
> ```text
> Jarrun's Ladder:36VF:12142OQ:ZL:21242CM:N:-----BEGIN PET BATTLE SCRIPT-----\nquit [ !self(#3).exists ]\nchange(next) [ self.dead ]\nchange(#3) [ self(#2).played ]\nchange(#3) [ round=3 ]\nuse(#1) [ round=4 ]\nchange(#1) [ round=6 ]\nstandby [ round=8 & enemy(#3).hp<524 ]\nuse(#3) [ self(#1).active ]\nuse(#3) [ self(#3).active & round>9 ]\nuse(#2)\nuse(#1)\nstandby\n-----END PET BATTLE SCRIPT-----
> ```

### My Beast's Bidding

Gorm Rootstinger P/S + Crimson Spore
Fight duration: ~1:05
Fast, reliable and safe for level 1 pets

---

## Suramar

### Chopped

Kun-Lai Runt P/S or P/B + Direbeak Hatchling
Fight duration: ~1:40
Reliable and safe for level 1 pets

### The Master of Pets

Mechanical Axebeak + Sprite Darter Hatchling
Fight duration: ~1:55
Reliable and safe for level 1 pets

---

## Val'sharah

### Dealing with Satyrs

Shadowbarb Hatchling + Anomalus
Fight duration: ~1:15
Rare chance of failing, but fast and safe for level 1 pets

### Training with Durian

Moon-Touched Netherwhelp + Pocket Cannon
Fight duration: ~1:40
Reliable and safe for level 1 pets
