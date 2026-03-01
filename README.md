# ems-aw-cdtruck-sensors-meta

## Création des submodules git

1. Créer les dépôts (repositories) sur GitHub. Un pour le projet principal (meta, dans ce cas) et d'autres.

2. Cloner le projet principal :

```sh
    git clone git@github.com:mario1980miranda/ems-aw-cdtruck-sensors-meta.git
```

3. Créer un répertoire pour regrouper les sous-projets :

```sh
    mkdir microservices
```

4. Ajouter les autres projets en tant que sous-modules (submodules) :

```sh
    git submodule add git@github.com:mario1980miranda/ems-aw-cdtruck-sensors-device-management.git microservices/sensors-device-management
```

```sh
    git submodule add git@github.com:mario1980miranda/ems-aw-cdtruck-sensors-temperature-processing.git microservices/sensors-temperature-processing
```

5. Vérification : Git génère alors un fichier .gitmodules répertoriant les projets dans les dossiers spécifiés.

6. GitHub affichera les sous-projets sous forme de liens pointant vers leurs dépôts respectifs.
