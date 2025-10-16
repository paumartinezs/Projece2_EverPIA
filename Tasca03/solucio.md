# T03: Seguretat Lògica: recuperant accés a sistemes

Un cop instalada la màquina, al iniciar-la prem **(Shift + Qualsevol tecla)** per entrar al menú de Zorin i prem la segona opció **“Advanced options for Zorin”**.

![imagen](img/foto1.png)

Després, ves a l’opció on diu **“Recovery mode”** i prem **Enter** (pots utilitzar qualsevol de les dues).

![imagen](img/foto2.png)

Un cop dins del menú de recuperació, entra en el **root** com surt en la captura per poder canviar la contrasenya.

![imagen](img/foto3.png)

Utilitza “mount -rw -o remount / per poder canviar la contrasenya del usuari.

![imagen](img/foto4.png)

Per trobar el nom d’usuari del usuari utilitza el codi mostrat en la captura

![imagen](img/foto5.png)

Per canviar la contrasenya escriu “passwd + usuar” (el usuari es el que has trobat anteriorment) i escriu la contrasenya nova.

![imagen](img/foto6.png)

Si heu seguit els passos com diu en aquesta guia, us ha de deixar poder entrar en el usuari.

![imagen](img/foto7.png)

Utilitza “grub-mkpasswd-pbkdf2” per generar un hash a partir d’una contrasenya.

![imagen](img/foto8.png)

Usa “grub-mkpasswd-pbkdf2 | tee salida.txt per permitir redirigir la sortida estàndard cap a un arxiu.

![imagen](img/foto9.png)

Ara fica “sudo nano -F /etc/grub.d/40_custom” per afegir la autentificació”

![imagen](img/foto10.png)

Un cop dins de l'arxiu nano, a la última línea posa “set superusers="nombre_login"
password_pbkdf2 nomre_login” i a la segona linia a continuació del nom utilitzat per el login posa el hash 

![imagen](img/foto11.png)

Guarda utilitzant “ sudo grub-mkconfig -o /boot/grub/grub.cfg” i reinicia la màquina

![imagen](img/foto12.png)

Després de reiniciar, fica el usuari i la contrasenya que has posat anteriorment y ya estaria.
