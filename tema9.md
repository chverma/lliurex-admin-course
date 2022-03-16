# Tema 9: Resolución de problemas
## El cliente no conecta con el servidor
1. Verificar link en la tarjeta de red tanto en el cliente como en el servidor
2. Acceder al cliente con usuario local y verificar parámetros de red (ip a)
3. Si el link está down o no se visualiza la tarjeta, puede que haya que habilitarla en la BIOS
4. Si hay link, probar *sudo netplan apply*
5. Si los parámetros de red son correctos, reiniciar el cliente

## El cliente conecta con el servidor pero no tiene Internet
1. Verificar si hay Internet en el servidor
2. Si lo hay, en el cliente ejecutar *resolvectl status* y nos dará el servidor DNS que debe ser el servidor
3. Verificar en el control de enrutamiento [Gestor de enrutamiento](https://wiki.edu.gva.es/lliurex/tiki-index.php?page=Gestor+de+enrutamiento+y+NAT).

## Ordenador arranca y se queda parado en el arranque

## El servidor no tiene Internet

## Un usuario no puede hacer login con sus credenciales

## El servidor ha dejado de funcionar

## Limpiar datos para el siguiente curso
En caso de que un servidor se "rompa" a nivel Software, cómo poder recuperarlo, ¿Hay que hacer una instalación limpia desde cero perdiendo usuarios y datos almacenados o se puede reinstalar sin perder la información?