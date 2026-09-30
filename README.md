# NaviCharts — sector files Aurora

Sector files IVAO exportés du cache du client ATC [Aurora](https://www.ivao.aero) (format JSON), un dossier par
sector file : `global.json` (aérodromes, points, routes, positions ATC), `section_NNN_X_Y.json` (tuiles par niveau
de zoom : contours, plans au sol, espaces, MVA) et `proc_<OACI>.json` (procédures).

Utilisés par [NaviCharts](https://github.com/sivelswhy/navicharts) : cloner ce dépôt dans `sector files/aurora/`
à la racine du projet, puis `npm run data`.

```sh
git clone https://github.com/sivelswhy/navicharts-sector-files.git "sector files/aurora"
```

Données issues des divisions IVAO, pour la simulation de vol uniquement. Ne pas utiliser pour la navigation réelle.
