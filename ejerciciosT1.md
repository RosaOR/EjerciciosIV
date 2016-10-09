#Ejercicios Tema 1

## Ejercicio 1.
### Consultar en el catálogo de alguna tienda de informática el precio de un ordenador tipo servidor y calcular su coste de amortización a cuatro y siete años.

Mirando por [pccomponentes](http://www.pccomponentes.com) he encontrado este servidor: 
[HP ProLiant ML310e G8 XE E3](http://www.pccomponentes.com/hp_proliant_ml310e_g8_xe_e3_1220_8gb_2tb.html)

Para calcula el coste de la armortización primero debemos saber cual es su coste sin IVA:


Su valor es de 738€, sin IVA su coste es de **609.92€** (La propia página nos lo muestra). 

**Amortización a 4 años**
Teniendo en cuenta una amortizació máxima de 25% cada año tomamos esto para los 4 años y obtenemos:
	-**Primer año**: 609.92€*0.25=152.48€
	-**Segundo año**: 609.92€*0.25=152.48€
	-**Tercer año**: 609.92€*0.25=152.48€
	-**Cuarto año**: 609.92€*0.25=152.48€
	-**Total**: 4*150.62€ = 609.92€

**Amortización a 7 años**
Para la amortización a 7 años podemos hacer como en el anterior caso o tambien coger un gasto con digitos descendentes (ya que un ordenador cada año que pasa pierde valor) como por ejemplo así:

	-**Primer año**: 609.92€*0.25=152.48€
	-**Segundo año**: 609.92€*0.25=152.48€
	-**Tercer año**: 609.92€*0.15 = 91.488€
	-**Cuarto año**: 609.92€*0.15 = 91.488€
	-**Quinto año**: 609.92€*0.10 = 60.992€
	-**Sexto año**: 609.92€*0.05 = 30.496€
	-**Septimo año**: 609.92€*0.05 = 30.496€
	-**Total**: 152.48€*2 + 91.488€*2 + 60.992€ + 30.496€*2 = 609.92€

##Ejercicio 2.

### Usando las tablas de precios de servicios de alojamiento en Internet y de proveedores de servicios en la nube, Comparar el coste durante un año de un ordenador con un procesador estándar (escogerlo de forma que sea el mismo tipo de procesador en los dos vendedores) y con el resto de las características similares (tamaño de disco duro equivalente a tranferencia de disco duro) en el caso de que la infraestructura comprada se usa sólo el 1% o el 10% del tiempo.

He encontrado estas dos páginas con estos precios en los que sus procesadores son parecidos. 
![](https://github.com/RosaOR/EjerciciosIV/blob/Ejercicios-T1/t1-2.JPG)

En 1and1 podemos encontrar un servidor virtual con CPU 4vCores, 4GB de RAM y disco duro de 300GB y tráfico ilimitado por 20€ al mes unos 240€ al año.


![](https://github.com/RosaOR/EjerciciosIV/blob/Ejercicios-T1/T1-2a.JPG)

En axarnet.es con CPU de 4 cores, 4GB de RAM y Tráfico ilimitado por 14.98€ al mes, que seria unos 179.76€

**Usando sólo el 1% del tiempo**
 0.03€/hora*24h*30dias*1% =0.23€/mes 
 0.029€/hora*24h*30dias*1% = 0.21€/mes

**Usando sólo el 10% del tiempo**

 0.03€/hora*24h*30dias*10% = 2.16€/mes
 0.029€/hora*24h*30dias*10% = 2.1€/mes

##Ejercicio 3
### ¿Qué tipo de virtualización usarías en cada caso?
[Comentado en el foro](https://github.com/JJ/IV16-17/issues/1#issuecomment-252452205)

##Ejercicio 4
###Comprobar si el procesador o procesadores instalados tienen estos flags. ¿Qué modelo de procesador es? ¿Qué aparece como salida de esa orden?

Al poner el comando que nos pide no obtengo ningun resultado, por lo que no los tiene instalados o los tiene desactivados:
![](https://github.com/RosaOR/EjerciciosIV/blob/Ejercicios-T1/t1-ej4.png)

Con cat /proc/cpuinfo obtenemos:
![](https://github.com/RosaOR/EjerciciosIV/blob/Ejercicios-T1/t1-4%281%29.png)


##Ejercicio 5
### 1. Comprobar si el núcleo instalado en tu ordenador contiene este módulo del kernel usando la orden kvm-ok.
No lo tenia instalado, así que realicé la instalación oportuna y despues comprobé que ya sí que estaba instalado.

![](https://github.com/RosaOR/EjerciciosIV/blob/Ejercicios-T1/T1-5.png)

###2. Instalar un hipervisor para gestionar máquinas virtuales, que más adelante se podrá usar en pruebas y ejercicios.

Voy a utilizar virtualbox.



