# A Greenbone Vulnerability Management docker image
### Brought to you by ###
[![Immauss Cybersecurity](https://github.com/immauss/openvas/raw/master/images/ics-hz.png)](https://immauss.com "Immauss Cybersecurity")


- - - -
## Instalación ##
Para instalar esta herramienta lo primero que deberemos hacer será clonar el repositorio a nuestro equipo, empleando el comando git clone
- - - - 

```
git clone  
```



```
docker run -d -p 9392:9392 -p 9390:9390 -e GMP=9390 --name openvas -v openvas:/data immauss/openvas:latest 
```

