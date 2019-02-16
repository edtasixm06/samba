# SAMBA
## @edt ASIX M06 2018-2019


Podeu trobar les imatges docker al Dockehub de [edtasixm06](https://hub.docker.com/u/edtasixm06/)

Podeu trobar la documentació del mòdul a [ASIX-M06](https://sites.google.com/site/asixm06edt/)

ASIX M06-ASO Escola del treball de barcelona

### Imatges:

* **edtasixm06/samba:18base** Servidor SAMBA bàsic amb *shares* d'exemple.

* **edtasixm06/samba:18users** Servidor bàsic de samba amb *shares* d'exemple per practicar accés autenticat als
shares, permisos de lectura/escriptura i modes.

* **edtasixm06/samba:18ldapusers** Servidor SAMBA amb usuaris locals i usuaris LDAP (unix). Es creen comptes d'usuari
samba d'usuaris locals i d'alguns dels usuaris ldap (no tots). Es creen també els directoris home dels usuaris de ldap 
i se'ls assigna la pripietat/grup pertinent. Finalment s'exporten els shares d'exemple usuals i els **[homes]** dels 
usuaris samba. D'aquesta manera un hostpam (amb ldap) pot muntar els homes dels usuaris (home dins home) usant samba.

* **edtasixm06/samba:18detach** Versió de samba:18ldapusers amb un bucle *cutre* per poder deixar-lo detach.
	
* **edtasixm06/samba:18ldapsam** Servidor SAMBA amb backend LDAP ldapsam. Requereix de l'ús de un servidor ldap preparat
amb l'schema samba. Les dades dels usuaris samba es desen en els comptes d'usuari ldap.


