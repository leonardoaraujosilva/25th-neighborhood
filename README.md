# 🏙️ 25th Neighborhood

[![Play Now](https://img.shields.io/badge/PLAY%20NOW-Click%20Here%20to%20Play-4CAF50?style=for-the-badge&logo=gamepad&logoColor=white)](https://leonardoaraujosilva.github.io/25th-neighborhood/)

> **Start playing this Web Prototype in your browser right now!**  
> *No installations required. Designed for PC, laptops, tablets, or smartphones.*

---

## 🎮 GAME OVERVIEW

**25th Neighborhood** is a tactical, asymmetrical stealth-survival board game powered by a web application. One player takes on the role of a mutating **Monster**, stalking secretly through the shadows of a quarantined suburban district, while the other players form a squad of **Hunters** trying to track, reveal, and destroy the beast before it evolves.

---

## 📱 WHAT IS A "PASS-AND-PLAY" (HOTSEAT) GAME?

**25th Neighborhood** uses a local multiplayer system known as **Pass-and-Play** (or *Hotseat*). 

This means **you only need a single device** (laptop, PC, or phone) to play with your entire group! 
* Players take turns using the same screen.
* When your turn ends, the app locks the interface behind a **Pass Screen**.
* You pass the device to the next player, ensuring the Monster's secret movements and hands of cards remain completely private without revealing hidden information.

---

## 🎲 GAME COMPONENTS
* **Digital Board / Web App (HTML5):** Manages the 5x5 map, card decks, combat dice, line of sight/stealth, and the secret log.
* **Hunters (3 Players):** Start at the Street Access (Outer Area).
* **The Monster (1 Player):** Starts hidden inside one of the houses.

---

## 🗺️ THE MAP (5x5 GRID)

The neighborhood consists of **25 Houses** (numbered 1 to 25) arranged in a 5x5 grid, plus the **Street Access (Rescue Area)**.

* **3 Infested Houses (Nests):** Feeding locations for the Monster.
* **4 Manholes (Sewers):** Allow the Monster to teleport from one sewer to any other sewer on the map.
* **8 Supply Depots (📦):** Contain 2 supply crates each.
* **10 Regular Houses:** Open ground.
* **Street Access (Gate):** The only entry and exit point of the neighborhood. Connects **exclusively to House 23** (center of the bottom row).

---

## ⚙️ PHASE 0: SETUP (MONSTER HIDE OUT)

1. The game starts **locked** in the Monster's preparation phase.
2. The Monster player must click a house on the map (highlighted in **Green**) to choose their starting Den.
3. **Spawn Restrictions:** The Monster **cannot** spawn on the Street, House 23 (Gate), or inside/adjacent to any Nest.
4. Once the Den is selected, the official hunt begins starting on Hunter 1's turn.

---

## 👣 STEALTH & TRACKING MECHANICS

### Monster Visibility
The Monster plays **completely invisible** on the map (even if a Hunter enters the same house). The Monster is only revealed temporarily if:
* It reaches the **Alpha Stage** (permanently visible).
* It performs an **Attack** or plays the **Pure Fury** card (visible for 2 turns).
* It steps into a **Bear Trap** (visible for 2 turns).
* It is struck by a blind shot or revealed by a **Flare** card (visible for 2 turns).

### The Comet Tail (Blood Trails)
Whenever the Monster moves from one house to another:
1. It leaves **3 Blood Cubes (🔴 3)** in the house it just left.
2. All previous blood trails on the map decay by 1 cube (3 $\rightarrow$ 2 $\rightarrow$ 1 $\rightarrow$ Gone).

---

## 🔄 TURN STRUCTURE

Turns follow an interleaved order: **Hunter 1 $\rightarrow$ Monster $\rightarrow$ Hunter 2 $\rightarrow$ Monster $\rightarrow$ Hunter 3 $\rightarrow$ Monster**.

### Hunters' Turn (2 Actions)
Each Hunter receives **2 Actions** per turn, choosing from:
* **Move (1 Action):** Move to an orthogonally adjacent house (highlighted in **Green**).
* **Search Items (1 Action):** Consume 1 crate in a Supply house (📦) to draw 1 card from the Hunters' deck (max 4 cards in hand).
* **Attack (1 Action):** Spend 1 Ammo to fire their weapon (see Combat section).
* **Play Cards:** *Free* effect cards cost no actions.

### Monster's Turn (1 Reactive Action)
After each Hunter's turn, the Monster gets **1 Reactive Action**, choosing to:
* **Move Hidden (1 Action):** Move to an adjacent house or via Sewer (leaves 3 blood cubes on exit).
* **Consume Nest (1 Action):** Devour biomass at a Nest house, heal +3 HP, and advance 1 Evolution step.
* **Attack (1 Action):** Strike all Hunters in the current house and reveal its position.
* **Instinct (Cards):** Draw 1 card at the start of each round (max 3 in hand).

---

## 🎯 COMBAT & TARGETING SYSTEM

Combat uses detailed dice rolls. Rolls of **4, 5, or 6** count as **Hits [✓]** and deal direct damage.

| Attacker | Weapon / Ability | Dice Rolled | Range | Cost |
| :--- | :--- | :---: | :---: | :---: |
| **Hunter** | Handgun (Basic Attack) | **4 D6** (4+ hits) | Same house or Orthogonal (1 House) | 1 Ammo |
| **Hunter** | Shotgun (Card) | **5 D6** (4+ hits) | Same house only | 1 Ammo |
| **Monster** | Claws (Stage 1) | **2 D6** (5+ hits) | Same house only | Free |
| **Monster** | Alpha Fury (Stage 3) | **3 D6** (4+ hits) | Same house only | Free |

### How Targeting Works in the App:
* **If the Monster is Visible & in Range:** Clicking "Attack" automatically locks onto the beast and resolves the shot.
* **If the Monster is Hidden:** The game enters **Targeting Mode** and highlights valid houses in **Purple**. You must click a house to fire blindly into the dark.

---

## 🃏 CARD DECKS

### Hunters
* **MRE Ration:** Free/1 Action. Heals **+3 HP** instantly.
* **Ammo Crate:** Free/1 Action. Grants **+3 Ammo** to your character.
* **Flare:** 1 Action. Reveals the Monster for **2 turns** if it is in your house or an adjacent house.
* **Bear Trap:** Free/1 Action. Set a trap in the current house *(Forbidden in Nests and Street)*. Deals 2 damage and **reveals** the Monster if it enters.
* **Shotgun:** 1 Action + 1 Ammo. Fires **5 attack dice** in the same house.

### The Monster
* **Regeneration:** 1 Action. Heals **+3 HP** while remaining hidden.
* **Pure Fury:** Free Effect. Attacks instantly with **2 D6** without spending an action, but becomes **Visible**.
* **Misdirection:** Free Effect. Grants 1 free extra movement to escape traps or ambushes.

---

## 🏆 ALPHA EVOLUTION & VICTORY CONDITIONS

* **Alpha Evolution:** Devouring all **3 Nests** evolves the Monster into the Alpha Stage. It gains **+8 HP**, its attacks upgrade to **3 D6 (4+ hits)**, and it becomes **permanently visible**.
* **Hunters' Victory:** Reduce the Monster's HP to **0**.
* **Monster's Victory:** Eliminate all Hunters in the neighborhood.