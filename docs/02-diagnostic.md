# Mise en route et diagnostic

## Préconditions mécaniques obligatoires

Avant de commencer :

1. **Positionner manuellement les deux vantaux à mi-course**

Cette disposition permet de :
- Prévenir tout blocage mécanique entre vantail maître et dormant
- Garantir l'ouverture sans contrainte du vantail dormant
- Éviter toute fermeture accidentelle (sens moteur inversé)

### Vérifications installateur
- Aucun obstacle n'entrave le mécanisme
- L'électroaimant n'est pas verrouillé

### Branchement moteurs
| Moteur | Sortie |
|--------|--------|
| Vantail Maître | Sortie moteur 1 |
| Vantail Dormant | Sortie moteur 2 |

> ⚠️ En l'absence de ces conditions, ne pas engager la procédure.

---

## 1. Vérification des moteurs

### Accès au mode
- Maintenir **Bouton 2** pendant **5 secondes**
- LED RGB clignote lentement en **blanc**

### Objectifs
- Identifier le moteur maître et le moteur dormant
- Vérifier le sens d'ouverture/fermeture
- Ajuster le sens via micro-switch si nécessaire

> Aucune temporisation : les moteurs fonctionnent uniquement tant que le bouton est maintenu.

### Étape 1 : Vérification du moteur maître

Le moteur maître est généralement doté d'un blocage mécanique (souvent couplé à un électroaimant).

| Bouton | Action |
|--------|--------|
| A | Rotation ouverture supposée |
| B | Rotation fermeture supposée |
| C | Valide et passe à l'étape 2 |

**Si l'ouverture n'est pas conforme** : inverser le micro-switch du moteur 1 et répéter les tests.

### Étape 2 : Vérification du moteur dormant

Le moteur dormant doit être libre de toute entrave (pas d'électroaimant généralement).

| Bouton | Action |
|--------|--------|
| A | Ouverture |
| B | Fermeture |
| C | Valide et quitte le mode |

**Si l'ouverture n'est pas conforme** : inverser le micro-switch du moteur 2.

### Cas particulier : inversion des moteurs
Si le moteur actionné ne correspond pas au vantail attendu, inverser les branchements électriques des moteurs 1 et 2, puis redémarrer à l'étape 1.

### Sortie du mode
- Validation complète (maître + dormant)
- Ou annulation : appui bref sur **Bouton 2**
- LED RGB s'éteint ou revient à l'état nominal

---

## 2. Diagnostic sorties (Éclairage et électroaimant)

### Accès au mode
1. Appui long **Bouton 2** (5s) → LED blanche clignotante
2. Relâcher 1 seconde
3. Appui long **Bouton 2** (5s) → LED **cyan** clignotante

### Commandes télécommande
| Bouton | Action |
|--------|--------|
| A | Éclairage moteur maître |
| B | Éclairage moteur dormant |
| C | Activation électroaimant |

### Sortie
- Appui bref sur **Bouton 2**

---

## 3. Diagnostic entrées (Clé, barrière IR, switch électroaimant)

### Accès au mode
1. Appui long **Bouton 2** (5s) → LED blanche
2. Relâcher 1s, appui long (5s) → LED verte
3. Relâcher 1s, appui long (5s) → LED **jaune** clignotante

### Tests à effectuer

| Élément | Action | LED attendue |
|---------|--------|--------------|
| Contact clé | Activer le switch | Cyan fixe |
| Barrière IR | Placer un obstacle | Rouge fixe |
| Contact électroaimant | Enclencher manuellement | Orange fixe |

Si la LED ne réagit pas correctement, vérifier le câblage.

### Sortie
- Appui bref sur **Bouton 2**
