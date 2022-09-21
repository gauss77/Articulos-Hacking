<p align="center">
  <a href="https://github.com/DenverCoder1/readme-typing-svg"><img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=F70000&width=200&lines=Cracking+WPS+PIN"></a>
</p>

<h1 align="center"></h1>

<h3 align="center"><ins>SISTEMA WPS PIN</ins></h3>

WPS (_Wifi Protected Setup_) es un estándar de red lanzado en el año 2007 cuyo objetivo es facilitar la conexión inalámbrica con tan solo pulsar un botón proveniente del router. De este modo, se evita introducir la contraseña del Wi-Fi (sobre todo si es larga y difícil de recordar) reemplazandola con un PIN de 8 dígito para su fácil acceso. El cifrado WEP no es compatible con WPS, sino con WPA/WPA2. Esto no quiere decir que este basado en brindar seguridad, sino simplemente simplificar el acceso, de hecho, mantenerlo activado puede presentar alto riesgo para los dispositivos que se encuentren conectados a la misma red.

La conexión de WPS es muy sencilla, una de las más comunes es pulsar el botón detrás del router y el emparejamiento con los dispositivos se hará automático. Algunos dispositivos como impresoras, adaptadores Wi-Fi poseen su propio botón WPS, por lo que primero se debe pulsar el del router y luego el del aparato para establecer la conexión. Algunos routers con botón WPS ofrecen un PIN de ocho cifras para simplificar la conexión con dispositivos que no tengan dicho botón, está se debe copiar e introducir manualmente como si fuera la contraseña de la red, que por lo general es más compleja. En caso de no contar con dicho PIN se debe acceder al panel de control del router desde el navegador (http://192.168.1.1) **>** Seguridad WPS y copiar el PIN (también se puede generar uno nuevo).

WPS contempla cuatro tipo de configuraciones diferentes para el intercambio de credenciales:

- **PIN** (Número de identificación personal): Al usuario se le ofrece un PIN de 8 dígitos para que ingrese manualmente en sus dispositivos y establezca conexión sin otorgar la contraseña real del Wi-Fi.

- **PBC** (Configuración del botón pulsador): El usuario presionar el botón WPS del punto de acceso (AP) y seguidamente el botón WPS del dispositivo para establecer la autenticación. Cualquier otra estación cercana no autorizada puede ganar acceso.

- **NFC** (Comunicaciones de campo cercano): Es una tecnología inalámbrica que permite la comunicación e intercambio de datos entre dos dispositivos sin interrupciones a corta distancia. El dispositivo debe ser colocado cerca del router para intercambiar información

- **USB** (Bus Universal en Serie): Es un método de forma física, las credenciales se guardan en una memoria flash USB que luego es introducido en el dispositivo que se desee autenticar a la red.

<p align="center">
  <img src="https://github.com/R3LI4NT/articulos/blob/main/Redes/GNU-Linux/img/WPS_PIN.png">
</p>

#### Vulnerabilidad

En primer lugar, al presionar el botón de habilitar WPS, estas inhabilitando todas las medidas de seguridad configuradas en la conexión, incluyendo el cifrado WPA/WPA2 será de poca utilidad. El PIN consta de 8 dígitos, lo que quiere decir que un ataque de fuerza bruta es más que suficiente para adivinarlo y acceder a la red. El ataque **WPS Pixie Dust** se centra en capturar el intercambio de paquetes entre el router víctima y el atacante, para posteriormente intentar crackear el PIN sin necesidad de conexión (offline) aplicando un diccionario de por medio.

<h1 align="center"></h1>