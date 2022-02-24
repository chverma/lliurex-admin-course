# Tema 5: Administrando el aula Lliurex
## Introducción
En esta unidad veremos cómo inicializar un servidor de aula Lliurex, aprenderemos a qué redes estamos conectados y con qué interfaz, conoceremos cómo instalar software de forma automática y remota, veremos cómo gestionar de forma todos los equipos de nuestra aula y, finalmente, indagaremos en la herramienta para la gestión de los repositorios.

## Conceptos

## Configuración del servidor de aula

## Conexiones de red cliente y servidor

## Instalación remota de software
Instalación de software tanto en el servidor como en los clientes sin necesidad de hacer uso de Zero Center y sin que estas acciones interfieran con lo previamente instalado.

## Gestión remota de los clientes

## Gestión de repositorios
Finalmente, vamos a ver la herramienta Repoman (Repository Manager). Esta no es una herramienta para instalar paquetes, sino para gestionar los diferentes repositorios o depósitos de software configurados a nuestro ordenador. En nuestro sistema, podemos tener tantos repositorios configurados cómo deseamos. De manera predeterminada, en LliureX solo tendremos configurados los depósitos de software de LliureX, pero podemos configurar todos los que deseamos.

Para acceder a la herramienta, lo hacemos a través del menú de Inicio > Administración de LliureX > RepoMan, o directamente buscándolo en la barra de busca del menú de inicio.
![Repoman](img/tema5/repoman1.png "Repoman")

La primera pantalla que nos muestra la herramienta es la de Opciones, con enlaces a las diferentes secciones, las cuales también se nos muestran al cuadro de la izquierda. Las diferentes opciones disponibles que tenemos son:
* Gestionar los repositorios por defecto, donde podremos:
    * Activar o desactivar los repositorios de LliureX desde Internet (de manera predeterminada en la versión de escritorio están activados)
    * Activar o desactivar los repositorios de LliureX desde uno Mirror o Réplica del centro. Si trabajamos en un modelo de centro y disponemos de una réplica de los repositorios de LliureX al servidor, esta sería la opción más adecuada.
    * Activar o desactivar los repositorios de Ubuntu. De manera predeterminada están desactivados, y podemos activarlos si necesitamos software de Ubuntu que no esté en LliureX. En caso de que un paquete esté tanto en los repositorios de Ubuntu como a los de LliureX, tendrá preferencia lo del repositorio de LliureX, aunque haya una versión más actualizada en Ubuntu.
* Gestionar repositorios personalizados, donde podremos configurar otros repositorios externos en LliureX y en Ubuntu. Para añadir un nuevo repositorio haremos clic en el botón que hay encima del recuadro de los repositorios, y añadimos su dirección web, junto con el nombre y una descripción.
* Herramientas del sistema, desde donde podremos actualizar las listas de software, lanzar el actualizador LliureX Up o LliureX Store.

![Repoman](img/tema5/repoman2.png "Repoman")