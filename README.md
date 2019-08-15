# **APLICACIÓN DE VEHÍCULOS**

### **Descripción:**
Esta aplicación está enfocada en el registro de vehículos con sus características y su respectivo dueño. Las diferentes funcionalidades implementadas están protegidas por un login por URL, el cual es fundamental para poder acceder a ellas. Dentro de la aplicación se pueden encontrar las funcionalidades de registrar un vehículo con su respectivo dueño, listar todos los vehículos ya registrados y mostrar unas estadísticas de los vehículos de acuerdo a sus marcas.

### **Instrucciones de instalación:**
- La aplicación debe ser montada en un servicio Apache con MYSQL o similar. 
- Luego de clonar el repositorio, modificar el archivo .env con el nombre de la base de datos, usuario de la base de datos y contraseña correspondientes.
- Después, es necesario abrir el CMD, ubicarse en la ruta del proyecto y escribir los siguientes comandos:
	'composer install'


### **Instrucciones de uso:**
Al iniciar la aplicación se debe poner en la URL la ruta "/A765" como código de verificación para el login y poder así, acceder a las funcionalidades que ésta trae. De otro modo, cualquier otra ruta que se coloque para la aplicación tendrá como resultado una página que dice "Zona prohibida".

<img src="/public/img/zona.PNG" alt="zona"
	title="Zona Prohibida"/>
  
Después de haber iniciado sesión, aparecerá una página con unos botones que llevan a cada funcionalidad. 

<img src="/public/img/enlaces.PNG" alt="enlaces"
	title="Enlaces"/>

En el primer botón se encuentra la funcionalidad de Registrar Vehículos. Este nos llevará a una página donde se debe deben llenar los campos de Placa del vehículo, Marca del vehículo, Cédula del dueño, Nombre del dueño y Apellidos del dueño. Luego se presiona el botón "Registrar" para guardar en la base de datos.

<img src="/public/img/registrar.PNG" alt="registrar"
	title="Registrar"/>

En el segundo botón encontramos la funcionalidad de Listar Vehículos. Este nos llevará a una página donde encontraremos una tabla con todos los vehículos registrados con la cédula del correspondiente dueño. Además, se muestra la placa del vehículo y su marca.

<img src="/public/img/listar.PNG" alt="listar"
	title="Listar"/>

En el tercer botón encontramos la funcionalidad de Estadísticas de Vehículos. Este nos llevará a una página donde encontraremos el conteo estadístico de cuántos vehículos hay de cada marca en específico.
