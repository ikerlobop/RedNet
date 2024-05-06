# RedNet
## Comandos Esenciales de Windows para Administración de Redes

| Comando                                     | Descripción                                                                                                           |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| `ping 192.168.2.10`                        | Este comando envía un paquete de datos a la dirección IP 192.168.2.10 para verificar la conectividad de red. Si la dirección IP responde, significa que hay conectividad con esa dirección IP. |
| `ping -n 5 192.168.2.11`                   | Realiza una prueba de ping a la dirección IP 192.168.2.11, especificando que solo debe enviar 5 paquetes de ping.     |
| `ipconfig \| find "IPv4"`                  | Muestra la configuración de red del equipo utilizando ipconfig y filtra la salida para mostrar solo la información relacionada con direcciones IPv4. |
| `ipconfig /all \| find "Descripción"`      | Muestra la descripción de todas las interfaces de red disponibles en el sistema.                                      |
| `ipconfig /all \| find "Nombre de host"`   | Muestra el nombre del host del sistema.                                                                               |
| `echo %userdomain%`                        | Muestra el nombre del dominio del usuario actualmente autenticado en el sistema.                                      |
| `ipconfig /all \| find "Dirección física"` | Muestra la dirección física (dirección MAC) de todas las interfaces de red disponibles en el sistema.                 |
| `arp -a`                                   | Muestra la tabla de traducción de direcciones ARP del equipo, que asocia direcciones IP con direcciones MAC.          |
| `nslookup google.es 8.8.8.8`               | Realiza una búsqueda de DNS inversa de la dirección IP de Google (google.es) utilizando el servidor DNS 8.8.8.8.      |
| `netstat -e -s`                            | Muestra estadísticas de red detalladas, incluyendo estadísticas de Ethernet.                                          |
| `netstat -s -p tcp`                        | Muestra estadísticas de protocolo TCP, como el número de segmentos enviados/recibidos, errores, etc.                  |
| `netstat -o 5`                             | Muestra las conexiones activas cada 5 segundos, junto con el PID (identificador de proceso) asociado a cada conexión. |
| `netstat -n -o`                            | Muestra las conexiones activas con direcciones IP y números de puerto en lugar de nombres de host y servicios, junto con el PID asociado a cada conexión. |
| `nbtstat /n`                               | Muestra estadísticas y conexiones NetBIOS sobre TCP/IP.                                                               |
| `tracert google.es`                        | Muestra la ruta tomada por los paquetes para llegar a la dirección IP de Google, mostrando cada salto en la red.      |
| `pathping google.es`                       | Proporciona información detallada sobre la ruta de red y el rendimiento de cada salto hacia la dirección IP de Google.|
| `route PRINT`                              | Muestra la tabla de enrutamiento del equipo, que contiene información sobre las rutas de red disponibles.             |
| `netsh int ip reset`                       | Restablece la configuración TCP/IP a los valores predeterminados, útil para solucionar problemas de conectividad de red al eliminar configuraciones incorrectas. |
