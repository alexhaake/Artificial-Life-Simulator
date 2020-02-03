PROYECTO DE REDES -ALEX HAAKE

INTRODUCION
Son dos oficinas una de 3 plantas y otra de  3 plantas- donde se comunican algunas plantas.
Izquierda-Oficina 1 :3 plantas
Derecha-Oficina 2: 2 plantas

OFICINA 1 - Planta 1:

Tenemos un router configurado con dos ethernet ip (0/0) y (0/1) y enroturado con (0/0/1) y y a sus dos ethernet correspondientes.
esta conectado a un swicht.
este Siwcht tiene 2 subnet distintas conectadas
1- es la 192.168.2.0 - esta es estatica con una impresora.
2-es la 192.168.8.0- esta es hibrida en un servidor DHCP configurado + acces point+3 equipos conectados inalambricamente + impresora inalambrica y 3 equipos conectados fisicamente al swicht.

OFICINA1 - Planta 2-(union con oficina nº2)

Tenemos un router configurado con dos ethernet (0/0) y (0/1)+enroturado con router de planta 1 y planta 3 y a sus dos ethernet correspondientes.
el router esta conectado a 2 swicht de distintas oficinas.
swicht nº1 Oficina1-> en este tenemos 2 subnet de tipo c
1-configurada estaticamente y conectada fisicamente al swicht. Rango 0 a 64
2-configurada mediante DHCP en otro rango 64 a 128 - aparte un point que funciona mediante el servidor DHCP y da IP a 2 portatiles y una impresora de forma inalambrica.
swicht nº 2 Oficina2-> este swicht tiene 4 servidores HTTP con imagienes
y un servidor DNS al que son accesibles todas las redes de las dos oficinas.

OFICINA1 -Planta3(union con oficina nº2)

Este Router esta configurado con una Ethernet(0/0) y enrutado con dos router en
0/0 y 0/1 y a su ethernet correspondiente .
El router de planta 3 esta conectado a un swicht.
Este Siwcht tiene conectados 10 equipos en VLSM usando 3 rangos distintos.

OFICINA2-Planta3(union con oficina n1)
Este router esta configurado con dos Ethernet(0/0)y(0/1) y enrotutado a otro 
router de la oficina 1 y a sus dos ethernet correspondientes.
Este router esta conectado a un swicht con dos Subnet de TIPO B.
1 subnet tipo B-esta configurada en un servidor DHCP. rango 0-64.
2 subnet de tipo B-esta configurada de forma estatica. rango 64-128.
