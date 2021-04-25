## Objetivo
Este Script lo utilizamos para saber el Hardware que lleva nuestro equipo. Con esta herramienta sabremos todos los detalles de este.<p> Espero que les sirva de ayuda.</p>

## Comentarios
Para poder realizar este Script. lo primero que tenemos que hacer es con la herramienta apt install, descargarnos lshw. (Como Root)
```
apt install lshw
```


# Script

## Funciones
```
Encabezado ()
{
    clear
    echo "___________________________________________"
    echo ""
    echo "         Hardware del Dispositivo"
    echo "___________________________________________"
    echo ""
}
ComprobarRoot ()
{
    if [ $(whoami) != "root" ]
    then
        echo "No eres el root"
        exit 1
    fi
}
```
En las funciones del Script he incorporado dos:
<ul>
    <li>Encabezado: Para presentar el script.</li>
    <li>ComprobarRoot: Para que el script al ejecutarlo sí o sí tenga que ejecutarse como root para recibir los datos.</li>
</ul>
    
## Bloque Principal
```
clear
Encabezado
ComprobarRoot
lshw
```

## Script Completo
```
#!/bin/bash
#Definicion de Variables

#Definición de Funciones
Encabezado ()
{
    clear
    echo "___________________________________________"
    echo ""
    echo "         Hardware del Dispositivo"
    echo "___________________________________________"
    echo ""
}
ComprobarRoot ()
{
    if [ $(whoami) != "root" ]
    then
        echo "No eres el root"
        exit 1
    fi
}
#Bloque Principal
clear
Encabezado
ComprobarRoot
lshw
```

## Vídeo de Utilización
<https://youtu.be/uKw5-C3exFA>
## Descargar Script
<https://drive.google.com/u/1/uc?export=download&confirm=lVO0&id=1Yh0711ieIXOHDZSWnvAzI4nHJrIj-gyU>
