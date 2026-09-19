# WoW Forever — Tanking Class Analysis

> A comprehensive, source-checked analysis of the three tanking classes in **World of Warcraft Forever** based on currently available info from Blizzard, talent calculators, other online sources and experience tanking end game content in vinalla and classic: the **Protection Warrior**, **Protection Paladin**, and **Feral Druid (Bear)** — across threat generation, aggro holding, end‑game raiding, PvP, race choice, talent progression, and professions.

📄 **Main document:** [`WoW_Forever_Tanking_Analysis_Report.md`](./WoW_Forever_Tanking_Analysis_Report.md)

---

## Why this was created

WoW Forever is a new project, and reliable, consolidated theorycraft for tanks is scarce and scattered across forum posts, patch notes, and word‑of‑mouth. This report was written to pull that fragmented knowledge into a **single, internally consistent, honestly‑caveated reference** — one that a prospective tank can actually plan a character around.

It exists because the questions tanks keep asking deserve better than a dozen half‑answers:

- Which tank should I roll, and *why*?
- How does threat actually work here, and how do I hold it?
- What does a correct 1→60 talent progression look like (that adds up to 51 points)?
- Which race, and which two professions, best serve my role?
- **Is tanking even worth it in PvP?**

## What it is

A long‑form technical review covering:

- **Per‑class analysis** — core threat mechanics, resource systems, rotations, and strengths/weaknesses for Warrior, Paladin, and Druid.
- **Comparative analysis** — side‑by‑side threat, survivability, and utility ratings.
- **Threat & aggro mechanics** — how threat is generated and held in PvE.
- **End‑game raid recommendations** — assessed across the three launch raid tiers: **Barrow Deeps (10)**, **Hyjal Summit (20)**, and **Onyxia's Lair (40)**.
- **Level‑by‑level talent progressions** — one point per level from 10→60, with cumulative totals that reconcile to a full **51‑point** build for each class.
- **Race selection guides** — separated for PvE, PvP, and levelling.
- **PvP builds** — reframed around what actually wins fights (see below).
- **Professions** — the two‑primary limit, camping/campfire buffs, and the account‑wide **Legacy** system.

## What it's to be used for

- **Choosing a main.** Compare the three tanks honestly before you commit dozens of hours.
- **Planning a build.** Follow a talent path that is mathematically correct at every level, not a vague end‑state dump.
- **Raid preparation.** Understand what each tank brings to 10‑, 20‑, and 40‑player content.
- **PvP planning.** Build a tank that disrupts, survives, and protects — deliberately, not as an afterthought.
- **A living reference.** As WoW Forever evolves, this is a base to correct and extend rather than start from scratch.

## What I hope readers take away

- **Confidence** that the numbers add up and the recommendations are reasoned, not asserted.
- **Clarity** on the real trade‑offs between the three tanks, so the choice fits *your* goals.
- A recognition that **tanks are a first‑class PvP pick**, not solely a PvE necessity.
- Honesty about the limits of the analysis (see [Verification & honesty](#verification--honesty)) — you should always be able to tell what is *confirmed* from what is *estimated*.

---

## Why tanks are genuinely viable — and needed — in PvP

> **Key mechanic:** In PvP, **threat is not a factor.** Threat and aggro only govern how *NPCs* choose targets; other players pick their own. So a tank's PvP worth has **nothing** to do with threat generation — and everything to do with the traits threat‑tanking is built on top of: **durability, control, and disruption.**

Because tanks stop being "the thing the boss hits" and become **durable disruptors**, they fill a role no damage dealer or healer can. That is exactly why they're wanted on serious PvP teams:

- **Survivability that refuses to die.** High armour, block/dodge/parry, and defensive cooldowns mean a tank soaks focus fire and forces the enemy to commit multiple players (and their cooldowns) to remove one target — a losing trade for them.
- **Peeling and protection.** A tank's core job in group PvP: body‑block, stun, and slow attackers off your healers and carries. Keeping *your* damage alive wins more fights than adding a fourth attacker.
- **Crowd control and disruption.** Stuns, interrupts, fears, roots, and knockbacks (e.g. War Stomp‑style AoE stuns, taunt‑adjacent forced‑attack effects, charge/intercept, Bash) shatter enemy setups and buy your team tempo.
- **Mobility and initiation.** Gap‑closers and shapeshift/mobility tools let tanks start fights on their terms, chase kills, or catch fleeing targets — control that a stationary caster simply doesn't have.
- **Objective dominance.** In battlegrounds, the ideal flag/orb/objective carrier is the hardest target to kill. A tank's durability plus mobility makes it the premier objective runner and node holder.
- **Area denial and zoning.** A tank standing on a choke, doorway, or objective is a wall the enemy must spend resources to move. Presence alone shapes the fight.
- **Utility and resilience to control.** Buffs, off‑heals/self‑sustain, and anti‑CC tools (fear/charm/sleep removal, etc.) keep a tank contributing through the enemy's best disruption.

**Bottom line for PvP:** value a PvP tank by how long it lives, how much it disrupts, and how much friendly damage it keeps alive — never by threat. A good tank doesn't out‑damage the enemy; it makes the enemy's damage *not matter*.

---

## How the report is organised

| Section | What you'll find |
|---|---|
| Executive Summary | The headline verdicts at a glance |
| Class Analyses | Warrior, Paladin, and Druid mechanics in depth |
| Comparative Analysis | Threat / survivability / utility, side by side |
| Threat & Aggro (PvE) | How threat is generated and held |
| End‑Game Raiding | Recommendations for the 10/20/40 tiers |
| Talent Progressions | Correct 1→60 paths totalling 51 points each |
| Race Selection | Separate PvE, PvP, and levelling picks |
| Specialised Endgame Builds | Including PvP builds (threat‑agnostic) |
| Professions & Legacy | Two‑primary limit, camping buffs, account‑wide perks |

## Conventions

- **Language:** British English (en‑gb) throughout — e.g. *armour*, *specialise*, *levelling*, *defence*, *colour*.
- **Talent maths:** 51 points total; 1 point per level from level 10 to 60 (points available = *level − 9*).
- **In‑game ability names** keep their canonical spelling even where that is US‑style (e.g. the Undead *Cannibalize* racial, the Gnome *Engineering Specialization* racial), because that is how the client itself labels them.

## Verification & honesty

This report is written to be **internally consistent and mathematically correct**, and it clearly marks what is **confirmed** versus **estimated or unverified**. WoW Forever is a moving target and some details cannot be independently verified, so treat the following as provisional and expect them to change:

- Exact numeric tuning (ability coefficients, threat multipliers, racial values).
- Precise effects of **Legacy** profession talents and some **camping buffs**.
- Anything explicitly flagged with a ⚠️ caveat in the document.

Corrections and updates are welcome — the aim is a reference that gets *more* accurate over time.

---

*Not affiliated with or endorsed by the WoW Forever project or Blizzard Entertainment. "World of Warcraft" is a trademark of Blizzard Entertainment; used here for identification only.*
