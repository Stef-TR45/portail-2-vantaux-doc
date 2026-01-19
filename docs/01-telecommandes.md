# Gestion des télécommandes

## 1. Appairage d'une télécommande

### Préconditions
- Carte sous tension
- Portail immobile
- Aucun mode diagnostic ni apprentissage actif

### Procédure
1. Maintenir le **Bouton 1** pendant **5 secondes**
2. Relâcher le bouton

### Indication visuelle
- LED RGB clignote rapidement en **bleu** → mode appairage activé
- Appuyer brièvement sur un bouton (A, B ou C) de la télécommande à associer

### Validation
- LED RGB **bleu fixe** pendant 3 secondes, puis extinction
- Enregistrement confirmé

### Remarques
- Capacité maximale paramétrable par logiciel (jusqu'à X unités)
- L'ajout d'une nouvelle télécommande n'efface pas les précédentes

---

## 2. Suppression d'une télécommande spécifique

### Préconditions
- Carte sous tension
- Portail à l'arrêt

### Procédure
1. Appui long **Bouton 1** (5s) → LED bleue clignotante
2. Relâcher 1 seconde
3. Appui long **Bouton 1** (5s)

### Indication visuelle
- LED RGB clignote rapidement en **violet** → mode suppression activé
- Appuyer brièvement sur un bouton de la télécommande à supprimer

### Validation
- LED RGB **violet fixe** pendant 3 secondes, puis extinction
- Télécommande supprimée de la mémoire

---

## 3. Suppression de toutes les télécommandes

### Procédure
1. Appui long **Bouton 1** (5s) → LED bleue clignotante
2. Relâcher 1 seconde
3. Appui long **Bouton 1** (5s) → LED violette clignotante
4. Relâcher 1 seconde
5. Appui long **Bouton 1** (5s)

### Indication visuelle
- LED RGB **magenta fixe** pendant 3 secondes, puis extinction

### Résultat
- Toutes les télécommandes sont supprimées de la mémoire
