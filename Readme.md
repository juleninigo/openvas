# A Greenbone Vulnerability Management docker image
### Brought to you by ###
[![Immauss Cybersecurity](https://github.com/immauss/openvas/raw/master/images/ics-hz.png)](https://immauss.com "Immauss Cybersecurity")


- - - -
## Instalación ##
Para instalar esta herramienta lo primero que deberemos hacer será clonar el repositorio a nuestro equipo, empleando el comando git clone
- - - - 

```
git clone https://github.com/juleninigo/openvas.git 
```
Después de clonar el repositorio nos situaremos en la carpeta openvas/compose y ejecutaremos el siguiente comando en la terminal


- - - - 
```
make start
```
El proceso tardara un rato...

- - - - 
Una vez este instalado entraremos en la url para acceder al panel de Openvas.
```
http://localhost:9392  admin:admin
```

- - - -
## Actualizacion de feeds ##
- - - - 
Una vez dentro del panel de openvas vamos a sincronizar los repositorios de vulnerabilidades, a mi me salen que ya estan actualizados.

- - - - 

![Panel](https://github.com/juleninigo/openvas/raw/master/images/feeds.png)

---

Ahora para actualizar las feeds en vuestras maquinas podeis usar el siguiente comando para tener una shell en el contenedor.

```
make workspace
```

