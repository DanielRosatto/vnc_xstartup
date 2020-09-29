## vnc_xstartup v0.1

Unix script basado en Xvfb y x11vnc que provee de un escritorio virtual customizable con su gestor de ventanas favorito.

**Usar en modo usuario, es recomendable crear un usuario exclusivo**
* Una vez descargado, ejecutar en el usuario dedicado:
``` [bash]
  $ git clone https://github.com/DanielRosatto/vnc_xstartup.git
  $ cd vnc_xstartup
  $ ./xstartup --user-service <Opcional el comando de arranque de su Window Manager favorito (Ej. Openbox-session)>
```
* Luego reiniciar el usuario dedicado.
* Finalmente poodrá acceder desde otro dispositivo en la misma LAN. 
* Si fuera una Tablet o celular con Realvnc, se crea la conexión <Ip del server *nix:5900>. 
* Sino puede usar un cliente vnc:
``` [bash]
  $ vncviewer <ip server *nix>:0
```
