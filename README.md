# Práctica Procontacto
Estas son las respuestas a los ejercicios de la páctica técnica para la vacante TP Developer.

**Ejercicio 1**

Ambiente Instalado.


![VScode](https://user-images.githubusercontent.com/61851810/164850775-94da7ee5-7c04-49d4-a3af-6d785b413113.jpg)



![Git](https://user-images.githubusercontent.com/61851810/164851161-2333fdc6-83bc-401c-88cb-e86f94503301.jpg)


**Ejercicio 2**

1.	¿Qué es un servidor HTTP?

	Es un software que se utiliza para proporcionar archivos a sitios de internet, es responsable de garantizar la comunicación entre servidor y cliente y también funciona como enlace entre dos máquinas. 

2.	¿Qué son los verbos HTTP? Mencionar los más conocidos.

	Son indicaciones al servidor sobre que es lo que se debe de hacer con los datos identificados con la URL.
	Los verbos más conocidos son GET y POST.

3.	¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?

	**Request.** Es una solicitud o petición que envía el cliente.
	
	**Response.** Es la respuesta a una petición del servidor web. 
	
	**Headers.** Son parámetros que se envían en una petición o respuesta HTTP al cliente o al servidor y proporcionan información esencial sobre la transacción en curso. 

4.	¿Qué es un queryString? (En el contexto de una url)

	Es una sección de la URL que contiene los datos que debe de pasar a las aplicaciones web.

5.	¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?

	Es un número que indica el estatus de la petición y tienen diferentes significados de acuerdo al valor devuelto. 
	Hay respuestas informativas, satisfactorias, redirecciones, errores en los clientes y errores en los servidores.

6.	¿Cómo se envía la data en un Get y cómo en un POST? 

	**GET:** *www.ejemplo.com/registro.php?nombre=maria&;apellido=diaz&;correo=maria@correo.com*
	
	**POST:**  Envía datos al servidor de manera oculta y el valor devuelto depende del header.
	
7.	¿Qué verbo http utiliza el navegador cuando accedemos a una página?

	GET

8.	Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.

	**JSON:** Es un formato de texto para almacenar y transportar datos, se trata de un subconjunto de la notación de objetos de JavaScipt
	
	Ejem.
	
	```JSON
	    {
	    "squadName": "Super hero squad",
	    "homeTown": "Metro City",
	    "formed": 2016,
	    "secretBase": "Super tower",
	    "active": true,
	    "members": [
		{
		"name": "Molecule Man",
		"age": 29,
		"secretIdentity": "Dan Jukes",
		"powers": [
		    "Radiation resistance",
		    "Turning tiny",
		    "Radiation blast"
		]
		},
		{
		"name": "Madame Uppercut",
		"age": 39,
		"secretIdentity": "Jane Wilson",
		"powers": [
		    "Million tonne punch",
		    "Damage resistance",
		    "Superhuman reflexes"
		]
		},
		{
		"name": "Eternal Flame",
		"age": 1000000,
		"secretIdentity": "Unknown",
		"powers": [
		    "Immortality",
		    "Heat Immunity",
		    "Inferno",
		    "Teleportation",
		    "Interdimensional travel"
		]
		}
	    ]
	    }
	```

	**XML:** Es un lenguaje de marcación extensible, y fue diseñada para almacenar y transportar datos.
	
	Ejem.
	
	```xml
	<message>
		<warning>
			Hola, mundo
		</warning>
	</message>
	```


9.	Explicar brevemente el estándar SOAP.

	Es un estándar que basado en XML para la transmisión de mensajes HTTP y otros protocolos de internet.
	Se necesitan un "contrato" que se le conoce como WSDL para poder hacer la transferencia de datos de lo contrario no se puede hacer dicha transferencia.
	Tanto como cliente y servidor deben tener ese contrato para poder saber que datos se deben mandar, que tipos etc. Tanto si vas a crear un servicio o consumirlo siempre se va a necesitar definir ese contrato.
	Y el manejo de datos es exclusivamente en XML.

10.	Explicar brevemente el estándar REST Full.

	Como característica principal es que están pensados para ser ligeros y más rápidos de los servicios SOAP.
	Estos no necesitan un contrato para ser consumidos, pero si obedecen reglas.
	Por ejemplo, que tipo de datos se deben usar, estos pueden usar HTML, XML, texto sin formato y JSON.
	El lenguaje más popular para su uso es Json.
	Hace uso de métodos también conocidos como verbos para indicar el tipo de operación que vamos a realizar sobre los recursos que nos ofrecen los servicios web.

11.	¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?

	Son parámetros que se envían al servidor para indicar la información básica (método HTTP, URL y versión). 
	
	El Content-type se utiliza para determinar el tipo MIME del recurso.

**Ejercicio 3**

1.	Realizar un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

 ![get-url](https://user-images.githubusercontent.com/61851810/164852247-2739195e-1fbe-4bd8-9193-0fb12778495f.png)

2.	Realizar un request POST a la URL anterior, y con body.

![post-url](https://user-images.githubusercontent.com/61851810/164852465-0e37d57c-4b47-4f50-9296-d88f461aaf57.png)

3.	Realizar nuevamente un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

![get2-url](https://user-images.githubusercontent.com/61851810/164852850-d10d762d-461a-4f4b-8e4a-ced38ba70ee5.png)

¿Qué diferencias se observan entre las llamadas el punto 1 y 3?

En el primer punto muestra la información que tiene la URL y en el tercer punto muestra la información incluyendo mis datos.

**Ejercicio 4**

https://trailblazer.me/id/mdazgordillo

**Ejercicio 5**

1.	Lead. Es donde se almacena información de los clientes prospecto. No tiene relación con ninguno de los demás objetos.
2.	Account. Es donde se almacena información de una organización, empresa o consumidor al que se le desea realizar un seguimiento (cliente, socio).  
3.	Contact. Son los datos de la persona asociada a una cuenta.
4.	Opportunity. Es donde se almacenan información relacionada con un intento de cliente potencial.  
5.	Product. Es donde se almacena la información de los servicios o artículos que ofrece la empresa.
6.	PriceBook. Es donde se almacena la lista de productos y sus precios.
7.	Quote. Es donde se almacena la información de los precios propuestos para cada servicio o producto.
8.	Asset. Es donde se almacena la información de productos comprados por los clientes.
9.	Case. Es donde se almacena la descripción detallada de los problemas de un cliente. Se utiliza para identificar y resolver los problemas.
10.	Article. Son documentos informativos.


![Diagrama](https://user-images.githubusercontent.com/61851810/164855202-91b183ed-48a3-4d1d-871f-c6bf6be48914.jpg)


![acc-contact](https://user-images.githubusercontent.com/61851810/164856472-198e5371-54e3-4af3-b01a-a901d8d51091.jpg)
![acc-opp](https://user-images.githubusercontent.com/61851810/164856485-480faca7-0fb7-4c99-8d1e-a2cbff9e8a1b.jpg)
![asset-case](https://user-images.githubusercontent.com/61851810/164856494-f17b88ba-be7e-437e-a802-44c8df905c15.jpg)
![contact-asset](https://user-images.githubusercontent.com/61851810/164856502-bf5842d3-437d-4c6d-b1f9-8dcbb61cdeb1.jpg)
![contact-case](https://user-images.githubusercontent.com/61851810/164856508-849e5a3b-0ddc-47d9-8d3e-8f920b966575.jpg)
![prod-asset](https://user-images.githubusercontent.com/61851810/164856514-dfaabdb9-355c-4ac1-baac-80ac1ac3ee7c.jpg)
![acc-asset](https://user-images.githubusercontent.com/61851810/164856519-e91b9933-203b-4ba0-978f-7a1fc9c2b09a.jpg)
![acc-case](https://user-images.githubusercontent.com/61851810/164856525-702471f1-5bdc-4180-af00-468fe9e2d92a.jpg)


**Ejercicio 6**

***Soluciones de Salesforce***

A.	¿Qué es Salesforce?

Es una solución basada en la gestión de hacer relaciones con clientes y después empresas. Es una plataforma CRM.
	
B.¿Qué es Sales Cloud?

Es una aplicación basada en la nube y tiene la intención de ayudar a los vendedores a vender de una manera más rápida e inteligente.
	
C.¿Qué es Service Cloud?

Es una solución que permite a los usuarios automatizar procesos de servicio al cliente.
	
D. ¿Qué es Health Cloud?

Es una solución para gestionar las relaciones con el paciente.
	
E. ¿Qué es Marketing Cloud?

Es una plataforma de marketing digital para gestionar la interacción de la marca con sus clientes.

***Funcionalidades de Salesforce***

A. ¿Qué es un RecordType?

Son los tipos de registro que permite a la plataforma hacer diferentes procesos.

B. ¿Qué es un ReportType?

Es un conjunto de registros disponibles basados en las relaciones entre objeto principal y sus objetos relacionados.

C. ¿Qué es un Page Layout?

Son los diseños de las páginas de detalle y edición de la organización. 

D. ¿Qué es un Compact Layout?

Es un diseño más pequeño donde muestran los campos clave de algún registro en la aplicación móvil de Salesforce.

E. ¿Qué es un Perfil?

Es la asignación que se le da al usuario donde se especifica cómo y qué puede hacer en la aplicación.

F. ¿Qué es un Rol?

Es la asignación que se le da a un usuario donde se especifica qué es lo que puede ver dentro de su organización.

G. ¿Qué es un Validation Rule?

Es una regla de validación donde se verifica que cuando los datos que ha introducido un usuario cumplan con las reglas previamente especificadas.

H. ¿Qué diferencia hay entre una relación **Master Detail** y **Lookup**?

Que el master detail tiene una dependencia directa entre dos objetos (padre-hijo) y es muy limitada la relación maestro-detalle y el Lookup es cuando solo necesitas tener la relación entre dos objetos pero no una dependencia entre ellos.

I. ¿Qué es un Sandbox?

Es una copia de la información de tu organización en producción a entornos de pruebas.

J. ¿Qué es un ChangeSet?

Son conjuntos de cambios que envían personalizaciones de una organización a otra.

K. ¿Para qué sirve el import Wizard de Salesforce?

Sirve para la importación de datos de una manera más sencilla.

L. ¿Para qué sirve la funcionalidad Web to Lead?

Para almacenar información capturada mediante un formulario web y convertirlo a un cliente potencial.

M. ¿Para qué sirve la funcionalidad Web to Case?

Para capturar casos desde un sitio web y enviarlos directamente a su instancia de Salesforce.

N. ¿Para qué sirve la funcionalidad Omnichannel?

Para proporcionar todos los elementos necesarios para ayudar a los agentes o gestores a ofrecer un mejor servicio al cliente, proactivo en todos los canales y dispositivos.

O. ¿Para qué sirve la funcionalidad Chatter?

Es una aplicación de colaboración en tiempo real que permite a sus usuarios trabajar en conjunto y compartir información.

***Conceptos generales***

A. ¿Qué significa SaaS?

Es un modelo de entrega de software basado en la nube en el que el proveedor desarrolla y mantiene el software de las aplicaciones en la nube, proporciona actualizaciones automáticas del mismo y lo pone a disposición de sus clientes a través de Internet.

B. ¿Salesforce es Saas?

Salesforce sí es SaaS.

C. ¿Qué significa que una solución sea Cloud?

Que se pueden almacenar y administrar las bases de datos, procesos y operaciones en servidores remotos y después permitir el acceso a esa información de a través de internet.

D. ¿Qué significa que una solución sea On-Premise?

Se refiere al tipo de instalación local de una instalación de software. Esta instalación se lleva a cabo dentro del servidor y la infraestructura (TIC) de la empresa.

E. ¿Qué es un pipeline de ventas?

El proceso de actividades y estrategias que necesita un vendedor para acelerar el ciclo de ventas, transformando clientes potenciales en clientes.

F. ¿Qué es un funnel de ventas?

Es un sistema diseñado para atraer a desconocidos, convertirlos en leads y transformarlos en clientes.

G. ¿Qué significa Customer Experience?

Es la forma de generar una relación entre consumidor y marca.

H. ¿Qué significa omnicanalidad?

Es una estrategia de comunicación orientada a la atención del cliente.

I. ¿Qué significa que un negocio sea B2B? ¿Qué significa que un negocio sea B2C? ¿Qué es un KPI?

B2B. Que son las ventas de un negocio a otro.
	
B2C. Que el negocio vende de forma directa al consumidor final.
	
KPI. Son indicadores de desempeño y hacen referencia a una serie de métricas que se utilizan para simplificar la información y poder hacer toma de decisiones.

J. ¿Qué es una API y en qué se diferencia de una Rest API?

Es que API es un conjunto de definiciones y protocolos que se usa para diseñar e integrar el software de las aplicaciones y Rest API es un estilo arquitectónico para aplicaciones en red basadas en cliente-servidor.

K. ¿Qué es un Proceso Batch?

Es el proceso mediante el cual una computadora completa lotes de trabajos, de forma simultáneamente, en orden secuencial y sin interrupción.

L. ¿Qué es Kanban?

Es un método de gestión de trabajo.

M. ¿Qué es un ERP? 

Es un sistema de planificación de recursos empresariales.

N. ¿Salesforce es un ERP?

No.

#Ejercicio 7


A.	Consultar tu ID haciendo un GET con POSTMAN a este WS:

https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

	},
		"-N07HT6ufgJAJQUbsG0y": {
		"email": "maria.diaz@procontacto.com.mx",
		"name": "María"
	}
	
B.	Agregar un campo al objeto Contact llamado idprocontacto de tipo texto de 255 caracteres. 


![addcont-sf](https://user-images.githubusercontent.com/61851810/164856859-f7fdbde0-e058-491e-bef9-e00831b9cb9c.jpg)

C.	Desarrollar un trigger para que cuando un usuario Modifica o Crea un contacto de Salesforce completando el campo generado el punto B con TU id obtenido en el punto A, se invoque al Web Service con el idprocontacto obtenga los datos de email de la respuesta y actualice el campo email del contacto. Usar Playground 1. 




