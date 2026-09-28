# Infrastructure réseau virtualisée — Active Directory, DNS, DHCP

Projet réalisé dans le cadre d'un TP noté en BTS SIO, option SISR.

## Contexte

Ce projet consiste à concevoir et déployer une infrastructure réseau fonctionnelle, entièrement virtualisée sous VMware (ESXi / Workstation), reproduisant les conditions d'un environnement professionnel d'administration systèmes et réseaux.

## Objectifs

- Centraliser la gestion des utilisateurs et des ressources via un service d'annuaire.
- Automatiser l'attribution d'adresses IP sur le réseau.
- Mettre en place une résolution de noms fiable entre les machines.
- Intégrer des postes clients à un domaine géré de façon centralisée.

## Environnement technique

| Élément | Détail |
|---|---|
| Hyperviseur | VMware ESXi / Workstation |
| Système serveur | Windows Server |
| Services déployés | Active Directory, DNS, DHCP |
| Postes clients | Machines virtuelles jointes au domaine |

## Architecture

*(Insère ici un schéma de ton infrastructure : serveur AD/DNS/DHCP, plan d'adressage, postes clients, éventuellement les VLAN si tu en as utilisé.)*

## Mise en œuvre

1. Installation et configuration du serveur Windows Server.
2. Déploiement du rôle Active Directory Domain Services et création du domaine.
3. Configuration du service DNS pour la résolution de noms interne.
4. Configuration du service DHCP pour l'attribution automatique des adresses IP.
5. Jonction des machines virtuelles clientes au domaine Active Directory.
6. Tests de validation : authentification des utilisateurs, attribution DHCP, résolution DNS.

## Difficultés rencontrées

La principale difficulté a été de centraliser et de relier l'ensemble des services (annuaire, DNS, DHCP, postes clients) sur une seule machine serveur, en veillant à ce que chaque composant communique correctement avec les autres sans conflit de configuration. Cela a nécessité de bien comprendre l'ordre d'installation des rôles et les dépendances entre services pour obtenir une infrastructure cohérente et stable.

## Compétences mobilisées

- Virtualisation d'infrastructure (VMware)
- Administration Windows Server
- Configuration et gestion d'Active Directory
- Configuration des services DNS et DHCP
- Diagnostic et résolution de problèmes réseau

## Conclusion

Ce projet a permis de mettre en pratique des compétences d'administration systèmes et réseaux dans un environnement proche de la réalité professionnelle, et de mieux comprendre l'articulation entre les différents services d'une infrastructure (annuaire, DNS, DHCP).

## Documents

- 📄 [Rapport de projet](./Rapport%20de%20projet.docx)
- 📘 [Documentation technique](./Documentation.pdf)
- 🎥 [Vidéo de démonstration](https://www.youtube.com/watch?v=Hnd-Le4G3Pk)

