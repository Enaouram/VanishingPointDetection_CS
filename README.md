# Projet de Reconnaissance Visuelle : Détection du Point de Fuite CentraleSupélec

## Vue d'ensemble
Ce dépôt contient le développement et l'exploration de plusieurs algorithmes visant à détecter le point de fuite dans des images. Ce travail fait partie d'une étude approfondie des techniques de vision par ordinateur pour identifier précisément les points de fuite, essentiels pour des applications telles que la conduite autonome, la robotique et la réalité augmentée.

## Structure du Répertoire

### Notebooks
- **VNP_ALGOS.ipynb** : Contient trois approches expérimentales différentes pour la détection du point de fuite :
  - **Algorithme inspiré par RANSAC** : Tente de trouver le point de fuite via une méthode statistique robuste capable de gérer efficacement les valeurs aberrantes.
  - **Méthode basée sur les équations des lignes** : Utilise les équations mathématiques des lignes détectées dans l'image pour calculer les intersections suggérant des points de fuite potentiels.
  - **Approche de Clustering** : Se concentre sur le regroupement des points d'intérêt qui pourraient indiquer la convergence des lignes vers le point de fuite. Ce carnet inclut une analyse détaillée et des comparaisons avec le VNP de vérité terrain fourni par le dataset.
- **VNP_SEG.ipynb** : Dédié à des scénarios d'image plus complexes, ce carnet explore les approches de segmentation, l'optimisation de LineSet et l'algorithme de détecteur de segments de ligne (LSD).
- **Reconstruction_Scene_3D.ipynb** : Explore les techniques de création de scènes 3D à partir de points de fuite dérivés des analyses d'image, offrant une profondeur géométrique à la compréhension des images.

### Road_Annotated_Dataset
Ce dossier contient le dataset obtenu de [Roboflow Universe](https://universe.roboflow.com/vanishing-point-and-road-detection/vanishingpointdetection), spécifiquement utilisé pour l'entraînement et les tests de nos algorithmes. Les descriptions détaillées et annotations sont incluses dans le carnet VNP_ALGOS.

### Images_SEG
Contient les images utilisées dans le carnet VNP_SEG, se concentrant sur les approches segmentées et les méthodes de détection de lignes avancées.

### Image d'Approche de Clustering
Comprend une explication visuelle de l'approche de clustering discutée dans le carnet VNP_ALGOS. Cette image aide à illustrer notre concept théorique et son application dans la détection des points de fuite.

## Pour Commencer

Pour démarrer avec ce projet :
1. Clonez le dépôt.
2. Assurez-vous d'avoir [Python](https://www.python.org/) installé, ainsi que des bibliothèques telles que [OpenCV](https://opencv.org/), [NumPy](https://numpy.org/), et [Matplotlib](https://matplotlib.org/).
3. Naviguez vers le répertoire `Notebooks` et lancez les carnets Jupyter pour voir les algorithmes en action.


## Références

1. Enrico Calleris, "Vanishing Point Detection," Medium, [Link](https://medium.com/@calleris.enrico/vanishing-point-detection-14250afa24d3).
2. Scientific Reports, Nature, 2023, [Link](https://www.nature.com/articles/s41598-023-30152-7).
3. IET Digital Library, "Journal Article on Vanishing Point Detection," IET Research Journals, [Link](https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/iet-cvi.2014.0187).
4. Ray Ryeng, "XiaohuLuVPDetection," GitHub Repository, [Link](https://github.com/rayryeng/XiaohuLuVPDetection).
5. IEEE Xplore, "Document Detail," IEEE, [Link](https://ieeexplore.ieee.org/document/10006943).
6. PyPI, "lu-vp-detect," Python Package Index, [Link](https://pypi.org/project/lu-vp-detect/).
7. IOPscience, "Journal of Physics: Conference Series," IOP Publishing, [Link](https://iopscience.iop.org/article/10.1088/1742-6596/1748/3/032052/pdf).

