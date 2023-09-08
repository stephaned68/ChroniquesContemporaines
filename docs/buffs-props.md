# Fonctions spéciales

La fiche de personnage Chroniques Contemporaines comporte de nombreuses fonctionnalités avancées détaillées ci-dessous.

## Buffs

De nombreuses capacités et traits permettent de donner des bonus (ou debuffs/malus) aux tests et jets de dés.

Certaines concernent les attaques du personnages et doivent être indiquées sur l'onglet _Caractéristiques_ dans les listes _Modificateurs d'attaque_ et _Modificateurs de dommages_.

D'autres concernent les divers caractéristiques et attributs du personnage et doivent être indiqués sur l'onglet _Capacités_ dans la liste _Buffs_.

Dans tous les cas :
- Si le buff est temporaire, une case à cocher permet de l'activer ou le désactiver selon les circonstances.
- Si le buff est permanent, il suffit de laisser la case cochée en permanence.
- Tous les buffs ont la même structure : 
  - le nom de la capacité ou du trait, qui apparaît dans les bulles d'aide associées aux jets dans le chat
  - la ou les attributs bénéficiant du modificateur ainsi que la valeur effective de celui-ci
  - si un buff modifie plusieurs attributs, ceux-ci doivent être indiqués à la suite les uns des autres, séparés entre eux par des points-virgules ';'

Les attributs modifiés peuvent être :
- Les six caractéristiques de base : FOR, DEX, CON, INT, PER, CHA
- L'attaque au contact que l'on peut indiquer via plusieurs alias : atc, atkcac, cac, contact
- L'attaque à distance que l'on peut indiquer via plusieurs alias : atd, atktir, cad, distance, tir
- L'attaque mentale que l'on peut indiquer via plusieurs alias : men, atkmen, mental, mentale
- L'attaque magique que l'on peut indiquer via plusieurs alias : mag, atkmag, magie, magique
- Le Pilotage (setting Bitume) : pil, atkpil, pilotage
- L'Initiative que l'on peut indiquer via plusieurs alias : init, initiative
- La défense : def
- Les points de vie : pv

La valeur du modificateur peut être spécifiée comme :
- Un nombre fixe
- La valeur d'un autre attribut, en l'indiquant entre [ ... ] (ex : [PER])
- Le rang dans une voie, en l'indiquant soit sous la forme [VOIE#] (où # est le numéro de la voie), soit sous la forme [rang {nom voie}]


## Propriétés d'équipement

Pour chaque élément de la liste d'équipement du personnage, il est possible de spécifier diverses propriétés influant sur les attributs.

### Cases à cocher

- La case "Equipement porté" est prise en compte dans la gestion de l'encombrement. De plus, si une propriété 'DEF' apparait dans la liste des propriétés de cet équipement, cocher ou décocher cette case coche ou décoche la case "Armure portée" dans la section DEFENSE de l'onglet _**Caractéristiques**_ de la fiche.

- La case "A une attaque" crée une ligne d'attaque sur l'onglet _**Caractéristiques**_ de la fiche. La ligne d'attaque est créée en fonction des propriétés indiquées pour l'équipement.

### Propriétés d'équipement

Une liste de propriétés peut être fournie pour un équipement, sous la forme d'une liste de paires _nom:valeur_ séparées par des virgules (,). La liste des propriétés supportées est la suivante :

- **DEF** :	Valeur du bonus de DEF de l'armure.
- **DEF-** : Valeur du malus d'armure.
- **RD** : Valeur de réduction des dommages.
- **ATD** : Valeur de portée pour une arme à distance.
  - Si cette proprété est indiquée, la ligne d'attaque utilise l'ATD du personnage, sinon la ligne d'attaque créée utilise l'ATC.
- **DM** : Dés de dommages de arme.
- **DM2** : Dés de dommages de arme si elle inflige plusieurs types de dommages.
