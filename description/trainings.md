## Entraînements avec des données Pirenne
Exemple de page:



| Nom du modèle | Caractéristiques techniques | Données utilisées  | Nombre de pages   |  Fine-tuné à partir de    |  Accuracy (validation)  |  Accuracy (test)    |     Résultat        |
|-------|-------|------|-------|---------|--------|-------|-------|
| Pirenne50 |   | Mahomet et Charlemagne, Les anciennes démocraties des Pays-Bas | 50 | Manu McFondue |0.8997153043746948 |89.90%| |
| Pirenne100 |    |    | 100 | Manu McFondue |  |88.84%| |
| Pirenne160 |  -r 0.0002 --lag 10 --min-delta 0.001 --workers 8   |    | 160 | Manu McFondue | 0.9116478562355042 | 91.51% | Image |
| Pirenne_0 |    |    | 420 | ----- |  |  | Image |
| **Pirenne420** | -r 0.0002 --lag 10 --min-delta 0.001 --workers 8  |    | 420 | Manu McFondue |  |  | Image |
| **Pirenne_et_autres** |  -r 0.0002 --lag 10 --min-delta 0.001 --workers 8  |    | 833 | ------ |  |  | Image |
| **AdHoc** | ketos train -t data_autres/train.txt -e data_autres/val.txt -f alto -r 0.0003 --lag 20 --min-delta 0.001 --workers 8 -B 8 --precision 16 -d |    | 413 | ----- |  |  | Image |
| Pirenne420adhoc |    |    | 420 | Modèle ad hoc |  |  | Image |




## Données dans modèle ad hoc HTR


| Projet  | Langue  | Dates   | Pages  |  Lien Github                 |
|-------|-------|---------|--------|------------------------|
| Cremma MSS 20 | Fr   | 20e s.   | 7 | https://github.com/HTR-United/CREMMA-MSS-20/tree/main/data/Lettre_de_ETessier_a_G-VTessier |
| CREMMA-AN-TestamentDePoilus | Fr | 1898-1918| 226  |  https://github.com/HTR-United/CREMMA-AN-TestamentsDePoilus/tree/main |
| FONDUE-FR-MSS-19 | Fr | 1893 | 99   | https://github.com/FoNDUE-HTR/FONDUE-FR-MSS-19/tree/main/data/zola_bodmer_Z-6-3 |
| CREMMA-MSS-19 | Fr | 19e s. | 7   | https://github.com/HTR-United/CREMMA-MSS-19/tree/main |
| Digital Peraire project | Fr | 20e s. | 70   | https://github.com/alix-tz/peraire-ground-truth |
| Cours HNU2000 à l'Université de Montréal  | Fr | 1914-1915 | 4   | https://github.com/alix-tz/dataset-celestine-doniau-danest |
| TOTAL |  |  | 413   |  |
