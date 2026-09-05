---
title: "Navarch"
date: 2017-01-05
weight: 2
description: >
  Agents which can Conquest, Pillage or Attack
---

![Navarch](https://asylamba.com/public/media/files/sources/navarch-tetrarchy.png)
(note some exact values in the image are out of date)

## Classes
| Name | Primary skill |
| --- | --- |
| Strategist | Leadership |
| Butcher | Strike |
| Conquerer | Conquest |
| Shipowner | Production |
| Sentinel | Defense |
| Instructor | Training |

## Abilities
### Pillaging ![Bombing](/images/bombing.PNG)
Allows a navarch to raid resources from an enemy controlled system or dominion. Compares the navarch's total bombing power against the defense of the system. Increased by Conquest skill, and by having certain types of ships in the fleet. see [Ship Stats - Bombing](/docs/ships/stats/#what-are-the-base-stats-of-all-of-the-ships) 
#### Does the time to pillage depend on bombing power?
yes slightly depends on defense and bombing power. The base time length for a pillage is 1h
### How much will I get from pillaging?
One pillage gives 150 ticks of the production of the system for a normal level of success, and 200 ticks for a critical. Each pillage lowers % of resources raided by 45% and it recovers over time by .25% per tick
### Will my fleet take damage from bombing a system?
Yes the fleet will take damage based on the total amount of defense the system has. On a failure, the damage is increased.
### What is the difference between Bombard and Pillage actions?
Both rely upon the bombing power of the fleet, however a bombard will destroy more buildings and kill more people, but without providing resources to the attacker.

### Conquest ![Invasion](/images/invasion.PNG)
Allows a navarch to convert an enemy controlled system or dominion into a system directly under your control. Compares the navarch's total invasion power against the defense of the system. Increased by Conquest skill, and by having certain types of ships in the fleet. see [Ship Stats - Invasion](/docs/ships/stats/#what-are-the-base-stats-of-all-of-the-ships) 
#### Does the time to conquest depend on invasion power?
yes slightly depends on defense and invasion power

#### How much invasion power do I need?
Invasion power is compared to system defense

### Repair ![Repair](/images/repair.PNG)
Repairs the fleet under the navarch's control. The Navarch gives 5 points of repair to the fleet for each skill rank. Increased by the Leadership skill, and by having certain types of ships in the fleet. see [Ship Stats - Repair](/docs/ships/stats/#what-are-the-base-stats-of-all-of-the-ships) 

#### How long do repairs take?
Repairs will only happen while a fleet is not moving or engaging in an offensive action. Ships will be repaired starting with the ship at lowest % health first. The rate of repair is:

**Repair Score * .5 HP per tick.**

**Example**: A navarch with 2 ranks of repair, and has a drone carrier x2 in their fleet will have 
(2 ranks * 5) + (4 score from fleet) = 12 repair score. Repairing 6 HP per tick. So in legacy with 3 minute ticks you can estimate it at 120 HP per hour.


## Stance
your stance decides when the fleet starts fights on its own. faction-mates are never targeted. the in-game Help panel (Navarch stances) has the full matrix

### Defender
engages enemy navarchs doing something hostile in its system (pillage, bombard, conquest, colonization, dominion takeover). also engages them on arrival: a Defender fleet jumping into a system where an enemy is mid-pillage attacks it. idle enemies are left alone, so two Defender fleets from different factions can share a system. joins any fight a faction-mate gets into here

### Deserter
never starts a fight. when caught arriving on a hostile picket it rolls to escape (50%) instead of fighting

### Prudent
will only fight if directly attacked. never joins in for a faction-mate

### Interdiction
(was "Aggressive") intercepts any enemy navarch arriving at its system, whatever they intend. does not start fights when it is itself the arriving fleet, but an enemy Interdiction fleet already sitting there will intercept it. two Interdiction fleets only leave each other alone once they already share a system

### Fury
engages any enemy navarch in the same system: when one arrives, when one starts a hostile action, and when the Fury fleet itself arrives. busy or idle, whatever their stance

### Can a busy fleet be attacked?
yes. a fleet mid pillage/bombard/conquest/colonization never breaks off to intercept, but an arriving Fury or Defender fleet engages it anyway, and it gets pulled into any fight its faction-mates have in that system. fleets in transit can't be engaged

### Which fleet gets engaged first?
most hostile stance first: Fury, then Interdiction, Defender, Prudent, Deserter. ties are random. faction-mates of the first target join that same battle, so a Fury screen parked in front of a conquesting fleet takes the hit and the conquest fleet joins it. one battle, not two

## What happens if you recall a Navarch with a fleet?
recalling them will destroy the fleet
