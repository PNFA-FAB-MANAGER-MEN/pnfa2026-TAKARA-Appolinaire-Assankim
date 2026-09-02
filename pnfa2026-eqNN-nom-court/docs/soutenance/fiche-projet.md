# Fiche projet — Équipe 20

> Livrable L2 · Jalon J1 (samedi 29 août 2026) · validée par l'encadreur référent.
> Aucune fabrication n'est autorisée avant la validation de ce jalon.

## 1. Titre et accroche

Robot éducatif programmable.

## 2. Besoin et bénéficiaires

La difficulté d'apprentissage visée:Facilité la conpréhension des boucles,coditionnement,etc.

## 3. Objectifs d'apprentissage

Trois objectifs observables rattachés au programme officiel, chapitre cité.
1.Conditionner une action
2.Programmation en bloc.
3.Calibration expérimentale.

## 4. Description du dispositif

L'objet est réaliser pour pour faire des actions comme:suivre des lignes par exemple.

## 5. Architecture technique pressentie

- 1 × Arduino Uno (contrôleur)
- 1 × capteur sonore KY-038 (mesure du niveau sonore)
- 3 × LED (vert, jaune, rouge)
- Résistances adaptées aux LED (généralement 220-330 Ω)
- Câbles de liaison + breadboard
Alimentation USB

## 6. Rôle des élèves

Gérer plusieurs niveaux de décision, pas juste un seuil unique.

## 7. Ancrage réseau et implantation

Lab de rattachement: établissement· lieu d'usage:Tous les établissements· conditions matérielles de la salle:Le fils électrique est suffisant.

## 8. Périmètre
| | Contenu | 
|---|---|
| Dans la v1.0 (Socle)	Capteur sonore KY-038, Arduino Uno, 3 LED (vert/jaune/rouge) selon 2 seuils, alimentation USB, boîtier imprimé en 3D | |
| En option (Avancé/Expert)	Buzzer d'alerte sonore, écran LCD affichant la valeur en direct, historique des pics sonores dans le temps | |
| Explicitement exclu	Reconnaissance vocale, distinction entre types de bruit (voix vs objet), application mobile, envoi d'alertes à distance | |

## 9. Risques et parades
| Risque | Type | Parade |
|---|---|---|
|  Le capteur KY-038 est sensible aux parasites valeurs instables |	technique |	Lissage par moyenne mobile sur plusieurs lectures ; calibration des seuils en conditions réelles |
|  L'imprimante 3D est partagée entre 25 équipes, risque de retard pour le boîtier (V3) |	calendrier|	Réserver un créneau d'impression dès la V2 validée ; prévoir 2-3 jours de marge avant le jalonalendrier | |
|  Les seuils calibrés en test peuvent ne pas correspondre à une vraie salle pleine d'élèves|	pédagogique|	Tester dans une salle réellement occupée avant la démonstration finale ; ajuster les seuils sur place | |

## 10. Budget matière estimé

Grandes masses en FCFA (plafond 60 000 FCFA) :

Arduino Uno : ~9 000 FCFA
Capteur KY-038 : ~1 500 FCFA
3 LED + résistances : ~500 FCFA
Buzzer : ~1 000 FCFA
Câbles/breadboard : ~2 000 FCFA
Filament impression 3D (boîtier) : ~2 500 FCFA
Divers (colle, vis) : ~1 000 FCFA

Total estimé : ~17 500 FCFA — largement dans le plafond, marge confortable pour imprévu.
## 11. Licences et diffusion

Code source : licence MIT — motivation : permettre à d'autres classes/promotions de réutiliser et adapter librement le code
Documentation, schémas, cahier de projet : licence Creative Commons BY-SA — motivation : partage libre avec obligation de citer l'équipe
Accord de l'équipe pour la mise en avant réseau : à faire valider par les 4 membres avant dépôt final

## Exemptions demandées
- [x] ET-FAB-06 (moulage) — justification : le boîtier est réalisé par impression 3D (FDM), 
      technique suffisante pour loger et protéger l'électronique ; aucune pièce moulée n'est nécessaire au fonctionnement du projet.
- [x] ET-MEC-01 (fonction motorisée) — justification : le projet est un indicateur visuel et sonore 
statique (LED + buzzer), sans aucune pièce mobile ni actionnement mécanique requis pour répondre au besoin identifié.
