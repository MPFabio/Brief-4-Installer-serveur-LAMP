# Brief-4-Installer-serveur-LAMP

# Livrables

1) Backup vault : les backups sont accessibles via le portail et le sont aussi à vos formateurs
2) Backup policy : les données sont sauvegardées 2 fois par jour : minuit et midi
3) Les données sont répliquées géographiquement 
4) Une documentation qui explique la démarche à suivre pour installer le linux et configurer les backup et l'installation du serveur web 
5) Un accès SSH avec certificat SSL. Le fichier de clé privée est disponible avec la documentation

# Critères de performance

Quiconque se trouvant en possession de la clé privée et du login associé peut se connecter en SSH au serveur : dangereux mais facile pour nous
Un deuxième disque est monté dans /mnt/data et contient les données de la base de données. Il ne doit pas dépasser 10 Go
Le port SSH de base (22) et le port 80 du serveur sont redirigés
BONUS : La base de données n'est pas sur un autre disque mais sur une autre VM Linux, sur le même réseau local mais non accessible depuis l'extérieur
