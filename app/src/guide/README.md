---
sidebar: auto
---

# Guide

## Carte

![Carte riskpaca à l'accueil](../assets/map-tools.jpg)

### Outils
- `Echelle`: Sélection rapide de l'échalle de la carte
- `Fond de carte`: Sélection du fond de carte à appliquer
- `Zoom`: Zoomer (+/-) sur la carte
- `Calcul de surface`: Permet de calculer la surface d'un polygone en km²
- `Calcul de distance`: Permet de calculer la distance d'un tronçon en km
- `Moteur de recherche`: Recherche parmi toutes les `Couches cartographiques`, `Actualités`, `Entités cartographiques` et `Infos & règlementations`

### Moteur de recherche

La sélection des éléments trouvés par le moteur de recherche a différentes conséquences selon le type d'élément.

#### Couche Cartographique
Ajoute la couche cartographique au contexte courant et l'affiche sur la carte.

#### Infos & Règlementations
Affiche et zoome sur l'élément sur la carte.
Ouvre le panneau d'informations de l'élément.

#### Actualités
Affiche et zoome sur les communes porteuses de l'actualité sur la carte.
Ouvre le panneau d'informations de l'élément.

#### Entités cartographiques
Affiche et zoome sur l'élément sur la carte.
Ouvre le panneau d'informations de l'élément.



## Contextes
![Panneau "Contextes"](../assets/contextes.png)

Met en surbrillance le contexte actif parmi la liste des contextes sélectionnables.

### Ajouter un nouveau contexte
L'ajout d'un nouveau contexte ou l'administration de ceux déjà existants se fait par le backoffice d'ORRM.

> Structure > Taxonomie > Preset

![Chemin d'accès a l'administration des contexte](../assets/add-preset-path.png)

![Bouton d'ajout d'un contexte](../assets/add-preset-button.png)



## Couches

### Couches sélectionnées
![Panneau "Couches"](../assets/couches-selection.png)

Le panneau de couches affiche les couches sélectionnées.  
Il existe cependant 3 "sous-types" de couches:
- Les éléments de cartographie, constitués des `Actualités`, `Entités cartographiques` et `Infos & règlementations` et reconnaissables par l'icone de roue crantée en haut à droite
- Les couches du contexte, qui ne peuvent pas être retirées
- Les couches ajoutées par l'utilisateur lors de sa navigation, qu'il peut retirer en cliquant sur la croix rouge en haut à droite

Il est possible, pour chacune des couches, de piloter son affichage, son opacité et son ordre d'affichage (en glisser-déposer)

### Catalogue de couches
#### Sélection
![Panneau "Catalogue de couches"](../assets/couches-catalogue.png)

Le panneau "Catalogue de couches" indexe toutes les couches disponibles et permet de les utiliser dans le contexte sélectionné.

#### Ajout de flux WMS
![Modale d'ajout de flux WMS](../assets/couches-ajout-flux.png)

Il est possible d'ajouter son propre flux WMS s'il n'est pas disponible dans le catalogue.  
Par exemple, pour un flux WMS récupéré dans le catalogue du CRIGE:

Il est possible de récupérer le lien du flux de la couche cartographique qui nous intéresse sur les ressources qui portent une "API Géo"
![Bouton "API Géo" du catalogue du CRIGE](../assets/crige-bouton-api-geo.png)
![Lien du flux de la couche cartographique du catalogue du CRIGE](../assets/crige-lien-flux-couche.png)

Il suffit d'intégrer ce lien dans la modale d'ajout de flux WMS
![Modale d'ajout de flux WMS complétée](../assets/couches-ajout-flux-crige.png)

La couche sera ensuite ajoutée au catalogue de couches pour votre instance. Il suffit de l'activer pour la voir apparaître sur la carte
![Couche WMS Active](../assets/couche-wms-active.jpg)


#### Filtrage
![Panneau "Catalogue de couches", filtres visibles](../assets/couches-catalogue-filtres.png)

Les couches du catalogue sont filtrables par nom, thématique, phénomène et profil.

#### Ajouter une couche au catalogue

L'ajout d'une nouvelle couche et l'administration de celles déjà présentes se font par le backoffice d'ORRM.

![Chemin d'accès a l'administration des couches du catalogue](../assets/add-couche-path.png)
![Bouton d'ajout de couche au catalogue](../assets/add-couche-button.png)

Saisir le lien du flux, sans les paramètres
![Bouton d'ajout de couche au catalogue](../assets/add-couche-flux.png)

Définir le bon type de couche et les paramètres au format JSON.  
S'ils ne sont pas saisis, certains paramètres sont substitués par leurs valeur par défaut:
- FORMAT
- HEIGHT
- WIDTH
- CRS
- VERSION

Aussi, les paramètres suivants ne doivent pas êtres saisis:
- SERVICE
- REQUEST

![Bouton d'ajout de couche au catalogue](../assets/add-couche-params.png)

Dans le cas d'un flux WFS, celui-ci ne portant pas les styles d'affichage des features qu'il expose, il faut les préciser au format SLD (disponible dans le catalogue du CRIGE).


## Légende
![Panneau "Legende"](../assets/legende.png)

Affiche en permanence les légendes des `Actualités`, `Entités cartographiques` et `Infos & règlementations`.
Affiche les légendes des couches WMS si leur flux en expose.



## A propos
![Panneau "a propos"](../assets/a-propos.png)

Les liens redirigent vers leurs pages correspondantes sur le site ORRM.

La date de dernière mise à jour et la version sont mises à jour automatiquement.

