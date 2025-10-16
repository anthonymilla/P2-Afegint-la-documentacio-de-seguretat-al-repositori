# T03: Seguretat Lògica: recuperant accés a sistemes

- ## Vulneració de l’accés al GRUB del Linux
![Creant la màquina virtual, posant la ISO](img/Imatge11.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge10.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge09.png)

Al iniciar la màquina fem shift + f (qualsevol tecla) i ens entrarà aquí al menú d'arrencada de Zorin:
![Creant la màquina virtual, memòria base i processors](img/Imatge08.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge07.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge06.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge05.png)

- ## Identifiqueu l’usuari del sistema.

![Creant la màquina virtual, memòria base i processors](img/Imatge04.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge03.png)
- ## Modifiqueu la contrasenya de l’usuari i verifiqueu que ara ja té accés.
![Creant la màquina virtual, memòria base i processors](img/Imatge02.png)
![Creant la màquina virtual, memòria base i processors](img/Imatge01.png)

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

