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

+ **No solucionable** != **no tratable**: Los problemas intratables son solucionables cuando el tama~no de la entrada es peque~no, pero resultan no solucionables para entradas medianas y/o grandes.

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



