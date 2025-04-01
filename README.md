SYSCALL – Service Hardening et Seccomp
Objectif : appliquer des techniques de service hardening pour limiter les actions système qu'un programme peut exécuter (filtrage des syscalls via seccomp), et sécuriser une application vulnérable.

Observation du système d'appels système

Utilisation de stracepour tracer l'activité système d'un programme
Observation en situation normale et sous exploitation
Application de seccompvia systemd

Limitation des appels système autorisés dans un service
Analyse et adaptation du fichier .servicepour chaque cas
Cas pratique – sécurisation de NGINX

Installation et démarrage de NGINX
Traçage de son activité
Application d'un profil de filtrage des appels système viasystemd
Cas pratique – sécurisation d'une application vulnérable

Utilisation d'une calculatrice TCP vulnérable ( calc.py)
Création d'un servicecalculatrice.service
Exploitation de la vulnérabilité
Application du durcissement (droits, appels système )
Les fichiers de tracing et de service sont organisés dans les dossiers :

observe_files/
service_hardening_files/
shitty_app_files/
