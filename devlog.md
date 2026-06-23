# Devlog — Calepinage de plaques et blocs

Contactez moi si bug majeur détecté ou idées/features à ajouter : julien.fumeron@vinci-construction.com

---

## 2026-06-08 — Base initiale

- Éditeur 2D : calepinage automatique, algorithmique
- Éditeur 3D : visualisation volumique avec coupes
- Métré : Liste plaques, sciages...

## 2026-06-23 — MAJ 1

1. Carottages débouchants corrigés  
- Ajustements de calcul et de restitution pour les cas débouchants, alignés avec les règles métier utilisées dans le rapport.

2. Dimensions plaques conditionnées revues  
- Prise en compte consolidée des dimensions min/max et du gabarit max dans les hypothèses exportées.

3. Masse individuelle carotte ajoutée  
- Intégration explicite de la masse individuelle dans les tableaux carottages et les récapitulatifs.

4. Doublons de traits de scie traités  
- Déduplication des segments de sciage pour éviter les doubles comptages, y compris cas d’axes/plaques hétérogènes.

5. Temps chantier enrichis  
- Ajout/clarification des temps manutention et des temps d’installation scie (rainurage, bloc débouchant, fond borgne).  
- Le temps global intègre ces composantes.

6. Algo orienté nombre de plaques  
- Ajustements pour que certaines composantes de charge/temps soient bien pilotées par le nombre de plaques.

7. Rapport enrichi: page Hypothèses  
- Ajout d’une section hypothèses avec gabarit, dimensions min/max, paramètres principaux et hypothèses de calcul retenues.

8. Rapport enrichi: page Récap  
- Ajout d’une section récap avec masse, nombre de blocs/plaques, temps, carottages, volumes/masses associés.

9. Consommations câble et déchets intégrées  
- Règle explicite: X m² de sciage câble = X ml de câble.  
- Calculs déchets béton, poussière sèche, poussière humide.  
- Conversion en fûts 200 L par type + page dédiée Déchets (avec formules et grandeurs utilisées).

10. Lisibilité schémas carottages améliorée  
- Décalage renforcé des numéros hors cercles, anti-chevauchement et anti-coupure bord image.
