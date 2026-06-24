# 🚀 LAMP Debian Installer

Script Bash automatisé pour installer un serveur LAMP sur Debian.

## 🎯 Objectif
Automatiser une stack web complète :
- Apache2
- PHP (Sury)
- MariaDB
- phpMyAdmin

## ⚙️ Fonctionnalités
- Installation automatique complète
- PHP version configurable
- phpMyAdmin optionnel
- Accès distant MariaDB (option)
- Script idempotent

## 🚀 Installation
```bash
git clone https://github.com/ImNvthan/lamp-debian-installer1.git
cd lamp-debian-installer1
chmod +x install-lamp.sh
sudo ./install-lamp.sh

## 🧪 Options
```bash
--no-phpmyadmin
--remote-db
PHP_VERSION=8.3 ./install-lamp.sh

## 🔐 Sécurité
sudo mariadb-secure-installation
sudo rm /var/www/html/info.php
