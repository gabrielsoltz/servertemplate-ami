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
6. CONFIGURACION IP DINAMICA ACTUAL COMO FIJA.
7. SETEAR MOTD
8. AJUSTES SYSCTL
9. AJUSTES MODPROBE
10. DESACTIVAR IPV6
11. SSHD_CONFIG
	- CREAR GRUPO SSH
	- SETEAR PASSWORD ROOT
	- CREAR USUARIO ADMIN
	- SETEAR PASSWORD ADMIN
	- CREAR CERTS ADMIN
	- CONFIGURAR SUDOERS ADMIN
	- CONFIGURAR BASHRC PS1
12. INSTALACIÓN DE CLOUDWATCH
13. ELIMINAR USUARIO EC2-USER Y SU CONFIGURACION EN SUDOERS.
14. REBOOT