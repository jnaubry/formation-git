# Convention pour les messages de commit

```
type(scope): subject 

<body>
<footer>
```

### 1. Type de commit
```
feat:    Nouvelle fonctionnalité ajoutée à l'application
fix:      Correction de bug
style:    Ajout/mise à jour de fonctionnalité en lien avec le style (css, UI, UX)
refactor: Refactorisation d'une section de code spécifique
test:     Tout ce qui est relatif aux tests
docs:     Tout ce qui est relatif à la documentation
chore:    Maintenance de code
```

### 2. Scope ou "portée" (Optionnel)
Fourni entre parenthèses après le type de commit, le scope (ou "portée des modifications" en français) décrit les parties du code affectées par les changements réalisés.
```
feat(claims)
fix(orders)
```

### 3. Subject ou objet
Courte description du changement appliqué.
- Doit faire moins de 50 caractères
- Votre message de commit ne doit pas contenir de signes de ponctuation ou d'erreurs d'espacement
- Ne doit pas se terminer par un .
- Doit utiliser le temps au présent de l'indicatif ou le mode impératif
```
feat(reclamations): ajout page de reclamations
fix(commande): validation nouvelle specification
```

### 4. Body ou corps (Optionnel)
Utilisez le corps du message de commit pour décrire les changements qui ont été fait et pourquoi ils ont été faits.
- Séparer l'objet du corps du texte par une ligne blanche
- Limiter chaque ligne à 72 caractères
- Ne pas supposer que la personne qui va revoir votre commit comprenne le problème initial, expliquez-le ici
- Ne pas supposer que votre code est clair et ne nécessite pas d'explications

```
refactor!: suppression du support pour Node6
MODIFICATION IMPORTANTE : nouvelles fonctionnalités JavaScript pas 
disponibles dans Node6.
```

### 5. Footer ou pied de page (optionnel)
Utilisez cette section pour ajouter les bugs (issues) affectés par vos modifications ou pour envoyer des commentaires à d'autres développeurs / testeurs.

```
fix(commandes): correction de typos dans le code
Voir le bug pour plus de détails sur les typos corrigés.
Reviewed-by: @John Doe
Refs #133
```
