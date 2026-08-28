# reporting — page de redirection uniquement

Ce dépôt est **public**. Il ne contient plus qu'une page de redirection.

## Ne rien remettre ici

L'application et `RESULTATS.xlsx` ont été déplacés vers le dépôt **privé**
`resortnamur/reporting-app`, servi par Cloudflare derrière un code d'accès
vérifié côté serveur.

Tant que ce dépôt est public, tout fichier qui y est déposé est téléchargeable
par n'importe qui, sans compte GitHub et sans code — y compris en tapant
directement son adresse, sans jamais passer par la page.

C'était précisément le défaut corrigé le 28/08/2026 : le classeur des recettes
journalières y était accessible librement, et le code d'accès de la page,
vérifié en JavaScript, valait la date du jour au format `JJMMAAAA`.

## Pourquoi ce dépôt subsiste

Pour que l'adresse historique `https://resortnamur.github.io/reporting/`
continue de fonctionner : les favoris existants y aboutissent et sont
redirigés. GitHub Pages n'étant servi que depuis un dépôt public sur un compte
gratuit, il ne peut pas être passé en privé sans éteindre cette redirection.

## Modifier la destination

Une seule valeur à changer dans `index.html` : la constante `DESTINATION`, et
l'URL identique dans la balise `<meta http-equiv="refresh">` juste au-dessus.
