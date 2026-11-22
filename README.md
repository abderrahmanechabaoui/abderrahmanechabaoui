<div align="center">

# Abderrahmane Chabaoui

**Élève ingénieur · Électromécanique & Digitalisation Industrielle · ENSAM Meknès**

Cybersécurité industrielle (OT) · Supervision SCADA · Automatisme · IIoT

[![Portfolio](https://img.shields.io/badge/Portfolio-1F5FBF?style=flat-square&logo=githubpages&logoColor=white)](https://abderrahmanechabaoui.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abderrahmane-chabaoui)
[![Email](https://img.shields.io/badge/Email-333333?style=flat-square&logo=gmail&logoColor=white)](mailto:abderrahmanechabaoui@gmail.com)
![Localisation](https://img.shields.io/badge/Casablanca,_Maroc-555555?style=flat-square)

</div>

> **Disponibilité** : je recherche un **stage de fin d'études (PFE) de 6 mois à partir de février 2027** en cybersécurité industrielle, SCADA ou automatisme.

---

## Profil

Élève ingénieur en Électromécanique et Digitalisation Industrielle, je travaille à l'interface entre le procédé industriel et les systèmes numériques. Mon expérience porte sur la collecte et la valorisation des données industrielles (OPC UA, MQTT, séries temporelles), la supervision (WinCC, FactoryTalk View SE) et la conception d'architectures OT sécurisées selon les principes de l'IEC 62443.

**Objectif** : contribuer à rendre les installations industrielles plus performantes, plus fiables et plus sûres.

---

## Domaines d'expertise

| Domaine | Compétences clés |
|---|---|
| **Cybersécurité OT** | Défense en profondeur, segmentation en zones et conduits, DMZ industrielle, cartographie des risques, sécurisation OPC UA et Modbus, notions IEC 62443 |
| **Automatisme & supervision** | Siemens S7-1200, TIA Portal, WinCC, FactoryTalk View SE, KEPServerEX, régulation PID |
| **IIoT & Industrie 4.0** | Node-RED, MQTT, InfluxDB, Grafana, jumeaux numériques, AAS, RAMI 4.0 |
| **Données & programmation** | Python (Pandas, OpenCV, FastAPI), C/C++, SQL, régression linéaire, Docker, ROS 2, Linux |

---

## Expérience professionnelle

### OCP Jorf Lasfar · Stagiaire IIoT et digitalisation industrielle
*Juillet 2026 – Septembre 2026 · Projet de fin d'année*

**Contexte** : station terminale du pipeline de pulpe de phosphate Khouribga – Jorf Lasfar (187 km).

**Réalisations** · *code disponible sur demande*
- **Capteur virtuel de densité** (régression linéaire multiple, validation Leave-One-Out) qui estime la densité de la pulpe à partir du courant de l'agitateur, du niveau et de la température.
- **Prédiction du temps avant débordement (TTO)** par régression sur fenêtre glissante, avec trois niveaux de risque.
- Modèles déployés dans un **microservice FastAPI**, découplé de l'orchestration Node-RED.
- **Chaîne IIoT conteneurisée** (Docker Compose) : OPC UA, Node-RED, InfluxDB, Grafana. Validée sur un bac pilote avec un simulateur OPC UA en Python.
- Étude de l'architecture de supervision **Rockwell FactoryTalk View SE** (HMI Server, FactoryTalk Linx, Historian).

```mermaid
flowchart LR
  A[Simulateur OPC UA<br/>Python] --> B[KEPServerEX]
  B --> C[Node-RED]
  C <--> F[FastAPI<br/>soft sensor + TTO]
  C --> D[InfluxDB]
  D --> E[Grafana]
```

**Technologies** : Python · OPC UA · KEPServerEX · Node-RED · FastAPI · Docker · InfluxDB · Grafana · FactoryTalk View SE

### Sofimed Maroc · Stagiaire instrumentation
*Juillet 2025 – Septembre 2025 · Stage d'initiation*

- Analyse et étude du fonctionnement du calculateur **Multiload II+**, utilisé sur les skids de chargement et de déchargement de GPL.

---

## Projets sélectionnés

| Dépôt | Description |
|---|---|
| **slurry-tank-digital-twin** *(privé, sur demande)* | Capteur virtuel de densité et prédiction de débordement : OPC UA, FastAPI, Node-RED, InfluxDB, Grafana, Docker |
| [**pv-digital-twin-opcua**](https://github.com/abderrahmanechabaoui/pv-digital-twin-opcua) | Jumeau numérique photovoltaïque : Simulink temps réel, KEPServerEX, Node-RED, analyse RAMI 4.0 |

### Architecture de cybersécurité d'un système industriel
*2026 – 2027 · Matériel et logiciel*

| Étape | Travail réalisé |
|---|---|
| Inventaire | Recensement des équipements (automates, SCADA/HMI) et des flux de communication |
| Analyse de risques | Cartographie des risques OT |
| Segmentation | Découpage du réseau en zones et conduits, filtrage des échanges |
| Défense en profondeur | Contrôle des accès, durcissement des postes |
| Protocoles | Sécurisation d'OPC UA (authentification, chiffrement) et de Modbus |

```mermaid
flowchart TB
  IT[Zone Entreprise - IT] -->|Pare-feu| DMZ[DMZ industrielle]
  DMZ -->|Pare-feu| SUP[Supervision - SCADA/HMI, OPC UA]
  SUP -->|Conduit filtré| CTL[Contrôle - Automates S7-1200]
  CTL --> FLD[Terrain - Modbus RTU, Profibus DP]
```

### Autres projets

| Projet | Période | Description | Technologies |
|---|---|---|---|
| **Supervision industrielle & passerelle IoT** | 2025 – 2026 | Programmation d'un automate S7-1200, écrans WinCC (conduite, états, alarmes), passerelle Node-RED vers le stockage et les tableaux de bord | TIA Portal, WinCC, Node-RED |
| **BMS pour batterie Li-ion** | 2026 – 2027 | Mesure des tensions, du courant et des températures, équilibrage des cellules, protections surcharge et décharge profonde, surveillance thermique | Électronique de puissance |
| **[Jumeau numérique photovoltaïque](https://github.com/abderrahmanechabaoui/pv-digital-twin-opcua)** | 2025 – 2026 | Modèle Simulink temps réel relié en OPC UA (KEPServerEX) à une IHM Node-RED en boucle fermée, et analyse RAMI 4.0 du système | MATLAB/Simulink, OPC UA, Node-RED |
| **Refroidissement d'un module batterie VE** | 2025 – 2026 | Modélisation de l'échauffement des cellules Li-ion et simulation du refroidissement du pack | Simulation thermique |

---

## Compétences techniques

| Catégorie | Outils et technologies |
|---|---|
| Automates & SCADA | ![S7-1200](https://img.shields.io/badge/Siemens_S7--1200-009999?style=flat-square&logo=siemens&logoColor=white) ![TIA Portal](https://img.shields.io/badge/TIA_Portal-009999?style=flat-square) ![WinCC](https://img.shields.io/badge/WinCC-009999?style=flat-square) ![FactoryTalk](https://img.shields.io/badge/FactoryTalk_View_SE-B22222?style=flat-square) ![KEPServerEX](https://img.shields.io/badge/KEPServerEX-1F4E79?style=flat-square) |
| Protocoles industriels | ![OPC UA](https://img.shields.io/badge/OPC_UA-444444?style=flat-square) ![Modbus](https://img.shields.io/badge/Modbus_RTU%2FRS--485-444444?style=flat-square) ![Profibus](https://img.shields.io/badge/Profibus_DP-444444?style=flat-square) ![MQTT](https://img.shields.io/badge/MQTT-660066?style=flat-square&logo=mqtt&logoColor=white) |
| IIoT & données | ![Node-RED](https://img.shields.io/badge/Node--RED-8F0000?style=flat-square&logo=nodered&logoColor=white) ![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=flat-square&logo=influxdb&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |
| Programmation | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![C++](https://img.shields.io/badge/C%2FC++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-E95420?style=flat-square&logo=ubuntu&logoColor=white) |
| Embarqué | ![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white) ![Arduino](https://img.shields.io/badge/Arduino-00878F?style=flat-square&logo=arduino&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white) ![Jetson](https://img.shields.io/badge/NVIDIA_Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white) |
| Simulation & CAO | ![MATLAB](https://img.shields.io/badge/MATLAB%2FSimulink-0076A8?style=flat-square&logo=mathworks&logoColor=white) ![CATIA](https://img.shields.io/badge/CATIA-005386?style=flat-square) ![AutoCAD](https://img.shields.io/badge/AutoCAD-E51050?style=flat-square&logo=autodesk&logoColor=white) ![Ansys](https://img.shields.io/badge/Ansys-FFB71B?style=flat-square&logo=ansys&logoColor=black) |
| Énergie | BMS · gestion thermique des batteries · photovoltaïque · électronique de puissance · schémas électriques |

---

## Formation

| Période | Établissement | Diplôme |
|---|---|---|
| 2024 – présent | École Nationale Supérieure d'Arts et Métiers (ENSAM), Meknès | Cycle ingénieur · Génie Électromécanique et Digitalisation Industrielle |
| 2022 – 2024 | ENSAM Meknès | Années préparatoires intégrées |
| 2022 | Lycée En-nasr, Casablanca | Baccalauréat Sciences Physiques |

---

## Certifications

| Certification | Organisme |
|---|---|
| Introduction to Cybersecurity | Cisco Networking Academy |
| Networking Basics | Cisco Networking Academy |
| KICKOFF Predictive Badge (gestion de projet) | PMI |

## Langues

**Arabe** : langue maternelle · **Français** : C1 (certifié TCF) · **Anglais** : courant

## Engagement associatif

- **Chef Média**, Club Robotique Arts et Métiers (CRIAM), 2025 – 2026
- Membre actif : Club Robotique, Events, Caravane Al Hayat, 2022 – 2026

---

<div align="center">

**Contact** · [abderrahmanechabaoui@gmail.com](mailto:abderrahmanechabaoui@gmail.com) · [LinkedIn](https://www.linkedin.com/in/abderrahmane-chabaoui) · [Portfolio](https://abderrahmanechabaoui.github.io)

</div>
