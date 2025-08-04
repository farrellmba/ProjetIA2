# CBIR
Ce projet propose une application web de recherche d’images fondée sur l’analyse du contenu visuel d’une image fournie par l’utilisateur, plutôt que sur des mots-clés.

L’utilisateur peut importer une image depuis son appareil, sélectionner un descripteur d’image parmi GLCM\_RGB, Haralick\_RGB, BiT\_RGB ou une combinaison des trois, ainsi qu’un type de distance (Euclidienne, Manhattan, Tchebychev ou Canberra) pour effectuer la comparaison avec les images enregistrées dans la base de données.

L’application extrait automatiquement la signature numérique de l’image soumise en fonction du descripteur choisi, puis la compare à celles des images de référence à l’aide de la distance sélectionnée. Les résultats sont présentés sous forme d’un classement des images les plus proches visuellement.

L’interface utilisateur est construite avec Streamlit, tandis que le traitement d’image repose sur OpenCV et NumPy. Afin d’optimiser les performances, les descripteurs sont pré-calculés et sauvegardés dans des fichiers (.npy)

---
https://github.com/farrellmba/ProjetIA2
