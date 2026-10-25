# Documents-revision

Pages web de révision interactives pour mes cours (GCI, GLG…), publiées avec GitHub Pages.

**Site : https://richard-jn.github.io/Documents-revision/**

| Cours | Page |
|---|---|
| GCI-1000 · Matériaux de construction | https://richard-jn.github.io/Documents-revision/gci-1000/ |
| GLG-1000 · Géologie | https://richard-jn.github.io/Documents-revision/glg-1000/ |

La progression (sujets révisés, quiz, indice de confiance) reste dans le navigateur de chaque personne.

## Mettre à jour

Les pages sont générées avec la trousse de révision (v6 ou plus récente), pas modifiées à la main :

```
python3 build.py courses/<cours>                 # construire et tester comme d'habitude
python3 publier.py ../Documents-revision         # reconstruit chaque cours + l'accueil dans ce dépôt
cd ../Documents-revision && git add -A && git commit -m "Mise à jour GCI-1000" && git push
```

Le site se met à jour 1 à 2 minutes après le push. Pour un nouveau cours, `publier.py` l'ajoute aussi à l'accueil (`cours.json`).
