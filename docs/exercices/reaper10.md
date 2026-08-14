# REAPER
![](https://www.reaper.fm/v7img/ss_persp_v7.jpg){data-zoom-image}<small>Source: reaper.fm</small>

# Exportation dans Reaper

L’exportation (Render dans Reaper) est l’étape finale de production. Elle consiste à transformer votre projet multipiste en un fichier audio unique **(WAV, MP3, FLAC, etc.)** pouvant être partagé, diffusé ou remis à un client ou un enseignant.

Pendant l’exportation, **Reaper** lit toutes les pistes, les effets, les automatisations et les réglages du projet pour créer un nouveau fichier audio final.


# Pourquoi exporter ?

Lorsque vous travaillez dans **Reaper**, votre projet contient :

- Des pistes audio
- Des pistes MIDI
- Des effets
- Des automatisations
- Des marqueurs
- Des fichiers de référence

Le fichier `.rpp` ne peut être lu que par **Reaper**.

Pour partager votre travail, vous devez créer un fichier audio final :

- WAV
- MP3
- FLAC
- AIFF


# Sélectionner une région ou tout le projet

Avant d'exporter, il faut déterminer ce qui sera rendu.


## Option 1 : Exporter tout le projet

**Reaper** exporte du début à la fin du projet.

### Exemple

```
|---------------------------|
Début                    Fin
```

### Utilisation

- Chanson complète
- Balado complet
- Projet final


## Option 2 : Exporter une portion du projet

Vous pouvez sélectionner uniquement une partie.

### Exemple

```
|------ Sélection ------|
```


### Utilisation

- Extrait
- Bande-annonce
- Test de mixage
- Version partielle


## Créer une sélection temporelle (Boucle)

1. Cliquer dans la règle temporelle
2. Glisser vers la droite

Une zone colorée apparaît :

```
|===== Région exportée =====|
```


# Utiliser la fenêtre Render

La fenêtre Render est le centre de contrôle de l'exportation.


## Ouvrir Render

### Menu

```
File > Render
```

### Raccourci

```
Ctrl + Alt + R
```

(ou selon la configuration du clavier)


## Fenêtre Render

Elle contient plusieurs sections importantes :

### Source

Détermine ce qui sera exporté.

Options courantes :

- Master Mix
- Stems sélectionnés
- Pistes individuelles

Pour un projet normal :

```
Master Mix
```


### Bounds

Détermine la durée exportée.

Options fréquentes :

- Entire Project
- Time Selection
- Selected Region

---

### Output Directory

Détermine où sera enregistré le fichier.

Exemple :

```
Projet/
└── Exports/
```


### File Name

Nom du fichier exporté.

Exemple :

```
Balado_Final
```


# Exporter en WAV

Le format WAV est le standard professionnel.


## Avantages

✔ Qualité maximale

✔ Aucune compression

✔ Compatible avec tous les logiciels audio

✔ Recommandé pour l'archivage


## Réglages recommandés

### Sample Rate

```
48000 Hz
```

pour la vidéo

ou

```
44100 Hz
```

pour la musique


### Bit Depth

```
24 bits
```

recommandé


### Exemple

```
Balado_Final.wav
```


# Exporter en MP3

Le MP3 est compressé.


## Avantages

✔ Fichier plus léger

✔ Facile à partager

✔ Compatible partout


## Inconvénients

❌ Légère perte de qualité


## Réglages recommandés

### Bitrate

Pour un balado :

```
128 kbps
```

Pour de la musique :

```
320 kbps
```


### Exemple

```
Balado_Final.mp3
```


# Vérifier les paramètres d’exportation

Avant de cliquer sur Render, il faut toujours vérifier certains éléments.


## 1. Vérifier les niveaux du Master

Observer le Master Meter.

### Correct

```
-6 dB à -1 dB
```


### À éviter

```
0 dB ou plus
```

Cela provoque :

- Saturation
- Distorsion


## 2. Vérifier la durée

S'assurer que :

- Le début est correct
- La fin est correcte


### Problème fréquent

Exporter :

```
0:00 à 15:00
```

alors que le projet dure :

```
0:00 à 5:00
```

Résultat :

10 minutes de silence à la fin.


## 3. Vérifier le nom du fichier

Mauvais :

```
ProjetFinalVersion2DerniereVraieVersion.wav
```

Bon :

```
NomPrenom_BaladoFinal.wav
```


## 4. Vérifier le dossier de destination

Toujours exporter dans :

```
Projet/
└── Exports/
```


## 5. Vérifier le format

Avant le rendu :

- WAV pour la remise finale
- MP3 pour le partage rapide


# Lancer l'exportation

Une fois les réglages validés :

Cliquer sur :

```
Render 1 file
```

ou

```
Render
```

Reaper crée alors le fichier final.


# Exemple d'organisation

```
Projet_Balado/
│
├── Projet_Balado.rpp
├── Audio/
│   ├── Entrevue.wav
│   └── Ambiance.wav
│
└── Exports/
    ├── Balado_Final.wav
    └── Balado_Final.mp3
```


👉 L’exportation est la dernière étape du processus de production et permet de transformer un projet Reaper en un fichier audio prêt à être diffusé ou remis.