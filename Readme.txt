
########################################################## voici les étapapes pour ce lab ##############################################################""

1. Choisissez entre VirtualBox ou VMware selon votre préférence, puis installez-le.
2. Installez un Windows Server (nous avons utilisé Windows Server 2019 pour cet exemple) dans la machine virtuelle. 
Assurez-vous que le Windows Server dispose de deux interfaces réseau : une interface publique pour la connexion à Internet et une interface locale.
3. Installez AD DS (Active Directory Domain Services) sur le Windows Server 2019 et promouvez-le en tant que contrôleur de domaine.
4. Ajoutez le rôle RAS/NAT (Remote Access Service/Network Address Translation) pour permettre aux clients de se connecter à Internet.
5. Ajoutez le rôle DHCP à l'interface locale du serveur pour permettre l'attribution automatique des adresses IP aux nouveaux clients.
6. Ajoutez des utilisateurs, en veillant à inclure au moins un utilisateur dans le groupe d'administrateurs du domaine.
7. Installez Windows 10 dans une autre machine virtuelle, puis rejoignez-le au domaine créé précédemment.


                             #######################################################################
														 Pour approfondir davantage, nous allons explorer quelques techniques d'énumération 
														 post-exploitation.
														 Nous supposerons que nous avons obtenu récemment des identifiants suite à 
														 une attaque de phishing ou à une phase de reconnaissance
														 ########################################################################
														 
														 
														 8. Installez un autre client Windows 10, sans le rejoindre au domaine.
														 9. Installez une machine Linux. Ces deux machines seront utilisées en tant qu'attaquants.
														 10. Utilisez la commande "runas" sur Windows pour injecter les identifiants volés dans la mémoire de la machine Windows attaquante. 
														 Assurez-vous d'ajouter la fonctionnalité RSAT (Remote Server Administration Tools) comprenant Active Directory Domain Services et Lightweight Directory Tools 
														 sur la machine Windows attaquante.
														 11. Utilisez la console MMC (Microsoft Management Console) pour effectuer l'énumération des informations.
														 12. Utilisez Bloodhound, un outil d'énumération, sur la machine Kali Linux pour obtenir davantage d'informations.
														 
