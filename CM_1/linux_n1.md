---
marp: true
class:
  - invert
paginate: true
background: img/linux.png
---

![bg](img/linux.png)

# Formation Linux N1
## Into the shell
*2H - Florent Guillemette - Session 1/3*

---

![bg](img/linux.png)

# Qu'attendez-vous de cette formation ?

---

![bg](img/linux.png)

# Sommaire
- Histoire de Linux
- Introduction OS
- Les distributions
- La philosophie
- L’arborescence
- La ligne de commande
- Les permissions
- Les utilisateurs et l’administrateur
- TP

---

![bg](img/linux.png)

# Histoire
- Projet d’un étudiant (Linus Torvalds)
- 1991
- Philosophie très proche des systèmes Unix mais open-source
## Aujourd’hui
- Modulaire, Sécurisé, accessible (financièrement), …
- Serveur, Embarqué, Réseaux, IoT, …
- Des “variantes” pour tous les cas d’usages

---

![bg](img/linux.png)

# Introduction OS
Linux est le noyau (gestion des périphériques)
GNU est une couche applicative minimale (explorateur de fichier, interface avec le noyau, …)
GNU/Linux pour l’ensemble (OS)

---

![bg](img/linux.png)

# Les distributions 1/2

Les variantes de Linux sont appelées des distributions.
Il existe des distributions amateurs et professionnelles.

Distributions professionnelles (ou d’un niveau professionnel):
- RedHat (CentOS, Fedora, RockyLinux, …), Suse, Ubuntu, Debian, …

Distributions spécialisées :
- Kali Linux (pentest)

---

![bg](img/linux.png)

# Les distributions 2/2

Pourquoi RockyLinux ?
- Écosystème Red Hat 
- Dans le top 3 des systèmes utilisé dans les organisations
- Disponible dans l’interface d’OVH :) 

---

![bg](img/linux.png)

# La philosophie

<h2><center>Tout est fichier</center></h2>

Tous les éléments du système ont une représentation sous forme de fichier (Les partitions d’un disque, un terminal, la RAM, …)

---

![bg](img/linux.png)

# L’arborescence 1/4

Oubliez Windows !
La racine ( / ) est la base du système de fichier. 
Filesystem Hierarchy Standard (FHS)

---

![bg](img/linux.png)

# L’arborescence 2/4

image

---

![bg](img/linux.png)

# L’arborescence 3/4

Les HDD/SSD sont dans le répertoire /dev/xxx
Les supports de stockage “massif” = sdX (sda, sdb, sdc, …)
Les partitions seront suffixées par un numéro (sda1, sda2, sda3, …)

---

![bg](img/linux.png)

# L’arborescence 4/4

On n'écrit pas directement dans le fichier de partition.
Il faut “monter” (mount) la partition au système de fichier.
Par exemple, /home (espace utilisateur) peut être monté sur une partition différente du système. (/home = sdb1)
Il existe plusieurs systèmes de fichier sur Linux (EXT-2,3,4 ,XFS, ZFS, BtrsFS, …)
Vous pouvez mixer les FS en fonction de vos besoins. 

---

![bg](img/linux.png)

# La ligne de commande

La principale interface de Linux
Le bash désigne un interpréteur et un langage (.sh)
Les commandes built-in (cd, ls, …)
Les programmes externes (mkdir, …)

---

![bg](img/linux.png)

# La ligne de commande

<h2><center> commande option argument </center></h2>

<h2><center> ls -rtl /var/log </center></h2>

- Une commande (ls, mkdir, …)
- -s, -1, -a, --help, --verbose
- /chemin/dossier/fichier

---

![bg](img/linux.png)

# Gestion des permissions

Les commandes importantes :
* chmod pour changer les droits
* chown pour changer le propriétaire d’un fichier/dossier
* chgrp pour changer le groupe d’un fichier/dossier

---

![bg](img/linux.png)

# Les utilisateurs

* Un login (sans caractères spéciaux)
* Un mot de passe (mais ce n’est pas obligatoire)
* Un home (/home/<login>)
* La liste des utilisateurs dans /etc/passwd et /etc/shadow
* Un utilisateur est limité par défaut
* Une application peut s’exécuter dans un compte utilisateur


---

![bg](img/linux.png)

# L'administrateur

* un seul admin : root
* A tous les droits par défaut
* Travailler sous root n’est une bonne idée
* la commande sudo permet à un utilisateur de faire des commandes “root”

---

![bg](img/linux.png)

# Sortez le SSH
* login: padawan
* mdp: Secure!1
* Port: 22
* IP dans le discord
<h2><center> GL HF </center></h2>

