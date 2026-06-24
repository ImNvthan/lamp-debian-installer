![Debian](https://img.shields.io/badge/Debian-11%2F12-red)
![Bash](https://img.shields.io/badge/Bash-Automation-blue)
![Status](https://img.shields.io/badge/status-working-green)

# 🚀 LAMP Debian Installer

Script Bash automatisé permettant de déployer rapidement un serveur LAMP sur Debian.

---

## 🎯 Objectif du projet

Automatiser l’installation d’une stack web complète afin de réduire le temps de configuration d’un serveur Linux :

- Apache2
- PHP (via dépôt Sury)
- MariaDB
- phpMyAdmin (optionnel)

---

## 🧠 Pourquoi ce projet ?

Ce projet simule un cas réel d’administration système :

- Déploiement rapide d’un serveur web
- Configuration automatique de services Linux

---

## ⚙️ Fonctionnalités

- Installation complète LAMP en une commande
- Support PHP version personnalisable
- Installation optionnelle de phpMyAdmin
- Configuration Apache automatique
- Activation PHP-FPM
- Option accès distant MariaDB
- Script idempotent

---

## 🖥️ Compatibilité
- Debian 11 / 12

---

## 🚀 Installation
```bash
git clone https://github.com/ImNvthan/lamp-debian-installer1.git
cd lamp-debian-installer1
chmod +x install-lamp.sh
sudo ./install-lamp.sh
```

🧪 Options disponibles
```bash
--no-phpmyadmin   # désactive phpMyAdmin
--remote-db       # autorise accès distant MariaDB
PHP_VERSION=8.3 ./install-lamp.sh
```

🔐 Sécurité (post-installation)
```bash
sudo mariadb-secure-installation
sudo rm /var/www/html/info.php
```
