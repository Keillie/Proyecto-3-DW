# **Manual de usuario de maracaje**

### **Introduccion**
#### En este proyecto se nos indicó realizar un sistema de marcaje web en el cual colocamos en práctica cada una de las enseñanzas vistas en clases e investigaciones de herramientas para desarrollar nuestras habilidades en el área de desarrollo web. Este consiste en realizar un marcaje de hora y salida de empleados según este ingrese teniendo el control de sus horarios de igual manera nos permite la realización de reportes respecto al marcaje según departamento, general, individual, etc. Este tipo de sistemas ayudan a cualquier tipo de empresa para llevar un mejor control de sus empleados y saber si cumplen con los horarios fijados al realizar reportes. El desarrollo de este proyecto nos permitió desarrollar nuestras diferentes habilidades en el área de desarrollo web de igual manera aprender sobre las autenticaciones, el uso de diferentes sistemas operativos como lo es el caso de Oracle Linux, Ubuntu, etc., también el uso de sistemas de gestores de base de datos.

### **Instalacion del sistema**
* PostgreSQL 15 y DBeaver
* Oracle linux 9
* Firabase para autenticacion
* Visual studio 2022 (Angular)
* Visual studio code 1.72.2 (C#)
* OpenVPN

### **Guia de uso**
___
***Registro de un empleado***
#### Se lanza la primera vista y para registrarnos damos clic en “Registrarse lo que nos redirecciona a la siguiente página.
![login](src\assets\login.png)
#### Tenemos la siguiente vista donde se nos indica colocar nuestros datos los primero es colocar nombre completo, apellidos completo, DPI, usuario que es el dato con el cual nos vamos a loguear en login, password y confirmación del password para verificar que sea el mismo y por último el botón de “Aceptar” para guardar cambios realizados. Ingresasmos nuestros datos en este caso para ejemplo las siguientes credenciales:
![login](src\assets\registrarse.png)
#### Colocamos datos y ya funcionaria de forma correcta enviándonos a la siguiente vista de inicio y realizamos un logueo con normalidad este hace uso de la autenticacion para validar y tambien busca en base de datos si existe tal usuario.
![login](src\assets\logueo.png)
___
***Ingreso al login de un usuario empleado***
#### Tenemos la primera pantalla de login la que nos indica que debemos ingresar al sistema con nuestras credenciales, colocamos los datos de usuario y password, en este caso si nos hemos equivocado en un dato de ingreso mostrara un mensaje en rojo esto significa que son incorrectos y realiza dicha autenticacion, no existe nuestro usuario en la base de datos y por lo tanto no estamos registrados, viéndose de la siguiente manera.
![login](src\assets\logueoinvalido.png)
#### Ingresamos de nuevo al sistema con los datos del usuario empleado correctamente, damos clic en “Aceptar” al ser correctos de forma automática nos enviara a la siguiente vista de marcaje y nos mostrara un mensaje en la parte superior derecha indicando bienvenido y la autenticacion correcta.
![login](src\assets\logueoexitoso.png)
#### Vista al dar aceptar e ingresar de forma correcta.
![login](src\assets\marcaje.png)
#### Ingresados al sistema tendremos un título de marcaje y un botón en la parte de abajo que indica “marcar” en la que el usuario al dar clic iniciara su primer marcaje pudiendo realizar el control de su entrada, este indicara la hora y fecha en que este realizando dicha acción.
![login](src\assets\realizandomarcaje.png)
#### Para indicar salida nuevamente debe marcar y quedara registrado este marcacion sera en el minuto 15:47pm.
#### Para salir tenemos un link en la parte superior del lado derecho en el que aparece “Salir” que al dar clic nos regresa a la pantalla principal del login.
![login](src\assets\salir.png)
___
***Ingreso de un administrador***
#### Un usuario administrador ingresa de la misma manera que un empleado en la pantalla aparece un input lo cual indica un espacio de usuario y otro para password, un botón en la parte de abajo que indica “Aceptar” para continuar el programa si este es correcto y en caso de ser incorrecto se veria como se mostró anteriormente. Se ingresan datos de forma correcta realiza autenticacion e ingresa de forma correcta. 
![login](https://drive.google.com/file/d/16oWB3yFpjIw2CODWX-WwCkM67LsDu2c3/view?usp=sharing)
#### En esta area encontramos el area de reporteria el cual se genera al dar clic en un botón según nosotros indiquemos podemos generar el general de empleados, de llegadas tarde, de salidas anticipadas o antes de tiempo, etc. También veremos el historial de empleados y se presenta una tabla con el de id de cada empleado, nombres, apellidos, y opciones donde se encuentran tres “Ver horarios”, “Editar”, Eliminar” de las acciones que podemos realizar. Nos indicará un mensaje de bienvenido al sistema al ser todo correcto. 
![login](src\assets\historial.jpg)
#### Nos permite ver horarios de un usuario en especifico incluyendo el del mismo admin.
![login](src\assets\verhorario.png)
#### Tenemos el listado de opciones de reporteria el cual al dar clic en alguno de ellos nos abre otra pestaña generandonos un .pdf el cual nos da la posibilidad de descargar o vizualizar para tener un contexto general. Teniendo en ella la opción de un reporte general, reporte general tarde, reporte general salidas anticipadas. 
![login](src\assets\opciones.jpg)
#### Tambien se tiene el area de departamentos donde se puede tener vizualizar los departamentos que existen. 
![login](src\assets\departamentos.jpg)
___
### **Restricciones del programa**
* Funcional únicamente para empleados del sistema que este registrado.
* Realiza autenticación de quienes ingresan al sistema.
* El administrador es el unico autorizado o que tiene la opcion de realizar reporterias.
* El administrador es el único que tiene acceso al historial de cada empleado y de realizar, modificaciones, eliminar o ver los datos específicos de cada uno.
* El sistema puede ser visto unicamente por personas que esten registradas por el OpenVPN.
* El empleado o usuario únicamente puede realizar marcajes lo que es de entrada y salida cuantas veces realice cierta acción.
* No permite que el usuario normal realice más acciones que no sea el marcaje.
* Un usuario al ser eliminado por el administrador no se borra del sistema solo se deshabilita pasando a otro estado y no puede volver a loguearse nuevamente ya que esta desactivado.
### **Conclusiones**
#### Se desarrolla un sitio web con el fin de realizar un marcaje de empleados para tener el registro de sus ingresos y egresos de cada uno, teniendo roles lo cual el administrador es el único que puede tener el historial de cada empleado, realizar reporterías según las opciones que se tengan y de realizar CRUD’s, mientras que el empleado únicamente tiene la capacidad de registrarse y realizar marcajes. La realización de este proyecto nos permitió desarrollar y ahondar más sobre la realización de APIS, JWT, request y response, uso de VPN, familiarizarnos con otros sistemas operativos, teniendo el control sobre backend, frontend, base de datos, etc.
