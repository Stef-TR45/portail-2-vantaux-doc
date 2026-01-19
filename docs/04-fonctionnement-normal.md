# Fonctionnement en mode normal

## Règles générales

| Règle | Valeur |
|-------|--------|
| Validation commande | Bouton maintenu ≥ 0,3 s |
| Anti double impulsion | 0,3 s après relâchement |
| Priorité | Sécurités > Commandes utilisateur |

---

## 1. Commandes télécommande

### Bouton A : Ouverture complète

| État du portail | Action |
|-----------------|--------|
| À l'arrêt / pause | Électroaimant 1s → Ouverture complète → Tempo 15s |
| En ouverture | Arrêt immédiat (pause) |
| En fermeture | Arrêt → Électroaimant 1s → Reprise ouverture |

### Bouton B : Fermeture complète

| État du portail | Action |
|-----------------|--------|
| À l'arrêt / pause | Fermeture complète (Dormant puis Maître) |
| En fermeture | Arrêt immédiat (pause) |
| En ouverture | Arrêt immédiat (pause) → Nouvel appui B pour fermer |

### Bouton C : Ouverture piétonne

| État du portail | Action |
|-----------------|--------|
| À l'arrêt / pause | Électroaimant 1s → Ouverture piétonne (Maître seul) → Tempo 15s |
| En ouverture piétonne | Arrêt immédiat (pause) |
| En position piétonne | Relance tempo 15s |

---

## 2. Fermeture automatique

Après ouverture complète ou piétonne :
- Temporisation de **15 secondes**
- Si aucune commande ni anomalie → fermeture automatique

### Pendant la temporisation

| Bouton | Action |
|--------|--------|
| A ou C | Maintien ouvert + relance tempo 15s |
| B | Fermeture immédiate |

---

## 3. Gestion des obstacles et sécurité

### Barrière infrarouge

| Situation | Réaction |
|-----------|----------|
| Obstacle en fermeture | Arrêt → Inversion → Ouverture complète → Tempo 15s |
| Obstacle en ouverture | Arrêt → Pause → Attente commande |

*LED moteurs clignotent 10s*

### Surintensité moteur

Les seuils sont issus de l'apprentissage (hors phase de démarrage).

| Situation | Réaction |
|-----------|----------|
| Surintensité en fermeture | Arrêt → Inversion → Ouverture complète → Tempo 15s |
| Surintensité en ouverture | Arrêt → Pause → Attente commande |

*LED moteurs clignotent 10s*

---

## 4. Gestion des anomalies

### Causes possibles
- Obstacles répétés dans un intervalle court
- Dépassement du temps de parcours maximum
- Incohérence de mouvement

### Procédure en cas d'anomalie

1. Arrêt immédiat des moteurs
2. Blocage des automatismes (fermeture auto désactivée)
3. LED moteurs clignotent 10s
4. Attente commande utilisateur (A, B ou C) pour relancer

---

## 5. Pilotage de l'électroaimant

| Situation | Action |
|-----------|--------|
| Avant ouverture (A ou C) | Alimentation 1s pour libérer le pêne |
| En fermeture | Aucune alimentation |

> ⚠️ L'électroaimant ne doit jamais être alimenté en continu.
