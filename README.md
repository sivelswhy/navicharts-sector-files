# NaviCharts — sector files Aurora

Sector files IVAO exportés du cache du client ATC [Aurora](https://www.ivao.aero) (format JSON), un dossier par
sector file : `global.json` (aérodromes, points, routes, positions ATC), `section_NNN_X_Y.json` (tuiles des niveaux de
zoom 0 à 6 : contours, espaces, MVA), `proc_<OACI>.json` (procédures) et `ground_<OACI>.json` (plan au sol précalculé
depuis les tuiles des niveaux 7 et plus, qui ne sont pas conservées).

Utilisés par [NaviCharts](https://github.com/sivelswhy/navicharts) : cloner ce dépôt dans `sector files/aurora/`
à la racine du projet, puis `npm run data`.

```sh
git clone https://github.com/sivelswhy/navicharts-sector-files.git "sector files/aurora"
```

Pour ajouter des sector files : déposer les exports `.zip` d'Aurora dans ce dossier, puis, depuis NaviCharts,
`npm run import-aurora` (extraction, plans au sol, tuiles inutiles retirées) ; commiter et pousser ce dépôt.

Données issues des divisions IVAO, pour la simulation de vol uniquement. Ne pas utiliser pour la navigation réelle.
