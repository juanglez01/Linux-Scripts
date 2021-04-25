## Objetivo
Este Script lo utilizamos para saber el Hardware que lleva nuestro equipo. Con esta herramienta sabremos todos los detalles de este.<p> Espero que les sirva de ayuda.</p>

## Comentarios
Para poder realizar este Script. lo primero que tenemos que hacer es con la herramienta apt install, descargarnos lshw.
<p><img src="https://github.com/juanglez01/Linux-Scripts/blob/5a93f937498d128c67234f8443f487475c17a6c4/Hardware/Captura%20de%20pantalla%20de%202021-04-24%2018-10-45.png"></p>

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
    <li> **Encabezado:** Para presentar el script.</li>
    <li> **ComprobarRoot:** Para que el script al ejecutarlo sí o sí tenga que ejecutarse como root para recibir los datos.</li>
</ul>
    
