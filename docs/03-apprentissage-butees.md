# Apprentissage des butées

## Préconditions

- Télécommande appairée
- Diagnostic moteurs validé
- Sens de rotation correct
- Vantaux positionnés à mi-course

---

## 1. Apprentissage du vantail Maître

### Accès au mode
- Maintenir **Bouton 3** pendant **5 secondes**
- LED RGB clignote rapidement en **rouge**

### Étape 1 : Validation de la fermeture

1. Maintenir **Bouton B** pour positionner le vantail dans une zone intermédiaire
2. Relâcher **Bouton B**
3. Appuyer brièvement sur **Bouton A**

➡️ Le vantail se ferme automatiquement jusqu'à détection de surintensité et switch porte fermée activé  
➡️ Position mémorisée comme **butée de fermeture**

*LED rouge fixe pendant 3 secondes*

### Étape 2 : Validation de l'ouverture

1. Maintenir **Bouton B** jusqu'à la position d'ouverture souhaitée
2. Relâcher **Bouton B**
3. Appuyer brièvement sur **Bouton A**

➡️ Position mémorisée comme **butée d'ouverture**  
➡️ Mesure du temps et du courant jusqu'à la fermeture

*LED verte fixe pendant 3 secondes*

### Étape 3 : Cycle automatique de validation

1. Appuyer brièvement sur **Bouton A**

➡️ Ouverture automatique jusqu'à la position mémorisée  
➡️ Après 5 secondes, fermeture automatique  
➡️ Recalcul et lissage des valeurs de courant et de temps

### Fin de l'apprentissage Maître
- Appui long **Bouton 3** pendant **15 secondes**
- LED blanche fixe 3 secondes, puis extinction

---

## 2. Apprentissage du vantail Dormant

### Accès au mode
1. Appui long **Bouton 3** (5s) → LED rouge clignotante
2. Relâcher **1 seconde**
3. Appui long **Bouton 3** (5s)

LED RGB clignote rapidement en **vert**

### Pré-positionnement du Maître
- Appui bref sur **Bouton C**
- Le vantail Maître se déplace automatiquement en position intermédiaire sécurisée

### Étapes (identiques au Maître)

| Action | Bouton |
|--------|--------|
| Positionnement | B maintenu |
| Validation fermeture | A bref |
| Positionnement ouverture | B maintenu |
| Validation ouverture | A bref |
| Cycle automatique | A bref |

### Fin de l'apprentissage Dormant
- Appui long **Bouton 3** pendant **15 secondes**
- LED blanche fixe 3 secondes, puis extinction

---

## Cas particulier : Portail en pente

Si la pente génère des courants asymétriques, connecter temporairement :

| Entrée | Moteur |
|--------|--------|
| Fin de course Aux1 | Maître |
| Fin de course Aux2 | Dormant |

> Les entrées Aux remplacent la détection par surintensité pendant l'apprentissage uniquement.  
> Les capteurs sont retirés après apprentissage.
