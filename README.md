# Network-NAT-RIP
Travail personnel que j'ai trouvé et que j'ai voulu faire.

Objectifs
▪ Mettre en place du NAT sur deux sites distants « W » et « Z » qui communiquent via un
réseau public de routeurs et qui sont dotés du même plan d’adressage en 192.168.0.0/24.
▪ Mettre en place du routage dynamique dans un réseau de routeurs et mettre en évidence
la tolérance de panne.
▪ Mettre en place du NAT Statique pour permettre l’accès extérieur à un serveur privé

Le schéma comporte 4 sites. Les deux sites d’extrémité W et Z utilisent le même réseau
192.168.0.0/24. On peut assimiler ces deux sites à des particuliers dotés d’une « box ». Sur le
site X, un réseau 172.11.0.0/24 comporte un serveur Web Serv-X d’adresse 172.11.0.1. Sur le
site Y, un autre serveur Web (Serv-Y) est accessible à l’adresse 172.12.0.1 sur le réseau
172.12.0.0/24.

Conséquence :
Le protocole RIP n’est pas utilisable sur les sites terminaux W et Z, du fait de l’utilisation du
même réseau IP par ces deux sites.
