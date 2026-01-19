# Référence des états LED

## Modes de fonctionnement (clignotement)

| Couleur | Fréquence | Mode | Bouton |
|---------|-----------|------|--------|
| Bleu | Rapide | Appairage télécommande | 1 (5s) |
| Violet | Rapide | Suppression télécommande | 1 (5s+5s) |
| Magenta | Rapide | Suppression toutes télécommandes | 1 (5s+5s+5s) |
| Blanc | Lent | Diagnostic moteurs | 2 (5s) |
| Cyan | Lent | Diagnostic sorties | 2 (5s+5s) |
| Jaune | Lent | Diagnostic entrées | 2 (5s+5s+5s) |
| Rouge | Rapide | Apprentissage Maître | 3 (5s) |
| Vert | Rapide | Apprentissage Dormant | 3 (5s+5s) |

---

## Validations et confirmations (fixe 3s)

| Couleur | Signification |
|---------|---------------|
| Bleu fixe | Télécommande appairée avec succès |
| Violet fixe | Télécommande supprimée |
| Magenta fixe | Toutes télécommandes supprimées |
| Rouge fixe | Butée fermeture mémorisée |
| Vert fixe | Butée ouverture mémorisée |
| Blanc fixe | Fin apprentissage (Maître ou Dormant) |

---

## Diagnostic entrées (fixe pendant test)

| Couleur | Entrée testée |
|---------|---------------|
| Cyan fixe | Contact clé activé |
| Rouge fixe | Barrière IR obstruée |
| Orange fixe | Contact électroaimant enclenché |

---

## Fréquences de clignotement

| Type | Période approximative |
|------|----------------------|
| Rapide | ~200 ms (5 Hz) |
| Lent | ~1000 ms (1 Hz) |

---

## Récapitulatif par bouton

### Bouton 1 - Télécommandes
```
5s      → Bleu rapide    (appairage)
5s+5s   → Violet rapide  (suppression une)
5s+5s+5s → Magenta rapide (suppression toutes)
```

### Bouton 2 - Diagnostic
```
5s      → Blanc lent  (moteurs)
5s+5s   → Cyan lent   (sorties)
5s+5s+5s → Jaune lent  (entrées)
```

### Bouton 3 - Apprentissage
```
5s    → Rouge rapide (Maître)
5s+5s → Vert rapide  (Dormant)
15s   → Blanc fixe   (fin apprentissage)
```
