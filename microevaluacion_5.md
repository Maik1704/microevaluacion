# CONFIGURACION DE ROUTERS CON SUBNETING

## SELECCION DE ROUTER
Imagen del primer diseno
![image](https://github.com/user-attachments/assets/c6567998-c09a-4370-8eac-237e855d8152)
## 1. Configuracion de IP de cada Router

## 2. Configuracion de Router de Tarata
### 2.1. Configuracion de la primera IP de Tarata hacia Cliza 
 - Primero Se ingresa a CLI y se ingresa en modo privilegiado
```bash
Enable
```
 - Luego se Ingresa el comando para entrar a la terminal de configuracion
```bash
conf t
```
 - Se le da un nombre con hostname
```bash
hostname Tarata
```
![image](https://github.com/user-attachments/assets/311e0aef-a314-45e8-8ff6-993df72fa2af)

 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet0/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.17 255.255.255.240 
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
![image](https://github.com/user-attachments/assets/90794aff-a36e-4e91-83f8-f4d08aeb9bb3)

### 2.2. Configuracion de la segunda IP de Tarata hacia Arani 
 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet1/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.33 255.255.255.240
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
![image](https://github.com/user-attachments/assets/9dae58c3-a39c-422c-9630-f36e44546852)

### 2.3. Configuracion de la tercera IP de Tarata hacia Punata 
 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet2/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.50 255.255.255.240
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
![image](https://github.com/user-attachments/assets/d1057319-525c-4768-ac59-66e3d6b67f2f)

### 2.4. Configuracion de la tercera IP de Tarata hacia Punata 
 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet3/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.65 255.255.255.240
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para terminar con la configuracion del router de Tarata colocamos el siguiente comando
```bash
end
```
 - Y para guardarlo usamos el siguiente comando
```bash
write memory
```
![image](https://github.com/user-attachments/assets/faa59737-ed44-47c3-8b8a-658b2127d8da)

## 3. Configuracion de Router de Cliza
### 3.1. Configuracion de la primera IP de Cliza hacia Tarata
 - Primero Se ingresa a CLI y se ingresa en modo privilegiado
```bash
Enable
```
 - Luego se Ingresa el comando para entrar a la terminal de configuracion
```bash
conf t
```
 - Se le da un nombre con hostname
```bash
hostname Cliza
```
![image](https://github.com/user-attachments/assets/aca8632d-5778-480d-a72d-b73489f9449c)

 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet0/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.18 255.255.255.240 
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
![image](https://github.com/user-attachments/assets/6a1b825b-b311-4536-86dd-9751414dbbb4)

### 3.2. Configuracion de la segunda IP de Cliza hacia el Switch
 - Ahora se configura con interface para que el router tenga una ip del router
```bash
interface GigabitEthernet1/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.81 255.255.255.240
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
 - Para terminar con la configuracion del router de Cliza colocamos el siguiente comando
```bash
end
```
 - Y para guardarlo usamos el siguiente comando
```bash
write memory
```
![image](https://github.com/user-attachments/assets/0e7a3fb3-0968-4ef2-bf62-b9c03a526b1f)

## 4. Configuracion de Router de Arani
### 4.1. Configuracion de la primera IP de Arani hacia Tarata
 - Primero Se ingresa a CLI y se ingresa en modo privilegiado
```bash
Enable
```
 - Luego se Ingresa el comando para entrar a la terminal de configuracion
```bash
conf t
```
 - Se le da un nombre con hostname
```bash
hostname Arani
```
![image](https://github.com/user-attachments/assets/ffa246e9-5ac9-49a6-9fe3-f68ec668bbfa)

 - Ahora se configura con interface para que el router tenga una ip del router
```bash
interface GigabitEthernet0/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.34 255.255.255.240 
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
![image](https://github.com/user-attachments/assets/9c9d473c-0c41-4245-be1e-0cdc25dcd8fa)

### 4.2. Configuracion de la segunda IP de Cliza hacia el Switch
 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet1/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.97 255.255.255.240
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
 - Para terminar con la configuracion del router de Cliza colocamos el siguiente comando
```bash
end
```
 - Y para guardarlo usamos el siguiente comando
```bash
write memory
```
![image](https://github.com/user-attachments/assets/034495c0-cf65-45ce-b456-03750fc55c94)

## 5. Configuracion de Router de Punata
### 5.1. Configuracion de la primera IP de Punata hacia Tarata
 - Primero Se ingresa a CLI y se ingresa en modo privilegiado
```bash
Enable
```
 - Luego se Ingresa el comando para entrar a la terminal de configuracion
```bash
conf t
```
 - Se le da un nombre con hostname
```bash
hostname Punata
```
![image](https://github.com/user-attachments/assets/d9ce041e-af03-4ca9-89f8-8da3f28af858)

 - Ahora se configura con interface para que el router tenga una ip del router
```bash
interface GigabitEthernet0/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.51 255.255.255.240 
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
![image](https://github.com/user-attachments/assets/3469e42a-1794-4b34-8a52-5ba5470cc782)

### 5.2. Configuracion de la segunda IP de Cliza hacia el Switch
 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet1/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.97 255.255.255.240
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
 - Para terminar con la configuracion del router de Cliza colocamos el siguiente comando
```bash
end
```
 - Y para guardarlo usamos el siguiente comando
```bash
write memory
```
![image](https://github.com/user-attachments/assets/7f1ca173-c976-413b-a527-5138db060c31)

## 6. Configuracion de Router de ElPaso
### 5.1. Configuracion de la primera IP de ElPaso hacia Tarata
 - Primero Se ingresa a CLI y se ingresa en modo privilegiado
```bash
Enable
```
 - Luego se Ingresa el comando para entrar a la terminal de configuracion
```bash
conf t
```
 - Se le da un nombre con hostname
```bash
hostname ElPaso
```
![image](https://github.com/user-attachments/assets/ba19f8ac-8fc1-4b68-9840-cdbb8273af7a)

 - Ahora se configura con interface para que el router tenga una ip del router
```bash
interface GigabitEthernet0/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.66 255.255.255.240 
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
![image](https://github.com/user-attachments/assets/3cbb7abd-6f44-4c92-ba83-343efd16a25e)

### 5.2. Configuracion de la segunda IP de ElPaso hacia el Switch
 - Ahora se configura con interface para que el router tenga una ip con los demas router
```bash
interface GigabitEthernet1/0
```
 - Y se le asigna la ip correspondiente
```bash
ip address 200.30.40.129 255.255.255.240
```
 - Por ultimo se le aplica para que se encienda
```bash
no shutdown
```
 - Para configurar la siguiente ip ahora colocamo exit para salir de la interface
```bash
exit
```
 - Para terminar con la configuracion del router de Cliza colocamos el siguiente comando
```bash
end
```
 - Y para guardarlo usamos el siguiente comando
```bash
write memory
```
![image](https://github.com/user-attachments/assets/34edf9b2-a9af-4320-9694-3d24a9bd7544)

### 6. Darle IP a las PCs
Por ultimo ingresas a la PC en la parte de config y le asignas una IP con DHCP
![image](https://github.com/user-attachments/assets/e89de66c-37fc-484c-9ab1-5c4d16b32106)
