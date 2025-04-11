⚠️ DTP Trunk Spoofing Attack Simulation Script

    Ce script est strictement à but pédagogique et ne doit être utilisé que dans un environnement de test isolé. Il permet de simuler une manipulation du protocole Dynamic Trunking Protocol (DTP) pour forcer une négociation de trunking entre des switches réseau.

❗ AVERTISSEMENT IMPORTANT
🚨 Interdiction d’usage sur des réseaux publics

Ce script modifie les paquets DTP (utilisés pour négocier des trunks VLAN) et peut perturber le fonctionnement des switches réseau en forçant des configurations non désirées. Utilisé sur des réseaux en production, il peut provoquer des interruptions de service, des erreurs de configuration ou des failles de sécurité.

⚠️ Son exécution en dehors d’un environnement local (lab, VM, réseau isolé) constitue une violation éthique et légale.

L’auteur de ce dépôt décline toute responsabilité en cas de mauvaise utilisation.
🎯 Objectif pédagogique

    Comprendre le fonctionnement de DTP (Dynamic Trunking Protocol) et la négociation de trunking VLAN.

    Simuler une manipulation DTP en envoyant des paquets modifiés pour forcer une négociation de trunking sur des switches réseau.

    Observer les effets d'une configuration incorrecte de trunking dans un environnement local.

📦 Dépendances

    Python 3.x

    Scapy

    DTP : Extension pour Scapy pour travailler avec DTP.

pip install scapy

🔧 Exécution du script

    Préparez l'environnement : Utilisez un réseau isolé ou un laboratoire virtuel dédié aux tests.

    Lancez le script :

    sudo python3 dtp_trunk_spoofing.py

Le script capture un paquet DTP, le modifie (adresse MAC et statut DTP), puis envoie ce paquet modifié sur le réseau pour simuler une attaque ou manipulation DTP.
