# **Manual técnico**
### **Objetivos**
* Desarrollar un sistema de marcaje con capacidad de reportería.
* Diseñar un sistema de marcaje de entrada/salida, CRUD de empleados e historial. 
### **Alcance**
#### Fundamentar o consolidar los temas vistos anteriormente en clase para mejorar la compresión sobre backedn, frontend lenguajes de programación, estructurado y uso de otras herramientas.
### **Instalacion del sistema**
* PostgreSQL 15 y DBeaver
* Oracle linux 9
* Firabase para autenticacion
* Visual studio 2022 (Angular)
* Visual studio code 1.72.2 (C#)
* OpenVPN
### **Diagrama de base de datos PostgreSQL 15**
#### Después de un análisis se desarrollo el siguiente diagrama para manejar el control de marcaje, departamentos y las diferentes consultas que necesitaremos manejar el sistema. Realizando cuatro tablas usuario, empleado, departamento, historial_emp con sus diferentes atributos.
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/diagramadb.jpg)
### **Oracle linux 9 alojamiento de base de datos**
#### Se configura Oracle Linuz 9 para alojar la base de datos "proyectotres" el cual contiene todos nuestro gestor de BD el cual funciona como servidor para ello configuaramos que pueda tener acceso a ciertas ip o bien lo podemos habilitar para cualquier usuario aunque esto no es seguro. Configuramos puerto de PostgresSQL y ya se encuentra la conexion de nuestra base datos a dbeaver mediente la ip y el usuario. 
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/alojamiento.jpg)
### **Vizualizacion de datos ingresados a la base de datos**
#### Para comprobar que si se esta manteniendo conexion mediante ip mostramos la comparativa para visualizar que se encuentran todas las tablas y los siguientes datos ingresados. 
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/tablas.jpg)
#### Tabla de Departamento
![departamento](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/departamento.jpg)
#### Tabla de Usuario y Empleado
![usuarioempleado](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/usuarioempleado.jpg)
#### Tabla de Historial_emp
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/historialemp.jpg)
### **VPN con OpenVPN**
#### Nos registramos en OpenVPN el cual nos brinda el servicio para poder realizar conexión máxima de 3 usuarios. 
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/OPENVPN.jpg)
#### Registramos a los usuarios a los cuales les permitiremos la conexion desde OpenVPN para que puedan tener comunicación las maquinas por medio de ip's que en este caso se encuentran la conexión en modo offline es decir el servicio de line se encuentra apagado.
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/usuariosvpn.jpg)
#### Realizamos conexion por medio de la aplicacion OpenVPN Connect instalada en nuestra pc y cada uno de los usuarios de igual manera deben de tenerla en su sistema para poder obtener comunicación. Nos logueamos y realizamos las configuraciones necesarios para poder obtener la conexion y que ya podamos hacer uso de nuestras ip generadas.
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/conexion.jpg)
#### En listado de usuarios este cambiará en linea y asi cada usuario el cual ya este logueado y este realizando una conexion. De esta manera realizamos para poder tener conexion de los otros usuario y poder realizar que cada uno contenga una parte del usario para que pueda duncionar.
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/enlinea.jpg)
#### Colocamos la ip y esta ya tendra conexión en este caso del otro usuario el cual esta registrado en el OpenVPN. Y carga nuestro aplicativo para ser funcional.
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/ip.jpg)
### **Autentiecacion mediante Firabase**
#### Firabase es una plataforma la cual nos facilita el uso de autenticacion para el desarrollo de nuestra aplicaciones web, para utilizarla realizamos el logueo y creamos un nuevo proyecto en el que realizamos todas nuestras configuraciones adecuadas para que este fuese funcional del lado de nuestro backend y frontend de forma correcta. 
![diagrama](https://github.com/Keillie/Proyecto-3-DW/blob/main/src/assets/firabase.jpg)
### **Conclusiones**
#### Se desarrollo un sistema de marcaje con reportería mediante el uso de diferentes herramientas implementadas para realizar una mejor presentacion del aplicativo web, de igual manera se realizo el analisis adecuado para el funcionamiento de la base de datos con el backend y frontend, entre otras varias configuraciones que se realizaron. Como futuros ingenieros este proyecto fue de mucho aprendizaje, tanto en el uso de autenticaciones, la reporteria para generar pdf, el uso de VPN, etc. 
