---
title: "Navarch"
date: 2017-01-05
weight: 2
description: >
  Des agents qui peuvent conquérir, piller ou attaquer.
---
## Capacités
### Pillage ![Bombardement](/images/bombing.PNG)
Permet à un navarque de piller les ressources d'un système ou d'un dominion contrôlé par l'ennemi. Compare la puissance totale de bombardement du navarque à la défense du système. Augmentée par la compétence Conquête, et par la présence de certains types de vaisseaux dans la flotte. voir [Ship Stats - Bombing](/docs/ships/stats/#what-are-the-base-stats-of-all-of-the-ships) 
#### Le temps de pillage dépend-il de la puissance de bombardement ?
Oui, cela dépend légèrement de la puissance de défense et de bombardement. Le temps de base pour un pillage est de 1h.
### Combien vais-je gagner en pillant ?
Un pillage donne 150 ticks de la production du système pour un niveau de succès normal, et 200 ticks pour un critique. Chaque pillage diminue le % de ressources pillées de 45% et se récupère au fil du temps de 0,25% par tic. 

### Conquête ![Invasion](/images/invasion.PNG)
Permet à un navarque de convertir un système ou un dominion contrôlé par l'ennemi en un système directement sous son contrôle. Compare la puissance totale d'invasion du navarque à la défense du système. Augmenté par la compétence Conquête, et par la présence de certains types de vaisseaux dans la flotte. voir [Ship Stats - Invasion](/docs/ships/stats/#what-are-the-base-stats-of-all-of-the-ships) 
#### Le temps de conquête dépend-il de la puissance d'invasion ?
oui, cela dépend légèrement de la défense et de la puissance d'invasion

#### De quelle puissance d'invasion ai-je besoin ?
La puissance d'invasion est comparée à la défense du système

### Réparation ![Repair](/images/repair.PNG)
Répare la flotte sous le contrôle du navarche. Augmenté par la compétence Leadership et par la présence de certains types de vaisseaux dans la flotte. voir [Ship Stats - Repair](/docs/ships/stats/#what-are-the-base-stats-of-all-of-the-ships) 

#### Combien de temps prennent les réparations ?
Les réparations ne sont effectuées que lorsqu'une flotte ne se déplace pas ou ne participe pas à une action offensive. Les navires sont réparés en commençant par le navire dont le pourcentage de santé est le plus bas. Le taux de réparation est le suivant :

**Score de réparation * 0,5 HP par tic**.

**Exemple** : Un navarque avec 2 rangs de réparation, et qui a un transporteur de drones x2 dans sa flotte aura 
(2 rangs * 4) + (4 points de la flotte) = 12 points de réparation. Réparant 6 HP par tic. Donc, dans l'héritage avec des ticks de 3 minutes, vous pouvez l'estimer à 120 HP par heure.


## Stance
la posture décide quand la flotte engage le combat d'elle-même. les alliés de faction ne sont jamais visés. le panneau d'aide en jeu (Postures de Navarque) donne la matrice complète

### Défenseur
engage les navarques ennemis qui font quelque chose d'hostile dans son système (pillage, bombardement, conquête, colonisation, prise de dominion). les engage aussi à l'arrivée : une flotte Défenseur qui saute dans un système où un ennemi est en plein pillage l'attaque. les ennemis au repos sont laissés tranquilles, deux flottes Défenseur de factions différentes peuvent donc partager un système. rejoint tout combat d'un allié de faction ici

### Déserteur
n'engage jamais le combat. surpris à l'arrivée par un piquet hostile, il tente de s'échapper (50%) au lieu de combattre

### Prudent
ne se bat que s'il est directement attaqué. n'intervient jamais pour un allié de faction

### Interdiction
(anciennement « Agressif ») intercepte tout navarque ennemi qui arrive dans son système, quelle que soit son intention. n'engage pas le combat quand c'est lui la flotte qui arrive, mais une flotte Interdiction ennemie déjà postée là l'interceptera. deux flottes Interdiction ne se laissent tranquilles qu'une fois qu'elles partagent déjà un système

### Furie
engage tout navarque ennemi dans le même système : quand un ennemi arrive, quand il lance une action hostile, et quand la flotte Furie arrive elle-même. occupé ou au repos, quelle que soit sa posture

### Une flotte occupée peut-elle être attaquée ?
oui. une flotte en plein pillage/bombardement/conquête/colonisation n'interrompt jamais son action pour intercepter, mais une flotte Furie ou Défenseur qui arrive l'engage quand même, et elle est entraînée dans tout combat que ses alliés de faction livrent dans ce système. les flottes en transit ne peuvent pas être engagées

### Quelle flotte est engagée en premier ?
la posture la plus hostile d'abord : Furie, puis Interdiction, Défenseur, Prudent, Déserteur. égalité = aléatoire. les alliés de faction de la première cible rejoignent cette même bataille, donc un écran Furie posté devant une flotte en conquête encaisse le coup et la flotte de conquête le rejoint. une seule bataille, pas deux

### Que se passe-t-il si vous rappelez un Navarque avec une flotte ?
Le rappeler détruira la flotte.

