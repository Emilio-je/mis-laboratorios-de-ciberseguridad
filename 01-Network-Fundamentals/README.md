# Lab 01 - Network Fundamentals

## Objetivo

Comprender los fundamentos de las redes de computadoras y la comunicación entre dispositivos dentro y fuera de una red local.

## Topología

La práctica fue realizada utilizando Cisco Packet Tracer.

La red está compuesta por:

- 1 Router Cisco 1941
- 1 Switch Cisco 2960
- 1 PC
- 1 Laptop
- 1 Cable Modem

## Direccionamiento IP

| Dispositivo | Dirección IP | Máscara | Gateway |
|---|---|---|---|
| PC1 | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| PC2 | 192.168.1.20 | 255.255.255.0 | 192.168.1.1 |
| Router | 192.168.1.1 | 255.255.255.0 | N/A |

## Conceptos aprendidos

### Switch

Un switch permite conectar diferentes dispositivos dentro de una misma red local y facilitar la comunicación entre ellos.

### Router

Un router conecta diferentes redes y permite que los dispositivos de una red local puedan comunicarse con otras redes.

### Dirección IP

Una dirección IP identifica lógicamente a un dispositivo dentro de una red.

### Dirección MAC

La dirección MAC identifica la interfaz de red de un dispositivo y normalmente permanece estable.

### Gateway

El gateway predeterminado permite que un dispositivo pueda enviar tráfico destinado a otras redes.

### DNS

DNS permite resolver nombres de dominio en direcciones IP.

### ARP

ARP permite descubrir la dirección MAC asociada a una dirección IP dentro de una red local.

## Comunicación dentro de la LAN

Cuando PC1 necesita comunicarse con PC2 y ambos pertenecen a la misma red, el tráfico no necesita pasar por el router.

```text
PC1
192.168.1.10
      |
      v
   Switch
      |
      v
PC2
192.168.1.20

    
PC1
192.168.1.10
      |
      v
   Switch
      |
      v
Router
192.168.1.1
      |
      v
   Internet
