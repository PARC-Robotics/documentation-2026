# Introduction

La plateforme de simulation utilisée pour ce défi est [Gazebo Harmonic](https://gazebosim.org/docs/harmonic/install_ubuntu/){target=_blank}. Les équipes doivent développer, tester et soumettre un logiciel permettant de réaliser avec succès la navigation autonome du **CAYTU Sito-É** dans le restaurant, de sa position de départ à sa position d'arrivée.

Pour réaliser cette tâche, les équipes sont invitées à utiliser le framework de navigation [Nav2](https://docs.nav2.org/index.html){target=_blank}. Les liens suivants fournissent la documentation et les tutoriels nécessaires à la prise en main de Nav2.

* [Guide de démarrage de Nav2](https://docs.nav2.org/getting_started/index.html){target=_blank}
* [Jazzy - Niveau intermédiaire - Navigation ROS 2 (Nav2)](https://www.youtube.com/playlist?list=PLNWNEEf8BvG45noktLVI9N0SmD72BpmH7){target=_blank}

Les packages ROS 2 du **CAYTU Sito-É** et les modèles d'environnement Gazebo (voir description ci-dessous) sont mis à disposition des équipes pour leur permettre de développer et de tester leurs solutions (voir [Dépôt GitHub](https://github.com/PARC-Robotics/PARC2026-Engineers-League){target=_blank}).

### Le CAYTU Sito-É

Le **CAYTU Sito-É** est un véhicule terrestre sans pilote (UGV) équipé de différents capteurs pour vous aider à atteindre votre objectif. Ces capteurs sont les suivants :

* **RPLIDAR C1 :** Un capteur LiDAR situé sur le dessus de la base du robot. Le RPLIDAR C1 publie ses données sur le sujet `/scan`.

* **Caméras de profondeur D435i (x2) :** Une caméra est montée sous le robot et l’autre vers sa base. Ces caméras publient des données couleur sur les sujets `/top_camera_color/image_raw` et `/bottom_camera_color/image_raw`, ainsi que des données de nuage de points 3D sur `/top_camera_depth/points` et `/bottom_camera_depth/points`. Des sujets sont également dédiés aux images compressées, qui utilisent une bande passante inférieure à celle des images brutes standard. Concernant la caméra D435i supérieure, les sujets correspondants sont `/top_camera_color/image_raw/compressed` et `/top_camera_color/image_raw/theora`, des sujets similaires étant disponibles pour la caméra D435i inférieure.

* **IMU :** Un capteur IMU est ajouté à la caméra de base et publie ses données sur le sujet `/imu`.

La figure ci-dessous montre l'agrobot avec des capteurs étiquetés.

![robot](../assets/robot_sensor_label.png)


<!-- ### Environnement de simulation

L'environnement de simulation utilisé dans cette phase est modélisé comme une terre agricole réaliste avec un terrain accidenté et des plants de tomates fruitiers.

![simulation](../assets/world_description.png) -->
