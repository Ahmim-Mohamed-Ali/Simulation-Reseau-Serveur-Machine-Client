# Simulation-Reseau-Serveur-Machine-Client
Gestionnaire de calculs de persistances distribués sur plusieurs machines en utilisant le réseau et les sockets

# Projet Description

Le projet « Distributed Computation of Persistence » vise à développer un outil de gestion d'un réseau de machines. Le réseau se compose de trois groupes principaux de machines : les travailleurs, les serveurs et les clients.

### Worker
Les Workers sont responsables de l'exécution des calculs. Ils reçoivent des tâches par le serveur les exécutent, produisant des résultats de calcul.

### Server 
Les serveurs reçoivent les résultats des calculs des travailleurs et gèrent leur organisation et leur stockage. Les résultats peuvent être stockés soit en RAM, soit sur disque dur. De plus, les serveurs peuvent effectuer des statistiques sur les résultats qui sont stockés.

### Clients
Les clients font partie du réseau et peuvent se connecter aux serveurs. 
Ils ont accès à la base de données maintenue par les serveurs, ce qui leur permet d'interroger des plages de résultats spécifiques et de demander divers types de statistiques aux serveurs.

# Projet Structure

### client
Ce dossier contient le code du logiciel client. Il fournit les fonctionnalités nécessaires pour se connecter aux serveurs et accéder à la base de données.
Les clients peuvent interroger les résultats et demander des statistiques aux serveurs.

### config
Le dossier de configuration contient les fichiers de configuration et les paramètres de l'ensemble du système. Il comprend tous les fichiers de configuration nécessaires pour les travailleurs, les serveurs et les clients.

### server
Le dossier du serveur contient le code du logiciel serveur. Il reçoit les résultats des calculs des travailleurs, les stocke de manière appropriée (dans la RAM ou sur disque) et effectue des statistiques sur les résultats.

### Test
Le dossier de tests comprend des cas de test et des tests unitaires pour le projet. Il garantit l'exactitude et la fiabilité de la fonctionnalité implémentée.

### Worker 
Le dossier Worker contient le code du logiciel Worker. Il gère les calculs requis par le projet. Chaque travailleur exécute les tâches assignées et produit des résultats de calcul.

# Installation Et Configuration
Pour utiliser le projet « Calcul distribué de persistance », procédez comme suit :

1.Clonez le référentiel du projet depuis GitHub.
2.Installez Java sur votre ordinateur s'il n'est pas déjà installé.
3.Configurez le projet en modifiant les paramètres et les fichiers de configuration nécessaires dans le dossier de configuration.
4.Compilez les fichiers source Java dans chaque package à l'aide d'un compilateur Java.
5.Exécutez les composants nécessaires sur les machines désignées comme travailleurs, serveurs et clients.
