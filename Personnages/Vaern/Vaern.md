---
Type: Player
Art: "![[Character Image Placholder]]"
Niveau: 9
Armure: 10
Resistances:
  - NONE
PV: 30
PV_temporaire: 0
Dégats_reçus: 0
DV: 3d6
DV_total: 3
DV_utilisé: 0
Vitesse: 9
FOR: 10
DEXT: 11
CONS: 11
INT: 20
SAG: 13
CHA: 14
savFOR: false
savDEXT: false
savCONS: false
savINT: true
savSAG: true
savCHA: false
Race:
  - Changelin
  - Fée
  - Mort Vivant
Alignement: Chaotique Mauvais
Sexe: Masculin
Age: "40"
Localisation: NONE
Classe:
  - Magicien
Sous_Classe: Nécromencien
Niveau_Classe:
  - "9"
Historique: Artisan Alchimiste
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
  - Changelin
  - Commun
  - Féérique
  - Céleste
Cuivre: 95
Argent: 0
Electrum: 0
Or: 74
Platine: 0
Maitrise: 4
Acrobatie: false
Arcanes: true
Athlétisme: false
Discretion: false
Dressage: false
Escamotage: false
Histoire: false
Intimidation: false
Intuition: false
Investigation: false
Médecine: true
Nature: false
Perception: false
Perspicacité: true
Persuasion: true
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

### Magicien
#### Restauration magique :
Récupère pendant un repos court récupère niveau du mage / 2 en sorts.
#### Tradition arcanique, École de la Nécromancie :
- Nécromancien érudit : Consomme moins de temps et d'or pour recopier les sorts lié.
- Sinistre Moisson : récupère le double de PV du niveau du sort (x3 si sort nécromancien) en tuant une créature ayant une âme.
#### Adepte élémentaire (feu):
ignore résistance feu et tout les 1 sont des 2

### Changelin
- Métamorphe
- Faveur des Fée (pris)

### Invocation : 
- Démon des Ombres

### Alchimie (Recette):
- potion de soin mineur, 1d4+4, prépa 1h, prix 7po
- poison paralysant, 20 po et 2h de travail (si un mec l'ingère ou la reçois dans les yeux il est paralyser pendant 1h)

### Nécromancie :
- golem de chaire (nécessite couture)
- Animation des morts : Humanoïdes et Rongeurs
### Maitrises
#### Armes : 
- dague
- bâton
- fronde
- arbalète légère
- fléchette
#### Armure 
- NONE
#### Outils : 
- Alchimie
#### Autres maitrises
- Télépathie avec Severus (pseudo-dragon)
- Télépathie avec Démon des Ombres
## Grimoire

| Informations                  |             |
| ----------------------------- | ----------- |
| caractéristique d'incantation | Intéligence |
| sorts à préparer chaque jour  | NONE        |
| DD de sauvegardes des sorts   | 16          |
| Bonus d'attaque avec un sort  | 8           |
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
- Paquetage d'Explorateur (25 rations, sac de couchage, gamelle, boite à amadou, 10 torches, 10j ration, une outre, 15m de corde)
- Grimoire (50 sorts/recette)
- Montre à Gousset (lore)
- Matériel d'Alchimiste, lettre d'introduction de guilde d'alchimiste, tenu de voyage
- Carte de visite du "mage" Greed le Nain
- Traité sur la communication avec les morts + voyage dimensionnel (bannissent), livre de remèdes.

# Histoire
Changelin à l'apparence véreuse et usé par le temps, il passe inaperçu, courbé sur son bâton, dans les basfonds des villes avec sa cape noire délavé et usé jusqu'à la toile.

C'est un alchimiste peu scrupuleux quand au contenu de ses potion, il n''hésitera pas à sacrifié une personne plus utile morte que vivante à son projet (et à sa personne). Vaern est à la poursuite d'un but connu de lui seul, il semble lié au médaillon qu'il regarde régulièrement.

Généalogie : parents inconnus, frères et sœurs potentiels : 2 ou plus, descendance non avéré mais hautement supposé au vu de ses fréquentation dûment monnayé (peut être bien la seule chose qu'il paye de bon cœur et sans marchandage).

## Autres informations

- Echoppe d'alchimie dans les bas quartier de Padiver (10po/mois)
- Médecin légiste pour la police de Padiver