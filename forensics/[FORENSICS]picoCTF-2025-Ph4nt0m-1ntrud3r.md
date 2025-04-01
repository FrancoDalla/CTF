<h1>Descripción</h1>
A digital ghost has breached my defenses, and my sensitive data has been stolen! 😱💻 Your mission is to uncover how this phantom intruder infiltrated my system and retrieve the hidden flag. To solve this challenge, you'll need to analyze the provided PCAP file and track down the attack method. The attacker has cleverly concealed his moves in well timely manner. Dive into the network traffic, apply the right filters and show off your forensic prowess and unmask the digital intruder! Find the PCAP file here Network Traffic PCAP file and try to get the flag. 

<h1>Resolución</h1>
Se reviso la captura de trafico con Wireshark. Al abrirla se pudo ver un par de cadenas que parecian ser partes de una cadena en base64.
Tras esto se utilizo el comando strings mediante una terminal para ver las cadenas de texto del pcap. Se copio el resultado y se pego en cyberchef para ver si se podía ver algún mensaje traduciendo desde base64.
Al realizar esto se pudo ver una salida de texto bastante desordenada pero que, sin embargo, permitía ver algúnos textos que se distuinguían como parte de un mensaje, tales como "PICOCTF", "th4t", "34sy". Al ver esto una teoría era que el mensaje estaba copiado en desorden por lo que en wireshark se ordenaron los paquetes por tiempo para copiar de esta manera los datos y ver si el resultado era más comprensible.
Al hacerlo se pudo divisar la FLAG picoCTF{1t_w4snt_th4t_34sy_tbh_4r_e5e8c78d} que era la solución al reto. 


<h1>Enlace al material del ejercicio</h1>
https://drive.google.com/file/d/1vsVHiscSu-vrVxrIifWP7PMuwVJM-MhF/view?usp=sharing

<h1>CAPTURAS</h1>

![pop](https://github.com/user-attachments/assets/601689f0-b4b2-40fa-bbbc-3df5019de3bd)

<i>Captura de la salida de strings del pcap</i>


![Captura de pantalla de 2025-03-07 17-48-49](https://github.com/user-attachments/assets/513591ea-5a38-455b-978a-2e20133f46bb)
<i>Captura de el resultado de la cadena con el orden que salia con strings</i>


![capturaDeFlag](https://github.com/user-attachments/assets/983f3983-3d2e-4a30-b21e-1195ffec1e71)
<i>Captura de la salida del texto al ordenar las capturas y copiar los valores de la cadena base64</i>
