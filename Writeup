# Welcome

## Rules

En la página del CTF ir al apartado de rules  y hasta el final de esa página está la flag

![c54b75e81b7c5c139e233643fab197d8.png](https://drive.google.com/file/d/1WccLPK-YE3hV7LIWtTeoFf_Go5jNGvtY/view?usp=share_link)

**flag{M1\_Pr1m3r4\_fl46}**

# Web

## HTML index

En la página principal del sitio del CTF abrimos las herramientas de desarrollador y en el inspector de código buscamos "flag". Encontramos la flag como un comentario dentro de un tag a

<img src=":/4eb1a0787b2d400db7facce27e322675" alt="b3898db6115ab22e6f602c58ee36c720.png" width="738" height="155" class="jop-noMdConv">

**flag{h7ml_1nd3x}**

## U.S. Government

Navegamos a la página web oficial de la casa blanca en https://www.whitehouse.gov/ y en el código fuente en el primer comentario está un link que nos lleva a la página web del servicio digital de USA https://www.usds.gov/. Ya que estamos en esa página en el código fuente aparece el cangrejo del reto y su nombre

<img src=":/343467c8159c48faa3a9088ce5e8867c" alt="30e236d500b31bae1f5e4e04b95fc880.png" width="674" height="246" class="jop-noMdConv">

**flag{Mollie}**

# OSINT

## ITESO

Descargamos la imagen que está en la descripción del reto y la abrimos en metadata2go para encontrar el comentario que nos mencionaron

<img src=":/7cb91b8779734694a4a6eba45e99a06f" alt="ad430d57115f80ac7bff7f0f7f7bf3d4.png" width="356" height="312" class="jop-noMdConv">

Copiamos esta cadena de texto y en cyberchef la decodificamos como base64 para encontrar la flag

<img src=":/e51614e75a0748219d4798770265cbbf" alt="2ec3ea1b52f021bac84616039f9b011b.png" width="478" height="249" class="jop-noMdConv">

**flag{the\_m3tadata\_1s_modified}**

## Pcap

Descargamos el archivo pcap de la descripción del reto y lo abrimos con wireshark. Al darle una revisada rápida vemos que hay tráfico de FTP. Filtramos la captura para ver el tráfico de FTP únicamente y vemos la contraseña que ingresaron para acceder

<img src=":/88d1ec9748aa42e1ad0aa9e97711a348" alt="3d903658322f1b8dfa120a26775d28c6.png" width="644" height="170" class="jop-noMdConv">

**flag{ftp\_is\_better\_than\_dropbox}**

## Matryoshka

Descargamos la imagen que está en la descripción del reto y en kali usamos el comando strings sobre ese archivo para encontrar que información tiene la imagen

<img src=":/394d3d5bfe844f4695037cc6415408b7" alt="6382d41315889506993b0f332a9d4eea.png" width="186" height="267" class="jop-noMdConv">

Vemos que hay un archivo matryoshka2.jpg dentro de la imagen que descargamos, por lo que usamos unzip para sacar esa imagen, lo cual nos da otra imagen. unzippeamos los archivos hasta que conseguimos un archivo de texto llamado flag.txt que contiene la flag

![4d5139dd222fada8830e7e6734a347cd.png](:/25614d78b7344ed187bb0fd453f55f77)

**flag{573g4n0gr4f14}**

# Crypto

## Crypto 1

Copiamos el texto cifrado y lo decodificamos como binario en cyberchef para obtener la flag

<img src=":/f07c1d8b9233408ab3751b8272329eed" alt="2bab2d3862f8c725518bac5581712dee.png" width="607" height="231" class="jop-noMdConv">

**flag{un05\_Y\_c3r0s)**

## Crypto 2

Copiamos el texto cifrado y lo decodificamos como hexadecimal en cyberchef para obtener la flag

<img src=":/eae6ea9d969140b6b5fb905b99ebb028" alt="84a0e9e17b215ce31209daf9e8798c4c.png" width="520" height="262" class="jop-noMdConv">

**flag{H3x4d3c1m4l}**

## Crypto 3

Copiamos el texto cifrado y usando el algoritmo de ROT13 lo decodificamos con cyberchef para obtener la flag

<img src=":/93073ff92c104a7d80ae5035451b8630" alt="e0befb9da45b8d6d28ca5cb2692827ca.png" width="514" height="257" class="jop-noMdConv">

** flag{N0\_35\_L0\_m15m0\_c4354r\_c1ph3r\_qu3\_l1ttl3\_c4354r}**

## Hi Hittler!

Copiamos la bandera cifrada y en cyberchef utilizamos el modo enigma con las configuraciones especificadas en el reto para obtener la flag

<img src=":/72b896b860374e1b879cc71f65a1dc93" alt="9c6fd97ca935588673e29a54017f1eb4.png" width="397" height="320" class="jop-noMdConv">

**FLAG{N0\_T0D0\_35\_CYB3R\_CH3F}**

## Decrypt

Descargamos el archivo .zip que está en la descripción del challenge y lo descomprimimos en la terminal de kali

<img src=":/3e3659d05590488c89af92a1d690f702" alt="f5a782b9b5020f09d3ae255f1d043e5e.png" width="395" height="273" class="jop-noMdConv">

Al abrir el archivo ende.py con nano vemos dentro del código que nos explica cómo desencriptar un archivo. Para hacer esto necesitamos el archivo que queremos desencriptar y aunque no sabemos a este punto también necesitaremos la contraseña, pero esa también la tenemos dentro del archivo pw.txt

<img src=":/bb0afef2802045e1929170323361f27b" alt="b50d9c27592fc17a85e71aba647d1f50.png" width="336" height="517" class="jop-noMdConv">

Ejecutamos el archivo ende.py con el archivo de texto a desencriptar y con la contraseña proporcionada y obtenemos la flag

<img src=":/edc12cb4cb6b4a33a6b6a4993f8a3865" alt="4a611a0cd705943cf596fb8e84f76aa4.png" width="372" height="168" class="jop-noMdConv">

**flag{R34l_Crypt0}**

# Nueva categoría

## Felicidades

Al haber completado todos los retos anteriores se nos abrirá esta nueva categoría, junto con Real Hacking, Hacking WIFI y W10. Para obtener la flag basta con abrir la descripción del reto, ahí se nos mostrará la flag y también el link para descargar la máquina de Windows necesaria para hacer los retos de W10

<img src=":/43fb0899db4749a792ff426654477868" alt="25212be617241ab115c403dfb6623ea5.png" width="307" height="426" class="jop-noMdConv">

**FLAG{CH3ckp01n7}**

# Hacking WIFI

## Borrador WEP

Para este reto era necesario ir al laboratorio T-205, o por lo menos estar cerca de él, y usar una antena de red que pudiera ponerse en modo monitor. En mi caso utilicé una antena TP-Link TL-WN722N. Una vez conectada la antena, la ponemos en modo monitor con los siguientes comandos (en mi caso la antena se llama wlan0, puede que el nombre cambie para ti)

<img src=":/bb8c6b5f328441658418306dc9d3e667" alt="9d199689b0527ba43c90568bee9c8a3d.png" width="409" height="441" class="jop-noMdConv">

Una vez que está en modo monitor escaneamos las redes que hay para obtener el BSSID y el canal de la red ITESO_CTF con el comando `airodump-ng wlan0 --encrypt wep`. Ya que tenemos esas dos cosas podemos empezar a inyectar paquetes en la red con el comando `besside-ng wlan0 -c 8 -b E4:E1:30:64:66:7C`

<img src=":/197289a4840f4007996f75c8b055fcb6" alt="17917ec0ad0d7b57e608768cc8f530ed.png" width="520" height="533" class="jop-noMdConv">

Vemos que se inyectaron los paquetes suficientes para obtener la contraseña de la red. Usamos el comando `aircrack-ng ./wep.cap` para ver la contraseña en texto plano

<img src=":/7a1e1d6b6c804ea78245040acdc5555b" alt="7ad81ff64241ebdb9457f6ccf9f56788.png" width="560" height="250" class="jop-noMdConv">

Accedemos a la red con la contraseña que acabamos de obtener y en un navegador web ingresamos la IP del gateway de la red, lo que nos mostrará una página para acceder a la administración del modem que nos pedirá una contraseña. Accedemos con la misma contraseña que accedimos a la red y vamos a la sección de servicios en donde encontraremos el borrador SMS y ahí encontraremos la flag del reto

<img src=":/c28c5b3cede945b085b307a9686bfc6d" alt="36c894e41eb9134a400a4c20466f8854.png" width="640" height="397" class="jop-noMdConv">

**FLAG{5M5\_D35d3\_M0d3m}**

# Real Hacking

## Hashes
