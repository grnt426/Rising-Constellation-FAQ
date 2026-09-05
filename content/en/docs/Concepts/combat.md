---
title: "Fleet Combat"
date: 2017-01-05
weight: 2
description: >
  How does combat between two fleets get resolved? 
---

### How is combat initiated?
When two [Navarch](/docs/agents/navarch/) agents are in the same system combat can begin in one of three ways:
1. A player clicks on the enemy Navarch while selecting their own, and chooses to fight. this can be queued: a moving or busy navarch can be ordered to attack a navarch in another system, the move is queued first and the attack resolves on arrival. if the target left in the meantime the order is skipped (you get a notification) and the queue moves on
2. A Navarch set to [Interdiction or Fury stance](/docs/agents/navarch/#stance) intercepts enemy fleets arriving in its system. Fury also attacks on its own arrival, whatever the enemy is doing. only idle fleets intercept, a fleet mid-action never breaks off. faction-mates of the intercepting fleet join the same battle
3. A Navarch set to [Defender stance](/docs/agents/navarch/#defender) will begin a fight if the system they are in is under attack (Pillage/Bombard/Conquest/Colonization), or if it arrives on an enemy doing one of those. Defender stance will also allow the navarch to join another navarch of the same faction in combat against the enemy.
### How does Combat get resolved?
Combat occurs in rounds during each round the following phases take place:

#### 1. Deployment
The squadron in the row corresponding to the round number are added to the battlefield.

**Example**: On the first round of combat, the squadron in the L1 column would be deployed, (Drone Carriers in this case)

![Fleet Example 1](/images/fleet_example_1.PNG)

##### Multiple Defending Navarch
If there are more than one defending navarchs in the system, the supporting ones will join in later rounds 3, 6 and 9.... 

**Example**: 3 navarch are defending a system (A,B,C), and an attacker comes in (X). Per round joining the fight:
1. A-L1 and X-L1
2. A-L2 and X-L2
3. A-L3 + B-L1 and X-L3
4. A-L4 + B-L2 and X-L4
5. A-L5 + B-L3 and X-L5
6. A-L6 + B-L4 and X-L6
7. B-L5
8. B-L6
9. C-L1

#### 2. Roll for initiative
The navarchs commanding the fleets roll off, using their  navarch levels as a modifier so that the higher level one will win more often.

#### 3. Attack
Each squadron takes turns making all of its attacks against a random enemy squadron on the battlefield.

**Example**: a squadron of 2 Gunner ships would make 2 explosive attacks, where a squadron of 8 Light Fighters would make 8 * (2 energy attacks + 1 explosive attack) for a total of 24 individual attacks. 

All of the damage from an attack goes to an individual ship, so even if a Gunner attacks and hits a light fighter with 25 health, most of the 390 of its attack is wasted, as it only removes a single ship from the squadron of light fighters. [Ship Stats](/docs/ships/stats/)


### Morale
Each ship has a morale base, increased by the level of the ship.
Ships start at 20 morale, and every level after gets you 0.5% more that also applies to all of the other statistics of the ship
During a fight, if a squadron's morale hits 0, they will flee the combat. 
Morale resets at the end of each combat, so squadron are always back at full morale value before the next fight.

#### What causes morale loss?
Morale is lowered with this events:
- on squadron: when 1 ship of the squadron is destroyed
- on entire fleet: when 1 squadron of the fleet is destroyed 


#### What causes squadrons to no longer respond to orders and flee in combat?
Running out of morale
