# Mélochroma
Faites jaillir les sons et mélodies de votre imagination pour les métamorphoser en une œuvre d'art vibrante, où chaque note peint un éclat de couleur sur la toile du réel.

## Public cible & objectif narratif
- L'installation est conçue pour les gens de tout âge

<br>

L'installation invite le public à explorer la fusion sensorielle entre la musique et la couleur, en transformant chaque mélodie jouée en une représentation visuel unique, créant ainsi une expérience immersive où son et image se rejoignent.

<br>

## Message Personnel

## Moodboard Visuel

## Moodboard Sonore

## Scénario interactif

```mermaid
    flowchart TD
 subgraph s1["Spotlight sur clavier, projection éteinte"]
        n1["Mode veille<br>"]
  end
    n1 -- commencer l'interaction --> n2["S'assoir sur le banc (détecteur de pression)"]
    n2 -- ouverture des lumieres --> n5["Animation de détection"]
    n5 -- choix --> n4["Mode performance"] & n3["Mode libre"]
    n4 --> n6["Début chrono 60s"]
    n3 --> n7["Manipulation de clavier synthétiseur"]
    n6 --> n8["Manipulation de clavier synthétiseur"]
    n7 --> n9["Visuel ondes jouées"]
    n8 --> n10["Visuel ondes jouées"]
    n9 --> n11["terminer"]
    n10 --> n12["fin chrono"]
    n11 --> n14["Si absence d'interactivité"]
    n11 -- retour mode de sélection --> n5
    n14 -- 2min et plus --> s1
    n12 --> n15["terminer"] & n16["recommencer"]
    n16 --> n6
    n15 --> n17["écouter performance"] & n14
    n14 -- moins de 2min --> n5
    n17 --> n16
```

## Exemples concrets

## Outil et logiciel technique
