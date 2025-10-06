# T03: Seguretat Lògica: recuperant accés a sistemes
## Enunciat

Després de la primera feina exitosa, us arriba un encàrrec urgent que obliga a que us hi poseu per donar-li solució.  
Com a fase prèvia rebreu una formació sobre la seguretat lògica que us permetrà tenir els coneixements necessaris per afrontar la tasca.  
Han arribat a la consultora un equip provinent d’un client que demana que els hi solucionem el problema.  
Tenen un portàtil amb **Zorin OS** (un Linux amb entorn gràfic) que usava habitualment un directiu. El problema és que ha oblidat la contrasenya i és necessari poder recuperar l’accés perquè hi ha documentació molt important que cal recuperar. Per evitar que una acció catastròfica pugui danyar l’equip original, ens han clonat el disc en un disc virtual perquè hi treballeu.

Per tant, el primer pas serà crear una màquina virtual al que connectareu aquest disc. A continuació, cal que entreu a la màquina virtual, trobeu el nom de l’usuari existent i assigneu-li una contrasenya nova.  
Quan el client és informat del senzill que és accedir a l’equip, demana si n’hi ha alguna manera de fortificar el sistema, ja que té por que si algú roba el portàtil hi pugui accedir a la informació que hi conté. Per tant, ara ens demanen que cerquem solucions per tal d’evitar que es pugui reiniciar la contrasenya amb el procediment anterior.  
Investigueu el procediment per tal que l’accés al GRUB quedi protegit per contrasenya per evitar canvis de configuració.

---

## Procediment individual

1. Vulnereu l’accés al GRUB del Linux.  
2. Identifiqueu l’usuari del sistema.  
3. Modifiqueu la contrasenya de l’usuari i verifiqueu que ara ja té accés.  
4. Investigueu com es pot fortificar l’accés al GRUB. És molt important que indiqueu les **fonts d’informació** que useu.  
5. Configureu la màquina virtual per tal de fortificar l’accés al GRUB.  
6. Documenteu el procediment en un document (cal incloure **imatges**) per posteriorment pujar-lo al vostre repositori.

---


## Solució

A l'arxiu [solucio.md](solucio.md) hi ha la solució de la tasca 3

[Tornar a la pàgina principal](../README.md)

