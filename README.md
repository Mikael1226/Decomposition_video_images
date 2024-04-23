# Decomposition_video_images

Dans ce travail, j'ai effectué trois étapes (la dernière est un ajout) :

- J'ai créé une fonction qui permet de découper la vidéo capturée par le bathybot en plusieurs images. Mais avant cela, j'ai cherché à obtenir des informations sur la longueur de la vidéo, ce qui est utile par la suite.
  
- J'ai généralisé sur le pas de temps pour contrôler le biais. Par exemple, si la vidéo dure 52 images et que j'ai besoin de la découper en trois images, la fonction me renvoie une erreur indiquant qu'elle n'est pas compatible avec la longueur de la vidéo (c'est comme effectuer une division par zéro).
  
- J'ai appliqué l'algorithme de seam carving pour redimensionner les images de très grande dimension. Cela nous permettra, par exemple, dans les images décomposées par la vidéo, de capturer le poisson de manière plus proche. Cet algorithme nous aide à éliminer les zones de moindre énergie tout en préservant les parties importantes. Ceci peut être utile dans l'étape suivante de la base d'apprentissage.
