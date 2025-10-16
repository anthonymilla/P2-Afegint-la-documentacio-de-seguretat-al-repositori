# T03: Seguretat Lògica: recuperant accés a sistemes

- ## Vulneració de l’accés al GRUB del Linux
Creem la nova màquina i posem la ISO.
![Creant la màquina virtual, posant la ISO](img/Imatge11.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge10.png)
![Posem el disc a SATA](img/Imatge09.png)

Al iniciar la màquina fem shift + f (qualsevol tecla) i ens entrarà aquí al menú d'arrencada de Zorin:
![fem shift + f o qualsevol tecla per entrar al menú d'arrencada de Zorin](img/Imatge08.png)
![Escollim Zorin recovery mode](img/Imatge07.png)
![Escollim per poder posar-nos com a root](img/Imatge06.png)
![Root](img/Imatge05.png)

- ## Identifiqueu l’usuari del sistema.

![Identificant l’usuari del sistema](img/Imatge04.png)

![Identificant l’usuari del sistema](img/Imatge03.png)
- ## Modifiqueu la contrasenya de l’usuari i verifiqueu que ara ja té accés.
![Modificant la contrasenya de l’usuari i verificant que ara ja té accés](img/Imatge02.png)
![Modificant la contrasenya de l’usuari i verificant que ara ja té accés](img/Imatge01.png)

- ## Investigueu com es pot fortificar l’accés al GRUB. És molt important que indiquis les fonts d’informació que usis.

## Què és el GRUB:
El GRUB és un gestor d'arrencada que permet triar quin sistema operatiu iniciar quan encenem l'ordinador.

## Per què aquesta necessitat de protegir el GRUB:
Si no està protegit, qualsevol persona amb accés físic pot modificar els paràmetres, entrar com usuari root i controlar completament l'ordinador sense necessitat de contrasenya.

## Com protegir el GRUB?

1. Fer còpia de seguretat dels arxius de configuració.
2. Crear usuaris i contrasenyes per accedir al GRUB (diferents dels usuaris del sistema).
3. Xifrar les contrasenyes amb un hash perquè no estiguin en text pla.
4. Actualitzar la configuració del GRUB perquè apliqui la protecció.
5. Opcionalment, bloquejar l’arrencada d’alguns sistemes operatius sense contrasenya o permetre que alguns es puguin arrencar lliurement (segons la versió de GRUB).

## Més mesures de seguretat:
Protegir el GRUB no és realment suficient, ja que també cal xifrar les particions, protegir la BIOS/UEFI amb contrasenya, també impedir l’arrencada des de dispositius externs i limitar l’accés físic a l’ordinador.

[Font d'informació que he usat](https://geekland.eu/proteger-el-grub-con-contrasena/).

- ## Configura la màquina virtual per tal de fortificar l’accés al GRUB
Ara protegirem el GRUB, posant la següent comanda:
![Protegint el GRUB](img/Imatge12.png)

Ara editarem l’arxiu, posem aquesta comanda:                          
![Editarem l'arxiu](img/Imatge13.png)

Seguidament el guardarem a salida.txt amb control+R.
![El guardarem a salida.txt amb control+R](img/Imatge14.png)

Ara posarem l’autenticació.
![Posant l’autenticació.](img/Imatge15.png)

Seguidament posem la següent comanda:
![Per mirar si tot està correcta](img/Imatge16.png)

I per finalitzar fem la comprovació.               
![Comprovació](img/Imatge17.png)

[Anar a l'enunciat](../Tasca02/README.md)                 
[Anar a la pàgina inicial](../README.md)

