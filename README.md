# 🚀 LAMP Debian Installer

![Debian](https://img.shields.io/badge/Debian-11%2F12-red)
![Bash](https://img.shields.io/badge/Bash-Automation-blue)
![Status](https://img.shields.io/badge/status-working-green)

---

## 🎯 Objectif du projet

Ce script automatise le déploiement d’un serveur web LAMP sur Debian.

Il permet de transformer un serveur vierge en environnement prêt à héberger des applications web.

---

## 🧠 Contexte

Ce projet a été réalisé dans une logique d’administration système :

- Automatisation d’infrastructure Linux
- Déploiement de services web
- Configuration serveur (Apache, PHP, MariaDB)
- Gestion d’options via CLI

---

## 🛠️ Méthodologie

Ce projet a été construit à partir d’une documentation technique décrivant l’installation manuelle d’un serveur LAMP sur Debian.

Cette procédure a ensuite été automatisée en script Bash, testée et adaptée sur environnement Debian (VM).

---

## ⚙️ Stack installée

- Apache2
- PHP (via dépôt Sury)
- MariaDB
- phpMyAdmin (optionnel)

---

## 🚀 Installation

```bash
git clone https://github.com/ImNvthan/lamp-debian-installer.git
cd lamp-debian-installer
chmod +x install-lamp.sh
sudo ./install-lamp.sh
```

🧪 Options disponibles
```bash
--no-phpmyadmin
--remote-db
PHP_VERSION=8.3 ./install-lamp.sh
```
🔐 Sécurité post-installation
```bash
sudo mariadb-secure-installation
sudo rm /var/www/html/info.php
```

## 🖥️ Résultat après installation
- Serveur web accessible sur port 80
- PHP opérationnel
- Base de données MariaDB active
- Interface phpMyAdmin (si activée)
