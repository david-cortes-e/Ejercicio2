# Ejercicio2    Cortés E. David
## **Programa para taller mecánico** :car:
#### Descripción
Este proyecto tiene como objetivo crear un programa que permita administrar de buena manera un taller mecánico.
Dicho programa tiene como eje central una ***interfaz amigable*** tanto para el administrador como para el usuario común.

Las partes del programa son:
* Autos en reparación :wrench:
  - Fecha de ingreso
  - Presupuesto
  - Fecha de egreso
* Lista de clientes :couple:
  - clientes frecuentes
  - colaboradores
  - agencias
* Facturación :moneybag:
  -facturas cobradas
  -facturas pendientes
* Otros :question:

#### Portada
Las propuestas de imagen de portadas del programa son las siguiente:

### Primer imagen

![imagen1.](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS-c9flpEkwl4rlHonbuc-BZ-pP2Dlnq0Wv1g&s)

### Segunda imagen

![imagen2](https://github.com/user-attachments/assets/80ea7e91-e29e-4a06-b493-dd80d7fd1e3c)



### Elaboración del programa

El programa será hecho en C#.
A continuación se muestra un ejemplo del codigo empleado.

```
using System;


class Persona{
	private string nombre;
	private string apellidoPaterno;
	private string apellidoMaterno;
	private int edad;

	public Persona(){}

	public Persona(string nombre,string apellidoPaterno,string apellidoMaterno,int edad){
		this. nombre=nombre;
		this.apellidoPaterno=apellidoPaterno;
		this.apellidoMaterno=apellidoMaterno;
		this.edad=edad;
	}

	public string Nombre{
		get{ return this.nombre;}
		set{ this.nombre=value;}
	}

	public string ApellidoPaterno{
		get{ return this.apellidoPaterno;}
		set{ this.apellidoPaterno=value;}
	}

	public string ApellidoMaterno{
		get{ return this.apellidoMaterno;}
		set{ this.apellidoMaterno=value;}
	}

	public int Edad{
		get{ return this.edad;}
		set{ this.edad=value;}
	}


}
class Abuelo: Persona{
	private string id_carnet;
	public Abuelo(){}

	public Abuelo(string nombre,string apellidoPaterno,string apellidoMaterno,int edad,string id_carnet): base(nombre,apellidoPaterno,apellidoMaterno,edad){
		this.id_carnet=id_carnet;
	}

	public string Id_Carnet{
		get{ return this.id_carnet;}
		set{ this.id_carnet=value;}
	}
}
```
