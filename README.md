# Lab-zabbix-pme

Lab Infrastructure PME Virtualisée + Supervision Zabbix
Projet personnel de mise en pratique des compétences en administration systèmes et réseaux.
Environnement entièrement virtualisé sous VMware Workstation.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Objectif
Concevoir et déployer une infrastructure réseau d'entreprise de A à Z, en reproduisant les conditions d'un environnement professionnel réel : contrôleur de domaine, gestion des utilisateurs et groupes, et supervision complète du parc avec alerting automatique.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Architecture

[Windows Server 2022]          [Debian 12 - Serveur Zabbix]
  - Active Directory (AD DS)     - Zabbix Server 7.4.8
  - DHCP                         - Supervision du parc
  - DNS                          
  - Domaine : zabbix.local
          |
    [VMware - Réseau 192.168.100.0/24]
          |
  [Windows 10 - technicien1]
    - Intégré au domaine
    - Agent Zabbix installé
    - Supervisé en temps réel

---
## Les 3 VMs

 <img width="484" height="150" alt="VM" src="https://github.com/user-attachments/assets/408e34b2-9215-4044-96ce-1d4c311fb3af" />


---

## Active Directory

Domaine : zabbix.local

OUs créées : Finance, Informatique, RH, Users

Utilisateurs créés : ilyes, finance, rh, technicien
<img width="1025" height="769" alt="Domaine" src="https://github.com/user-attachments/assets/3f55c069-b2ae-4c71-a6fc-2ee1b692005f" />


---

## Supervision Zabbix

Hôtes supervisés : technicien1 (Windows 10) + Zabbix server (Debian)

<img width="1028" height="768" alt="Hotes zabbix" src="https://github.com/user-attachments/assets/e60f71cc-21ba-4343-b618-836c2d1010ed" />

---

## Alerting - Détection d'incident

Simulation d'une panne sur technicien1 - Zabbix détecte automatiquement et génère une alerte.


<img width="1025" height="773" alt="probleme client" src="https://github.com/user-attachments/assets/d6dbeed4-6a7e-4f78-a4d9-1fcebd7a60a5" />

---

## Compétences

Windows Server 2022 - Active Directory - DHCP - DNS - VMware Workstation - Debian Linux - Zabbix 7.4.8 - Supervision réseau - Alerting

---

## Auteur

MAZOUZI Ilyes - Diplômé TSSR - En recherche d'alternance Bachelor ASR

ilyes.mazouzi1@gmail.com - Lens (62)

