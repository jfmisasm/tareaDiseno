# **Layered Pattern!**

También llamado patrón de arquitectura por  capas, es una de las técnicas más comúnes que los arquitectos de software utilizan para dividir sistemas de software complicados. Al pensar en un sistema en términos de capas, se imaginan los principales subsistemas de software ubicados de la misma forma que las capas de un pastel, donde cada capa descansa sobre la inferior. En este esquema la capa más alta utiliza varios servicios definidos por la inferior, pero la ultima es inconsciente de la superior. Además, normalmente cada capa oculta las capas inferiores de las siguientes superiores a esta.

[LayeredArquitecture](https://www.google.com/search?q=layered+pattern&client=opera&hs=G5K&source=lnms&tbm=isch&sa=X&ved=0ahUKEwinkuXu84LkAhUl11kKHTisDU8Q_AUIESgB&biw=1473&bih=706#imgrc=aoEsrrw4jgZ1EM:)

## Capas Principales

### 1. Capa de Presentación 
		Referente a la interacción entre el usuario y el software.  Puede ser tan simple como un menú basado en líneas de comando o tan complejo como una aplicación basada en formas.  Su principal responsabilidad es mostrar información al usuario, interpretar los comandos de este y realizar algunas validaciones simples de los datos ingresados.

### 2. Capa de Reglas de Negocio (Empresarial): 
		También denominada Lógica de Dominio, esta capa contiene la funcionalidad que implementa la aplicación.  Involucra cálculos basados en la información dada por el usuario y datos almacenados y validaciones.  Controla la ejecución de la capa de acceso a datos y servicios externos.  Se puede diseñar la lógica de la capa de negocios para uso directo por parte de componentes de presentación o su encapsulamiento como servicio y llamada a través de una interfaz de servicios que coordina la conversación con los clientes del servicio o invoca cualquier flujo o componente de negocio.

### 3. Capa de Datos: 
		Esta capa contiene la lógica de comunicación con otros sistemas que llevan a cabo tareas por la aplicación.  Estos pueden ser monitores transaccionales, otras aplicaciones, sistemas de mensajerías, etc.  Para el caso de aplicaciones empresariales, generalmente esta representado por una base de datos, que es responsable por el almacenamiento persistente de información.  Esta capa debe abstraer completamente a las capas superiores (negocio) del dialecto utilizado para comunicarse con los repositorios de datos (PL/SQL, Transact-SQL, etc.).


## Beneficios
Los beneficios de trabajar un sistema en capas son:

	– Se puede entender una capa como un todo, sin considerar las otras.
	– Las capas se pueden sustituir con implementaciones alternativas de los mismos servicios básicos
	– Se minimizan dependencias entre capas.
	– Las capas posibilitan la estandarización de servicios
	– Luego de tener una capa construida, puede ser utilizada por muchos servicios de mayor nivel.

