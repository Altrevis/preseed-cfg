# README - Installation Automatisée Debian

## Description
Ce fichier de préconfiguration permet une installation automatisée de Debian avec des paramètres définis, incluant la langue, la disposition du clavier, la configuration réseau, le partitionnement du disque, la création d'utilisateurs et l'installation de logiciels.

## Configuration
### Localisation
- Langue : Français (fr_FR)
- Clavier : AZERTY (fr)
- Fuseau horaire : Europe/Paris

### Réseau
- Connexion Wi-Fi configurée avec PEAP
- SSID : `votre wifi`
- Type de sécurité : WPA (PEAP)
- Nom d'utilisateur : `votre adresse mail`
- Mot de passe : `votre mot de passe`
- Vérification du certificat : Désactivée

### Dépôts Debian
- Miroir Debian : `ftp.fr.debian.org`
- Proxy HTTP : Aucun

### Partitionnement
- Disque ciblé : `/dev/sda`
- Méthode de partitionnement : Standard
- Installation du chargeur de démarrage GRUB sur `/dev/sda`

### Utilisateurs
- Root
  - Mot de passe : `admin`
  - Mot de passe faible autorisé
- Utilisateur standard
  - Nom d'utilisateur : `user1`
  - Mot de passe : `pass1`
  - Mot de passe faible autorisé
  - Chiffrement du dossier personnel activé

### Logiciels installés
- `openssh-server` (pour l'accès distant SSH)
- `htop` (outil de surveillance des processus)

### Personnalisation
- Création automatique d'un fichier `/home/helloworld.txt`

## Utilisation
Ce fichier doit être utilisé lors d'une installation automatisée de Debian avec `preseed`. Assurez-vous de le charger correctement dans l'installeur pour appliquer ces paramètres automatiquement.

## Avertissement
⚠ **Ce programme n'est utilisable que pour du debian 12, et il est important de sauvegarder vos donné si vous l'utilisé sur votre machine directement pour éviter une suppression total de vos donnée**

