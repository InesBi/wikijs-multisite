# Wiki.js Multi-Instance Platform

## Description
Infrastructure DevOps pour déployer plusieurs Wiki.js indépendants via Docker, Nginx et GitHub Actions.

## Structure du projet
- **instances/** : Contient un dossier par Wiki avec son docker-compose.yml
- **nginx/** : Fichier de configuration pour reverse proxy Nginx
- **.github/workflows/** : CI/CD GitHub Actions

## Déploiement
1. Pousser le code sur `main`
2. Le workflow CI déploie automatiquement sur le serveur
3. Accès :
   - http://wiki1.monplateforme.local
   - http://wiki2.monplateforme.local
   - http://wiki-public.monplateforme.local

## Configuration serveur
- Docker + Docker Compose
- Nginx installé et configuré
- Clé SSH configurée dans GitHub secrets
test 1 