# Description

Le Dockerfile "package" l'application dans une image intégrant serveur web et d'application.

Le fichier docker-compose.yml rend disponible l'application et son serveur de base de données en une seule commande.  
Il fait appel à des volumes pour permettre la mise à jour de l'application en temps réel, typiquement pour un usage sur une station de développement, et l'installation automatique de la base via des scripts sql à fournir dans le répertoire prévu à cet effet.

# Amélioration

- Serveurs web et d'application sont découplés via deux images distinctes.
- Celles-ci sont créées par un processus d'intégration continue.
- Les images sont déployées à l'aide d'un orchestrateur.
- "config" et "secrets" sont utilisés en fonction des paramètres.