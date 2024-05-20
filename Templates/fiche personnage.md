---
Type: Player
Art: "![[Character Image Placholder]]"
Niveau: 0
Armure: 0
Resistances:
  - NONE
PV: 0
PV_temporaire: 0
Dégats_reçus: 0
DV: 0d0
DV_total: 0
DV_utilisé: 0
Vitesse: 0
FOR: 0
DEXT: 0
CONS: 0
INT: 0
SAG: 0
CHA: 0
savFOR: false
savDEXT: false
savCONS: false
savINT: false
savSAG: false
savCHA: false
Race:
  - RaceName
Alignement: NONE
Sexe: GenderName
Age: "0"
Localisation: NONE
Classe:
  - ClassName
Sous_Classe: SubClassName
Niveau_Classe:
  - Classe_0
Historique: NONE
Groupe_Associé: NONE
Aime: NONE
Aime-pas: NONE
PersonalityTrait:
  - NONE
SocialTrait:
  - NONE
MentalTrait:
  - NONE
Proficiencies:
  - NONE
Langues:
  - NONE
Cuivre: 0
Argent: 0
Electrum: 0
Or: 0
Platine: 0
Maitrise: 0
Acrobatie: false
Arcanes: false
Athlétisme: false
Discretion: false
Dressage: false
Escamotage: false
Histoire: false
Intimidation: false
Intuition: false
Investigation: false
Médecine: false
Nature: false
Perception: false
Perspicacité: false
Persuasion: false
Religion: false
Représentation: false
Survie: false
Tromperie: false
---
# `=this.file.name` | niveau `=this.niveau`
````col
```col-md 
## Informations
![[image personnage placeholder.png]]

|     Vitesse     | Classe d'Armure |     Résistances     |                    Points de vie                    |         Dés vie : `=this.DV`          |
| :-------------: | :-------------: | :-----------------: | :-------------------------------------------------: | :-----------------------------------: |
| `=this.vitesse` | `=this.armure`  | `=this.Resistances` | `=this.PV + this.PV_temporaire - this.Dégats_reçus` | `=this.DV_utilisé` / `=this.DV_total` |


| `=this.classe` | `=this.Niveau_Classe` |
| -------------- | --------------------- |
| Race           | `=this.Race`          |
| Alignement     | `=this.Alignement`    |
| Historique     | `=this.Historique`    |
| Langues        | `=this.Langues`       |
| Age            | `=this.Age`           |
| Sexe           | `=this.Sexe`          |

``` 
```col-md 
## Caractéristique

| type         | valeur       | bonus                | sauvegarde      | valeur sauvegarde    |
| ------------ | ------------ | -------------------- | --------------- | -------------------- |
| Force        | `=this.FOR`  | `=(this.FOR -10)/2`  | `=this.savFOR`  | `=(this.FOR -10)/2`  |
| Dextérité    | `=this.DEXT` | `=(this.DEXT -10)/2` | `=this.savDEXT` | `=(this.DEXT -10)/2` |
| Constitution | `=this.CONS` | `=(this.CONS -10)/2` | `=this.savCONS` | `=(this.CONS -10)/2` |
| Intelligence | `=this.INT`  | `=(this.INT -10)/2`  | `=this.savINT`  | `=(this.INT -10)/2`  |
| Sagesse      | `=this.SAG`  | `=(this.SAG -10)/2`  | `=this.savSAG`  | `=(this.SAG -10)/2`  |
| Charisme     | `=this.CHA`  | `=(this.CHA -10)/2`  | `=this.savCHA`  | `=(this.CHA -10)/2`  |

## Compétences
| Compétences         |                        | Bonus                                |
| ------------------- | ---------------------- | ------------------------------------ |
| Acrobaties (Dext)   | `=this.Acrobatie`      | `=this.Maitrise + (this.DEXT -10)/2` |
| Arcanes (Int)       | `=this.Arcanes`        | `=this.Maitrise + (this.INT -10)/2`  |
| Athlétisme (For)    | `=this.Athlétisme`     | `=this.Maitrise + (this.FOR -10)/2`  |
| Discretion (Dex)    | `=this.Discretion`     | `=this.Maitrise + (this.DEXT -10)/2` |
| Dressage (Sag)      | `=this.Dressage`       | `=this.Maitrise + (this.SAG -10)/2`  |
| Escamotage (Dex)    | `=this.Escamotage`     | `=this.Maitrise + (this.DEXT -10)/2` |
| Histoire (Int)      | `=this.Histoire`       | `=this.Maitrise + (this.INT -10)/2`  |
| Intimidation (Cha)  | `=this.Intimidation`   | `=this.Maitrise + (this.CHA -10)/2`  |
| Intuition (Sag)     | `=this.Intuition`      | `=this.Maitrise + (this.SAG -10)/2`  |
| Investigation (Int) | `=this.Investigation`  | `=this.Maitrise + (this.INT -10)/2`  |
| Médecine (Sag)      | `=this.Médecine`       | `=this.Maitrise + (this.SAG -10)/2`  |
| Nature (Int)        | `=this.Nature`         | `=this.Maitrise + (this.INT -10)/2`  |
| Perception (Sag)    | `=this.Perception`     | `=this.Maitrise + (this.SAG -10)/2`  |
| Perspicacité (Sag)  | `=this.Perspicacité`   | `=this.Maitrise + (this.SAG -10)/2`  |
| Persuasion (Cha)    | `=this.Persuasion`     | `=this.Maitrise + (this.CHA -10)/2`  |
| Religion (Int)      | `=this.Religion`       | `=this.Maitrise + (this.INT -10)/2`  |
| Repésentation (Cha) | `=this.Représentation` | `=this.Maitrise + (this.CHA -10)/2`  |
| Survie (Sag)        | `=this.Survie`         | `=this.Maitrise + (this.SAG -10)/2`  |
| Tromperie (Cha)     | `=this.Tromperie`      | `=this.Maitrise + (this.CHA -10)/2`  |

``` 
````
## Capacités, traits et maitrises


## Grimoire

| Informations                  |     |
| ----------------------------- | --- |
| caractéristique d'incantation |     |
| sorts à préparer chaque jour  |     |
| DD de sauvegardes des sorts   |     |
| Bonus d'attaque avec un sort  |     |
### Sorts Mineurs

- nom_du_sort
### Sorts tier 1 : 0/0

- [ ] nom_du_sort
### Sorts tier 2 : 0/0

### Sorts tier 3 : 0/0

### Sorts tier 4 : 0/0

### Sorts tier 5 : 0/0

### Sorts tier 6 : 0/0

### Sorts tier 7 : 0/0

### Sorts tier 8 : 0/0

### Sorts tier 9 : 0/0

## Inventaire

| Monnaie          |                  |
| ---------------- | ---------------- |
| Pièce de cuivre  | `=this.cuivre`   |
| Pièce d'argent   | `=this.argent`   |
| Pièce d'électrum | `=this.Electrum` |
| Pièce d'or       | `=this.or`       |
| Pièce de platine | `=this.Platine`  |
### Armes
### Equipement
### Autres
## Histoire
