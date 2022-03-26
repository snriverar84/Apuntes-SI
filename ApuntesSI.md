# Apuntes SI

https://fagonzalezo.github.io/iis-2022-1/

Clases presenciales 1 dia por semana - Los miercoles

Hoy 14 de marzo, ya toca leer lo de la semana 1, para la siguiente semana lo de la semana 2
Entregas por file request. Este es el grupo 1
En SI que coños es un transformer??
que es CODEX?
para el miercoles de la otra semana video 1, video 2, capitulo 2 rossen
	practica 2: Note de pyton (colab): dESARROLARLO en ayuda de la libreria del libr de rossen, hay un github con librerias
	Igual ahi aparece en la pag del curso, 14 a 21
	
	En el PDF que descargue, el cap 21 esta en la pag 1378
	
	
	Video 1 S1:
	Inteligencia artifical -> Racionalidad Computacional:
							Alcanzar de manera optima los objetivos definidos
							Objetivo -> Funcion de utilidad
							Actuar racionalmnte: Maximizar la actividad
	
	Areas de la IA:
		- Reprsentacion del conocimiento - Razonamiento
		- Aprenizaje computacional -> 80% del curso
		- Planeacion
		- Precepcion
		- Lenguaje
		- Robotica
		. 
	Agente: Entidad que percibe actos
		
	Semana 2
	
	Video 1
	
	Agentes y ambientes.
	El enfoque de la IA va a ser hacia los agentes. Cuando se construye un sistema inteligente se construye un agente inteligente.
	El agente es un sistema fisico o de software que recibe percepciones a traves de sensores y ejecuta acciones a partir de actuadores.
	Las percepciones las recibe de un ambiente y en ese ambiente ejecuta las acciones. 
	Los agentes se define como una funcion
						F : P* -> A
						La funcion recibe una secuncia de percecpciones (P*) y a partir de esas entradas genera unas 
						acciones (salida)
		Un agente racional es aquel que escoje cualquier accion que maximiza el valor esperado de la medida de desempeño dada la secuencia 
		de percepciones a la fecha
			- El agente no es onminicnete: Hace lo mejor que puede con la información que tiene
			- No es clarividente: No sabe de antemano que va a pasar
			Para desarollar un agente intelignete se debe especificar el ambiente de desempeño, entonces un agente requiere:
				- Medida de desempeño
				- Ambiente
				- Actuadores
				- Sensores

## Video 2 semana 2

![image](https://user-images.githubusercontent.com/36849580/160250293-61328ddf-9ece-4788-87d6-305b675f3a70.png)


Agentes reflejos: Eligen sus acciones de acuerdo a lo que están percibiendo

- Tiene memoria en el estado acutal del mundo, pero no considera las consecuencias de sus acciones futuras
- Reglas de agente pacman: * Si tiene una galleta al frente, se la come. En el segujndo ejemplo si no tiene una galleta al frente (hay espacios) se queda quieto y no avanza:
	
	![image](https://user-images.githubusercontent.com/36849580/160250758-3cce91bd-9f5e-4372-acf2-e39e88c5df39.png)

- La alternativa es un agente que planea: Que pasa en el mundo si se ejecuta una acción
	Para esto se necestia un modelo del mundo y un objetivo
	
### Problema de busqueda: 
	Un problema de busqueda es un  espacio de estdos
	![image](https://user-images.githubusercontent.com/36849580/160253154-18e0613c-74bc-4f3d-b9e3-1d9f57738cce.png)
	
	Que elementos hay?
	- Estados
	- Funcion Sucesora
	
	Cuantos estados hay:
		2^9 : Porque? Pues porque hay 2 estados, hay o no hay galleta y 9 posibles posiciones
		Pero esto toca multiplicaro por 9m que son las posibles posiciones del pacman: 2^9 * 9
		Pero a esto adicionalmente toca sumarle la orientacion del pacman, que son 4, entonces
			2^9 * 9 * 4
		D ehecho, se ajusta a 2^8 porque el poacman ya esta ocupando una posicion, entonces seria
			2^8 * 9 * 4
	Funcion sucesor:
		Cuando estoy en un estado particular, que pasa con mis acciones
	Estado inicial y estado final
		Donde empiezo y a donde quiero llegar
	
	![image](https://user-images.githubusercontent.com/36849580/160253538-953a1fcb-59d4-46c5-b7e4-d0486a3c07ba.png)

		
