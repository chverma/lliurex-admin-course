# Tema 6: Proxmox
## Introducción


## Instalación
Una vez descargada la ISO y grabada en un USB, iniciamos con el USB.

![Remote Installer](img/tema6/1.png "Licencia de Proxmox")

Todos sabemos que es importante leerse la licencia :)

![Licencia de Proxmox](img/tema6/2.png "Licencia de Proxmox")


Esta es una de las partes más delicadas y depende de lo que queréis tener montado en vuestro centro, también depende de la cantidad de discos duros que tengáis instalados y de si queréis invertir dinero en una cabina de discos duros.

![Opciones de instalación](img/tema6/3.png "Opciones de instalación")

Si queréis dejarlo en ext4. Y utilizar un único disco para utilizar Proxmox en las máquinas virtuales, no va a dar malos resultados. El otro disco duro lo podéis utilizar para hacer copias de seguridad.

Proxmox utiliza ZFS que es una combinación de administrador de volúmenes y sistema de ficheros.

![Selección de opciones](img/tema6/4.png "Selección de opciones")


Las opciones que tenemos son las siguientes:

| Sistema         | Características |
|:--------------|:-----|
|RAID0 	|Suma capacidades de los discos. Si falla una unidad es inservible.|
|RAID1 	|Dato escrito idénticamente. Mínimo 2 discos de la misma medida.|
|RAID10 |	Una combinación de RAID0 y RAID1. Mínimo 4 discos.|
|RAIDZ-1 |	Variación de RAID-5, paridad sola. Mínimo 3 discos.|
|RAIDZ-2 |	Variación de RAID-5, paridad doble. Mínimo 4 discos.|
|RAIDZ-3 |	Variación encima RAID-5, paridad triple. Mínimo 5 discos|

Si habéis optado por adquirir una tarjeta controladora para montar un RAID, esta opción no la tenéis que usar. Siempre y cuando la tarjeta sea reconocida por Proxmox, se verá como un único disco. Las opciones que estamos configurando es RAID por vía software.

La opción más nivelada entre todos los parámetros a tener en cuenta sería la opción de RAID1.

![Opción recomendada](img/tema6/5.png "Opción recomendada")


Configuramos la zona geográfica.

![Zona geográfica](img/tema6/6.png "Zona geográfica")


Configuramos el password y la contraseña.

![Configuración de contraseña](img/tema6/7.png "Configuración de contraseña")


Configura la red según los parámetros de tu centro. El ejemplo dado no es el correspondiente al que deberías de utilizar.

![Configuración de red](img/tema6/8.png "Configuración de red")

Comprobamos que todos los parámetros que hemos configurado son los correctos y le damos a Install. Enseguida empezará la instalación que suele ser bastante rápida.

![Instalación de proxmox](img/tema6/9.png "Instalación de proxmox")


Una vez finalizada la instalación. Reiniciamos el sistema y pasaremos a la siguiente unidad. Configuración del Proxmox.

![Instalación de proxmox](img/tema6/10.png "Instalación de proxmox")

## Configuración


## Funcionamiento
¿Cómo combinar la complejidad y la variedad del software de los ciclos formativos de la tarde con la sencillez y la estabilidad de las clases de informática en ESO y Bachillerato? ¿Cómo utilizar servicios pesados en las aulas informáticas? Tenemos el problema de que los ciclos formativos requieren de gran variedad de servicios como diversos servidores web, diversos servidores de BD, diversos entornos de desarrollo, etc. Se instala y se desinstala mucho. Si instalamos directamente en el servidor corremos el riesgo de que haya problemas en el aula y si se usan máquinas virtuales el rendimiento es muy bajo porque tanto el servidor como los clientes no son potentes. ¿Alguna sugerencia? ¿Cómo lo hacen en otros centros?