# Wave3D
*Faites prendre formes les sons que votre imagination compose*

## Concept

***Wave3D*** propose une interaction directe avec un synthétiseur qui, à chaque note jouée, fait vibrer des cordes physiques. Ces vibrations révèlent visuellement les ondes sonores et les fréquences produites. Le public est invité à expérimenter et à observer la manière dont les sons prennent forme, offrant une exploration à la fois auditive et visuelle des compositions musicales.

### Public cible & objectif
- L'installation est conçue pour les gens de tout âge

L'installation invite le public à explorer la nature du son et des compositions mélodiques en découvrant les ondes que ceux-ci génèrent.

## Mise en scène

L'interacteur est accueilli dans une pièce sombre, où un projecteur éclaire un synthétiseur au centre, accompagné d'un banc sur lequel il est invité à s'asseoir. Une douce ambiance sonore joue en fond, renforçant l'immersion. Dès qu'il s'installe, un détecteur de pression sous le banc capte sa présence et déclenche une animation de bienvenue, illuminant les cordes face au clavier. L'interacteur est alors invité à jouer, produisant des ondes sonores qui font vibrer les cordes en synchronisation avec les notes. Il peut choisir entre deux modes : le mode "performance", pour enregistrer ses compositions, ou le mode "libre", pour explorer et s'amuser en toute simplicité avec le clavier.


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

## Composantes techniques

### Composantes principales

- **Synthétiseur** : Un clavier synthétiseur numérique qui génère les sons et ondes selon les notes jouées.
  
- **Cordes vibrantes** : Des cordes physiques (comme des cordes de guitare ou des fils tendus) reliées à un système de vibration ou de résonance pour réagir aux fréquences et ondes sonores produites par le synthétiseur.
  
- **Amplificateurs et transducteurs** : Ces dispositifs permettent de convertir les signaux sonores en vibrations physiques sur les cordes, les faisant réagir aux sons produits par le synthétiseur.
  
- **Système de détection de présence (capteur de pression)** : Un capteur de pression ou un interrupteur caché sous le banc pour détecter la présence de l'utilisateur et déclencher l’animation de bienvenue.
  
- **Système de projection et éclairage** : Un projecteur pour éclairer le synthétiseur et des lumières LED ou un système d'éclairage programmable pour illuminer les cordes pendant l'animation.
  
- **Interface de contrôle (ordinateur ou microcontrôleur)** : Un ordinateur ou un microcontrôleur (comme Arduino ou Raspberry Pi) pour gérer les interactions entre les capteurs, le synthétiseur, les transducteurs et les lumières. Il centralise les signaux et déclenche les différentes actions (lumières, sons, vibrations).
  
- **Système d'enregistrement audio** : Un système d'enregistrement pour sauvegarder les compositions créées par l'interacteur.
   
- **Enceintes et système audio** : Pour la diffusion de l’ambiance sonore et des sons générés par le synthétiseur, un système de haut-parleurs est nécessaire.
  
- **Logiciel interactif** : Un programme qui synchronise les actions, comme l'activation des cordes en fonction des notes jouées, la gestion des modes "performance" et "libre", ainsi que l’enregistrement des sons. (Touchdesigner ou MAX)
  
- **Support structurel** : Un cadre solide ou un système de montage pour maintenir les cordes tendues et bien alignées par rapport au synthétiseur.

