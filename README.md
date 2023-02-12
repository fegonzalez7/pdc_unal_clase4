# Programación de Computadores - UNAL
## Problemas y algoritmos

## Problemas

<table cellspacing="1" bgcolor="">
	<tr bgcolor="#252582">
		<th><b>Definición</b></th>
	</tr>
	<tr bgcolor="#e4e4ed">
		<td style="color:#141414">Se tiene un problema cuando se desea <u>encontrar uno o varios objetos desconocidos</u> (ya sean estos números, símbolos, diagramas, figuras u otras entidades), que <u>cumplen condiciones o relaciones</u>, previamente definidas, respecto a uno o varios objetos conocidos o desconocidos.<br>
    Normalmente usan entradas (datos conocidos), se procesan a través de las condiciones/relaciones para hallar una salida (datos desconocidos).</td>
	</tr>
</table>

Cuál es el objetivo entonces:

<table cellspacing="1" bgcolor="">
	<tr bgcolor="#252582">
		<th><b>Solución de problemas</b></th>
	</tr>
	<tr bgcolor="#e4e4ed">
		<td style="color:#141414">Solucionar un problema es <b>encontrar</b> los objetos desconocidos.</td>
	</tr>
</table>

### Clasificación de problemas
+ **Condicionados:** Hace referencia a las condiciones y relaciones entre los objetos conocidos y desconocidos.
  + **Bien condicionados:** Si a partir de la entrada (no sobran ni faltan objetos conocidos) y a partir de la descripción de la relación (algunas veces llamada condición) entre la entrada y la salida se puede encontrar dicha salida. En los problemas bien condicionados se cuenta con la información necesaria para resolver el problema y la solución no depende de una elección personal de índole emocional.
  + **Mal Condicionados:** Son problemas en los cuales no se cuenta con la información necesaria para resolver el problema, o la respuesta está sujeta a una elección personal de cada ser humano (que depende de los sentimientos, emociones, cultura, religión, política, tradición, etc.)
+ **Solucionables:** Son problemas para los cuales existe una salida válida (se
puede encontrar) para la entrada dada.
  + **Computable:** Son problemas para los cuales existe una secuencia finita de pasos "bien definidos" que permiten describir la relación entre entrada y salida, y que al ser aplicados a la entrada terminan en algún momento produciendo la salida.
  + **Tratable:** Son problemas para los cuales los recursos (tiempo y espacio) que se necesitan para su solución son finitos y no crecen exponencialmente a medida que aumenta el tamaño de la entrada.
  + **Algoritmico:** Cuando un problema es computable , tratable y bien condicionado se denomina *algorítmico*.
+ **Indecidible:** Son problemas en los que no se sabe si existe una solución "computable" o "tratable". Este tipo de problemas no son el objeto del curso.

Tenemos algunos casos interesantes:

+ **No solucionable** != **Mal condicionado**:  En los problemas mal condicionados es posible que la relación no esté bien dada, no sea clara, sobren o falten objetos conocidos, mientras que en los no solucionables se tienen claras tanto la entrada como la relación entre .entrada y salida

+ **No solucionable** != **no tratable**: Los problemas intratables son solucionables cuando el tamaño de la entrada es pequeño, pero resultan no solucionables para entradas medianas y/o grandes.

### Ejemplos

1. Sean P=(a,b) y Q=(c,d) los puntos que definen un segmento de recta.
Encontrar un segmento de recta perpendicular al anterior, que pase por su punto medio.

<details><summary>Solución</summary><p>
<table cellspacing="3" bgcolor="">
	<tr bgcolor="#">
		<th><b>Elementos conocidos</b></th>
    <th>Los puntos P y Q.</th>
	</tr>
	<tr bgcolor="#">
		<th><b>Elementos desconocidos</b></th>
    <th>Un segmento de recta.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Condiciones</b></th>
    <th>El segmento de recta debe pasar por el punto medio entre P y Q, y debe ser perpendicular a la recta trazada entre P y Q</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Tipo de problema</b></th>
    <th>Solucionable - Algoritmico: 
    <br><b>Paso 1: </b> Trazar un círculo con centro en el punto P que pase por el punto Q. 
    <br><b>Paso 2: </b>Trazar un círculo con centro en el punto Q que pase por el punto P. <br><b>Paso 3: </b>Trazar un segmento de recta entre los puntos de intersección de las circunferencias trazadas en los pasos 1 y 2.</th>
	</tr>
</table>
</p></details><br>

2. De las siguientes cuatro imágenes, ¿cuál es la más llamativa?:
<div align='center'>
<figure> <img src="https://i.postimg.cc/bwwx1Wrn/image.png" alt="" width="650" height="auto"/></br>
<figcaption><b></b></figcaption></figure>
</div>

<details><summary>Solución</summary><p>
<table cellspacing="3" bgcolor="">
	<tr bgcolor="#">
		<th><b>Elementos conocidos</b></th>
    <th>Las 5 imágenes.</th>
	</tr>
	<tr bgcolor="#">
		<th><b>Elementos desconocidos</b></th>
    <th>La imagen más llamativa.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Condiciones</b></th>
    <th>La imagen buscada es la más llamativa para quien resuelve el problema.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Tipo de problema</b></th>
    <th>Solucionable - Mal condicionado <br>
    Se tiene bien detallada la entrada (las imágenes de la figura) y tener una salida (es una de las imágenes de la entrada), no se tiene una clara relación entre la entrada y la salida: la noción de llamativo depende de quien vea las imágenes y no se puede describir</th>
	</tr>
</table>
</p></details><br>

3. Un granjero tiene cincuenta animales entre conejos y gansos. Si la cantidad
de patas de los animales es ciento cuarenta, ¿cuántos conejos y cuántos gansos tiene el
granjero? (Asuma que solo hay gansos y conejos)

<details><summary>Solución</summary><p>
<table cellspacing="3" bgcolor="">
	<tr bgcolor="#">
		<th><b>Elementos conocidos</b></th>
    <th>La cantidad total de animales (50), cantidad de patas totales (150), número de patas de los gansos y número de patas de los conejos.</th>
	</tr>
	<tr bgcolor="#">
		<th><b>Elementos desconocidos</b></th>
    <th>La cantidad de conejos y la cantidad de gansos.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Condiciones</b></th>
    <th>La suma de los conejos y los gansos es igual a 50. La suma de las patas de los conejos y de los gansos es igual a 150.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Tipo de problema</b></th>
    <th>Solucionable - Algoritmico - Bien condicionado<br>
    <details><summary>Solución:</summary><p>Conejos: 20, Gansos:30</p></details></th>
	</tr>
</table>
</p></details><br>

4. ¿Existe, en la expansión decimal de π, una secuencia de tamaño n para
un número natural n dado?

<details><summary>Solución</summary><p>
<table cellspacing="3" bgcolor="">
	<tr bgcolor="#">
		<th><b>Elementos conocidos</b></th>
    <th>El número n.</th>
	</tr>
	<tr bgcolor="#">
		<th><b>Elementos desconocidos</b></th>
    <th>Un valor de verdad (falso o verdadero).</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Condiciones</b></th>
    <th>Verdadero si existe en la expansión decimal de π una secuencia de tamaño n del número n, para todo número natural n, Falso en otro caso.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Tipo de problema</b></th>
    <th>Indecidible.<br>
     Este problema es indecidible por que si en el primer millón de dígitos de π no se encuentra una secuencia como la buscada, nada garantiza que en el siguiente millón de dígitos no se encuentre tal secuencia. Pero si no se encuentra en el segundo millón, nada garantiza que no se encuentre después, o no se encuentre. De esta manera no se puede decidir si existe o no existe tal secuencia.</th>
	</tr>
</table>
</p></details><br>

5. Realizar la suma de dos números naturales.

<details><summary>Solución</summary><p>
<table cellspacing="3" bgcolor="">
	<tr bgcolor="#">
		<th><b>Elementos conocidos</b></th>
    <th>Dos números naturales.</th>
	</tr>
	<tr bgcolor="#">
		<th><b>Elementos desconocidos</b></th>
    <th>Un número natural.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Condiciones</b></th>
    <th>El número desconocido debe ser igual a la suma de los dos números dados.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Tipo de problema</b></th>
    <th>Solucionable - Algoritmico.<br>
    <details><summary>Solución:</summary><p>Qué dijeron...navidad?</p></details></th> </th>
	</tr>
</table>
</p></details><br>

6. Una partícula se mueve en el espacio de manera aleatoria, si en el instante de tiempo t se encuentra en la posición x, ¿cuál será la posición exacta de dicha partícula 10 segundos después?

<details><summary>Solución</summary><p>
<table cellspacing="3" bgcolor="">
	<tr bgcolor="#">
		<th><b>Elementos conocidos</b></th>
    <th>Posición en el instante de tiempo t, lapso de tiempo transcurrido (10 s).</th>
	</tr>
	<tr bgcolor="#">
		<th><b>Elementos desconocidos</b></th>
    <th>Una posición en el espacio.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Condiciones</b></th>
    <th>La partícula se mueve en el espacio de manera aleatoria.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Tipo de problema</b></th>
    <th>No solucionable - Indecidible.<br>
    No se puede solucionar por que no existe forma de predecir la posición de la partícula, pues su movimiento es aleatorio, es decir, se mueve de manera arbitraria.</th>
	</tr>
</table>
</p></details><br>

7. Un robot debe trasladar una pila (montón) de cajas desde un punto A hasta un punto C usando, si lo requiere, un punto intermedio B. Las cajas inicialmente están todas en el punto A, ordenadas como muestra la siguiente figura. En cada traslado, el robot sólo puede tomar una caja que esté en la cima de un montón y llevarla a uno de los otros dos puntos. Además, en ningún momento puede poner una caja sobre otra más pequeña. Mirando la figura, ¿cómo puede el robot pasar las tres cajas apiladas en el lugar A, al lugar C.? (Torre de Hanoi).

<div align='center'>
<figure> <img src="https://i.postimg.cc/T3rgnxqC/image.png" alt="" width="650" height="auto"/></br>
<figcaption><b></b></figcaption></figure>
</div>

<details><summary>Solución</summary><p>
<table cellspacing="3" bgcolor="">
	<tr bgcolor="#">
		<th><b>Elementos conocidos</b></th>
    <th>Número de cajas, posición inicial y posición destino, número de lugares de
apilamiento.</th>
	</tr>
	<tr bgcolor="#">
		<th><b>Elementos desconocidos</b></th>
    <th>Una secuencia de traslados.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Condiciones</b></th>
    <th>La secuencia de traslados solicitada debe respetar las reglas enunciadas: no se puede poner una caja sobre otra más pequeña, solo se puede tomar una caja a la vez y solo la que este más arriba en una pila de cajas.</th>
	</tr>
  <tr bgcolor="#">
		<th><b>Tipo de problema</b></th>
    <th>Solucionable - Algoritmico.<br>
    Lápiz y papel para escribir los pasos de la solución.</th>
	</tr>
</table>
</p></details><br>

----------------------
## Algoritmos