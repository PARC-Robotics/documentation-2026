# Introduction

## Défi de Navigation

La plateforme de simulation utilisée pour ce parcours est [Gazebo Harmonic](https://gazebosim.org/docs/harmonic/install_ubuntu/). Les équipes doivent développer, tester et soumettre un logiciel pour piloter de manière autonome **CAYTU Sito-É** dans les champs de maïs.

Les packages ROS 2 du **CAYTU Sito-É** et les modèles d'environnement Gazebo (voir description ci-dessous) sont mis à disposition des équipes pour leur permettre de développer et de tester leurs solutions (voir [Dépôt GitHub](https://github.com/PARC-Robotics/PARC2026-Engineers-League)).

### Le CAYTU Sito-É

Le **CAYTU Sito-É** est un véhicule terrestre sans pilote (UGV) équipé de différents capteurs pour vous aider à atteindre vos objectifs. Ces capteurs sont :

* **RPLIDAR C1:** Un capteur lidar situé en haut de la base du robot. Le RPLIDAR C1 publie le sujet `/scan`.

* **RGB Camera (x2):** Deux caméras RVB latérales sont installées à gauche et à droite du robot. Suspendues à un surplomb, elles offrent une vue aérienne des terres agricoles. Les sujets publiés par ces caméras sont nommés « /left_camera/ » et `/right_camera/`.

* **ZED 2i Camera:** Il s'agit d'une caméra stéréo située à l'avant de la base du robot. Elle publie tous les sujets `/zed2/`, y compris les données de nuages ​​de points (`/zed2/point_cloud/cloud_registered`).

* **IMU :** Un capteur IMU est ajouté à la base et publié sur le sujet `/imu`.

La figure ci-dessous montre l'agrobot avec des capteurs étiquetés.

![robot](../assets/robot_sensor_label.png)


<!-- ### Environnement de simulation

L'environnement de simulation utilisé dans cette phase est modélisé comme une terre agricole réaliste avec un terrain accidenté et des plants de tomates fruitiers.

![simulation](../assets/world_description.png) -->
