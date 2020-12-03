# Faster-RCNN-Receipt-detection

###  Transfert learning(Faster R-CNN) : Prédiction de zones délimitantes les réçus ainsi que leur total( voir work_notebook.ipynb pour le code)
![PicsArt_12-03-03 19 40](https://user-images.githubusercontent.com/33714469/100955992-e0627180-3517-11eb-81a1-20384d208ef8.png)


-- *Objectif* : Développer un système d'extraction d'informations pertinantes d'une image ( reçu et sa zone de total dans notre cas)


## Dataset utilisé:
- Lien du dataset :  https://github.com/clovaai/cord);
- Documentation du dataset: https://openreview.net/pdf
- les données et le model n'ont pas pu être téléchargé ici à cause des contraintes de taille 


## Environnement:
- Model : Faster-RCNN
- Google colab : Torch>=1.5.0 (Gpu) + pandas + matplotib + PIL


## les points abordées dans ce notebook sont:
- Extraction des coordonnées délimitant les reçus et leur total des fichiers d'annotation
-  Sélection des reçus disposant de coordonnées de points les délimitant
-  Redimensionnement des images (moyenne des longueurs et largeurs des 4 premieres resolutions apparaissant le plus dans le dataset)
-  Modification des classes pytorch pour l'entrainement sur le dataset( certains fichiers et lignes de codes proviennent du répertoire [github](https://pytorch.org/tutorials/intermediate/torchvision_tutorial.html) officiel de pythorch : segmentation et prediction COCO) 
-   Utilisation d'un modèele Faster R-CNN avec un réseau ResNET-50 fPN pour l'entrainnement
-  Visualisation des résultats sur les données de test 


