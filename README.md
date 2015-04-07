Server Template AMI

Script en Bash para estandarizar Sistemas Amazon Images (AMI).
Fué realizado para ejecutar previo a la instalación de los servicios productivos de cada servidor. 
Realiza control de errores en cada uno de sus funcionalidades. Todo lo realizado se loguea en $LOG.

Para Ejecutar: ./servertemplate-ami.sh [HOSTNAME]

Funcionalidades:

1. UPGRADE SISTEMA
2. ELIMINAR PAQUETES: Desintalación de Paquetes no necesarios
3. DESACTIVAR SERVICIOS: Desactivación de Serivicios al Inicio no necesarios
4. ZONEDATE: Eliminar Paquete NTP y Setear Zona Horaria.
5. SETEAR HOSTNAME
6. SETEAR AMAZON TAGS
7. CONFIGURACION IP DINAMICA ACTUAL COMO FIJA.
8. SETEAR MOTD
9. AJUSTES SYSCTL
10. AJUSTES MODPROBE
11. DESACTIVAR IPV6
12. SSHD_CONFIG
	- CREAR GRUPO SSH
	- SETEAR PASSWORD ROOT
	- CREAR USUARIO ADMIN
	- SETEAR PASSWORD ADMIN
	- CREAR CERTS ADMIN
	- CONFIGURAR SUDOERS ADMIN
	- CONFIGURAR BASHRC PS1
13. INSTALACIÓN DE CLOUDWATCH
14. ELIMINAR USUARIO EC2-USER Y SU CONFIGURACION EN SUDOERS.
15. REBOOT