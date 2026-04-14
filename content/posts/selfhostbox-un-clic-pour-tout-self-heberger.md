---
title: "SelfHostBox : un clic pour tout auto-héberger"
date: 2026-04-14
draft: false
tags: ["self-hosting", "docker", "devops", "projet"]
summary: "Pourquoi j'ai créé SelfHostBox, une plateforme qui rend le self-hébergement accessible à tous en un clic."
---

## Le constat

L'auto-hébergement, c'est un peu le Graal de l'indépendance numérique. Ne plus dépendre de Google pour ses fichiers, d'Apple pour ses photos, de LastPass pour ses mots de passe — reprendre le contrôle de ses données, c'est un sentiment puissant.

Mais la réalité, c'est que c'est pénible.

Chaque app a son docker-compose, sa configuration, ses variables d'environnement, son reverse proxy, ses certificats SSL. Déployer Nextcloud + Vaultwarden + Jellyfin sur le même serveur ? Tu passes plus de temps dans les fichiers YAML qu'à utiliser les apps elles-mêmes.

J'ai vu des collègues, des amis, des gens bien plus compétents que la moyenne, abandonner l'idée d'auto-héberger parce que la barrière d'entrée était trop haute. Et ça m'a dérangé.

## L'idée

**SelfHostBox** — un clic, et c'est déployé.

Une interface web où tu choisis une app, tu cliques sur "Deploy", et 30 secondes plus tard tu as une instance fonctionnelle avec HTTPS, backups automatiques, et mises à jour programmées. Pas de YAML à écrire, pas de certificat à générer à la main, pas de reverse proxy à configurer.

Le tout basé sur Docker et Traefik — des outils qu'on connaît, qu'on maîtrise, et qui marchent.

## Ce que ça fait

- **20+ apps** disponibles : Nextcloud, Vaultwarden, Jellyfin, Gitea, Pi-hole, Home Assistant, Paperless, et d'autres
- **SSL automatique** via Let's Encrypt et Traefik
- **Backups quotidiens** — local ou S3
- **Mises à jour automatiques** (optionnel)
- **Monitoring** — CPU/RAM par app
- **Multi-utilisateur** avec permissions
- **Domaines personnalisés** ou sous-domaines auto-générés

## Pourquoi je l'ai construit

Parce que j'en avais marre de refaire la même config à chaque fois. Parce que le self-hébergement devrait être aussi simple qu'installer une app sur son téléphone. Parce que l'indépendance numérique ne devrait pas être réservée à ceux qui savent écrire un docker-compose.

Et honnêtement ? Parce que c'est un projet qui me permet de mettre en pratique tout ce que j'aime : Docker, automatisation, infra as code, et UX. Construire un outil qui rend un truc compliqué accessible, c'est ce qui me motive.

## Pour qui ?

- **Tu veux ton propre cloud** sans prendre 3 jours à configurer Nextcloud ? SelfHostBox.
- **Tu veux un gestionnaire de mots de passe** sans payer 1Password ? Un clic.
- **Tu veux du streaming** pour ta famille ? Jellyfin en 30 secondes.
- **Tu es freelance** et tu setup des infras self-hébergées pour tes clients ? C'est fait pour ça aussi.

## La suite

Le projet est open source, en Python + Docker, et je continue à ajouter des apps et améliorer l'interface. Si tu veux tester, contribuer, ou juste voir le code :

👉 [github.com/Mounik/SelfHostBox](https://github.com/Mounik/SelfHostBox)

Et si t'as des questions, hésite pas — je suis pas loin.