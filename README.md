#  Déploiement Automatisé de Machines Virtuelles dans vCenter

##  Description

Ce projet permet de **déployer automatiquement des machines virtuelles** (VMs) dans un environnement VMware vSphere à l'aide de scripts Python. Il réduit les interventions manuelles, évite les erreurs humaines, et standardise le processus de déploiement à partir de templates.

##  Objectif

> Automatiser le processus de création, configuration et mise en service de VMs dans vCenter.

---

##  Arborescence du Projet
```bash
vm-deployment/
├── config/
│ └── vm-config.json # Fichier de configuration principal
├── scripts/
│ ├── deploy-vm.py # Script principal de déploiement
│ └── functions.py # Fonctions utilitaires
├── templates/
│ └── vm-template-config.json # Configuration spécifique des templates
├── logs/
│ └── deployment.log # Fichiers de journalisation
├── requirements.txt # Bibliothèques Python nécessaires
├── install.py # Script d'installation automatisée
└── README.md # Documentation (ce fichier)

```


---

##  Prérequis

- Python **3.6 ou supérieur**
- Accès à un serveur **VMware vCenter**
- Droits suffisants pour créer des VMs
- Templates de VM existants dans vSphere
- Connexion réseau au vCenter

---

##  Installation

### 1. Cloner le projet
```bash
git clone https://github.com/ton-utilisateur/vm-deployment.git
cd vm-deployment
```



---

##  Prérequis

- Python **3.6 ou supérieur**
- Accès à un serveur **VMware vCenter**
- Droits suffisants pour créer des VMs
- Templates de VM existants dans vSphere
- Connexion réseau au vCenter

---

##  Installation

### 1. Cloner le projet
```bash
git clone https://github.com/ton-utilisateur/vm-deployment.git
cd vm-deployment
```


### 2. Lancer le script d'installation
```bash
python install.py
```
Ce script :

    Vérifie votre version de Python

    Installe les dépendances via requirements.txt

    Crée les dossiers nécessaires

    Vérifie la présence des fichiers de configuration



##  Utilisation
Déploiement d'une VM
```bash
python scripts/deploy-vm.py
```

## Étapes effectuées :
```bash
    Connexion sécurisée à vCenter

    Vérification des ressources

    Clonage de la VM

    Configuration (CPU, RAM, disque)

    Connexion réseau

    Démarrage (optionnel)

```
##  Logs
```bash
Tous les événements sont enregistrés dans le dossier logs/ avec des fichiers datés.

```
##  Auteurs
```bash
    Hasna Daoui

    Nana Diawara
```


