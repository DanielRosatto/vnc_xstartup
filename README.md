## vnc_xstartup v0.1

Unix script basado en Xvfb y x11vnc que provee de un escritorio virtual customizable con su gestor de ventanas favorito.

**Usar en modo usuario, es recomendable crear un usuario exclusivo**
* Desde el usuario dedicado hacer:
``` [bash]
  $ git clone https://github.com/DanielRosatto/vnc_xstartup.git
  $ cd vnc_xstartup
  $ ./xstartup --user-service <Opcional el comando de arranque de su Window Manager favorito (Ej. Openbox-session)>
```
* Luego reiniciar el usuario dedicado.
* Finalmente poodrá acceder desde otro dispositivo en la misma LAN.
* Si fuera una Tablet o celular con Realvnc, se crea la conexión <Ip del host>:5900
* Sino puede usar el cliente vnc que sse incorpora con las dependencias:
``` [bash]
  $ gvncviewer <ip del host>:0
```
En el caso de ser un usuario avanzado, es posible modificar el servidor vnc editando convenientemente la linea FF de xstartup 
