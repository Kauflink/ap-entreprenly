# Capítulo III: Requirements Specification

## 3.1. User Stories

<!-- Epics-->
<table>
  <tr>
    <th>Epic-01</th>
    <th>Gestión de Inventario</th>
  </tr>

  <tr>
    <td colspan="2" >
      <strong >Descripción:</strong>
       <br></br>
      Como usuario quiero gestionar mi inventario(lotes y productos) para visualizar los datos con mayor claridad.
    </td>
  </tr>

  <tr>
    <td align="center">1</td>
    <td align="center">Agregación de Productos</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">Edición de lotes</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">Agregación de Lotes</td>
  </tr>
  <tr>
    <td align="center">4</td>
    <td align="center">Eliminación de Lotes</td>
  </tr>
  <tr>
    <td align="center">10</td>
    <td align="center">Visualización de detalles de Producto</td>
  </tr>
  <tr>
    <td align="center">5</td>
    <td align="center">Edición de Productos</td>
  </tr>
  <tr>
    <td align="center">6</td>
    <td align="center">Visualización de detalles de Lotes</td>
  </tr>
  <tr>
    <td align="center">13</td>
    <td align="center">Buscador de Productos</td>
  </tr>
</table>
<br> </br>

<table>
  <tr>
    <th>Epic-02</th>
    <th>
      Notificaciones de Inventario
    </th>
  </tr>

  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      <br></br>
      Como usuario quiero que el sistema me notifique el estado de mis lotes para organizarme mejor.
    </td>
  </tr>

  <tr>
    <td align="center">7</td>
    <td align="center">Detección de Stock Agotado</td>
  </tr>
  <tr>
    <td align="center">8</td>
    <td align="center">Mostrar alertas de estado al visualizar detalles</td>
  </tr>
  
  <tr>
    <td align="center">9</td>
    <td align="center">Dashboard de Lotes</td>
  </tr>

  <tr>
    <td align="center">11</td>
    <td align="center">Alerta de Producto sin Stock</td>
  </tr>
  <tr>
    <td align="center">12</td>
    <td align="center">Alerta de caducación de Lote</td>
  </tr>
</table>
<br> </br>

<!-- US-->
<table>
<tr>
<th>User Story</th>
<th>01</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Agregación de Productos</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero agregar productos para gestionar mi inventario de manera eficiente.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Agregar producto correctamente</strong><br>
Dado que el usuario está en el formulario de productos<br>
Cuando ingrese los datos correctamente<br>
Y presione el botón “Guardar”<br>
Entonces el producto se registrará exitosamente<br><br>

<strong>Scenario 2: Validación de datos</strong><br>
Dado que el usuario está en el formulario de productos<br>
Cuando deje campos obligatorios vacíos<br>
Y presione el botón “Guardar”<br>
Entonces el sistema mostrará mensajes de error
</td>
</tr>
</table>

<br></br>

<table>
<tr>
<th>User Story</th>
<th>02</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Edición de lotes</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero editar los lotes para actualizar los datos del inventario.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Editar lote correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y selecciona un lote existente<br>
Cuando modifique los datos correctamente<br>
Y presione el botón “Guardar”<br>
Entonces los cambios del lote se actualizarán exitosamente<br><br>

<strong>Scenario 2: Validación al editar lote</strong><br>
Dado que el usuario está editando un lote<br>
Cuando ingrese datos inválidos o deje campos obligatorios vacíos<br>
Y presione el botón “Guardar”<br>
Entonces el sistema mostrará mensajes de error y no guardará los cambios
</td>
</tr>
</table>

<br></br>

<table>
<tr>
<th>User Story</th>
<th>03</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Agregación de Lotes</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero agregar lotes para gestionar correctamente las cantidades, fechas de vencimiento
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Agregar lote correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y selecciona un lote existente<br>
Cuando ingrese una cantidad, fecha válida<br>
Y presione el botón “Agregar”<br>
Entonces el nuevo lote se agregará exitosamente.<br><br>

<strong>Scenario 2: Validación al agregar lote</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y selecciona un lote existente<br>
Cuando ingrese una cantidad, fecha válida<br>
Y presione el botón “Agregar”<br>
Entonces saldrá un mensaje de error por campo inválido
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>04</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Eliminación de Lotes</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero eliminar lotes para deshacerme de los lotes que no me sirvan
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Eliminar lote correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y selecciona un lote existente<br>
Cuando presione el botón “Eliminar”<br>
Entonces el lote se eliminará exitosamente<br><br>

<strong>Scenario 2: Validación al eliminar lote</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y selecciona un lote existente<br>
Cuando presione el botón “Eliminar”<br>
Entonces saldrá un mensaje de error de no haber seleccionado un lote
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>05</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Edición de Productos</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero editar productos para actualizar los datos en el inventario
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Producto editado correctamente</strong><br>
Dado que el usuario está en la sección de productos<br>
Y selecciona un producto existente<br>
Cuando presione el botón “Editar”<br>
Entonces el producto se actualizará exitosamente<br><br>

<strong>Scenario 2: Validación al editar productos</strong><br>
Dado que el usuario está en la sección de productos<br>
Y no selecciona un producto existente<br>
Cuando presione el botón “Editar”<br>
Entonces el sistema mostrará mensajes de error<br><br>
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>06</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Visualización de detalles de Lotes</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero visualizar los detalles de los lotes para poder gestionar mejor el inventario
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Detalles de lote mostrados correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y selecciona un lote existente<br>
Cuando presione el botón “Ver Detalles”<br>
Entonces los detalles se mostraran exitosamente<br><br>

<strong>Scenario 2: Validación al visualizar detalles de lote</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y no selecciona un lote existente<br>
Cuando presione el botón “Ver Detalles”<br>
Entonces los detalles saldrá un mensaje de error<br><br>
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>07</th>
<th>Epic ID</th>
<th>02</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Detección de Stock Agotado</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero ser notificado cuando tengo bajo/nada de stock
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Alerta de stock próximo a agotarse mostrada correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y uno o más lotes tienen stock por debajo del umbral definido<br>
Cuando el usuario accede al dashboard de lotes<br>
Entonces se debe mostrar una alerta visible indicando los lotes próximos a agotarse<br><br>

<strong>Scenario 2: Alerta de stock agotado mostrada correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y uno o más de sus lotes estan agotados<br>
Cuando el usuario accede al dashboard de lotes<br>
Entonces se debe mostrar una alerta indicando los lotes agotados<br><br>
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>08</th>
<th>Epic ID</th>
<th>02</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Mostrar alertas de estado al visualizar detalles</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero visualizar alertas de estado al ver el detalle de un lote para identificar rápidamente si tiene stock bajo, está agotado o próximo a vencer.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Alerta de stock próximo a agotarse mostrada correctamente</strong><br>
Dado que el usuario selecciona un lote<br>
Y el lote no tiene stock bajo, está agotado o próximo a vencer.<br>
Cuando presiona "Ver Detalles"<br>
Entonces se mostrarán los detalles del lote con alertas de estado<br><br>

<strong>Scenario 2: No mostrar alertas si el estado es normal</strong><br>
Dado que el usuario selecciona un lote<br>
Y el lote tiene stock bajo, está agotado o próximo a vencer.<br>
Cuando presiona "Ver Detalles"<br>
Entonces se mostrarán los detalles del lote sin alertas<br><br>
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>09</th>
<th>Epic ID</th>
<th>02</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Dashboard de Lotes</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero visualizar un dashboard de lotes con indicadores y alertas para conocer rápidamente el estado de mi inventario al ingresar al módulo de lotes.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Visualización de resumen de lotes</strong><br>
Dado que el usuario ingresa al módulo de lotes<br>
Cuando se carga la pantalla<br>
Entonces se debe mostrar un resumen con indicadores clave sobre los estados de los lotes<br>

<strong>Scenario 2: No mostrar alertas si no existen condiciones críticas</strong><br>
Dado que el usuario ingresa al módulo de lotes<br>
Y no existen lotes vencidos ni próximos a vencer<br>
Cuando se carga el dashboard<br>
Entonces no se debe mostrar el banner de alertas<br><br>
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>10</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Visualización de detalles de Producto</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero visualizar la información detallada de cada producto en el listado para conocer rápidamente sus características, stock disponible y precio sin necesidad de ingresar a otra pantalla.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Visualización de información del producto</strong><br>
Dado que el usuario accede al listado de productos<br>
Cuando se carga la información<br>
Entonces cada producto debe mostrar sus datos principales<br>
Y debe incluir: tipo, nombre, descripción,codigo QR, stock total y precio<br><br>

<strong>Scenario 2: Manejo de información incompleta del producto</strong><br>
Dado que el usuario accede al listado de productos<br>
Y un producto no cuenta con algún dato (descripción o código QR)<br>
Cuando se carga la información<br>
Entonces el sistema debe mostrar los demás datos disponibles correctamente<br>
Y los campos faltantes deben mostrarse como vacíos("-")<br><br>
</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>11</th>
<th>Epic ID</th>
<th>02</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Alerta de Producto sin Stock</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero ser notificado cuando un producto no tiene stock disponible
para poder tomar acciones como reabastecerlo.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Alerta de producto sin stock mostrada correctamente en dashboard</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y uno o más productos tienen stock total igual a 0<br>
Cuando el usuario accede al dashboard de lotes<br>
Entonces se debe mostrar una alerta indicando los productos sin stock<br><br>

<strong>Scenario 2: Indicador visual de producto sin stock en listado</strong><br>
Dado que el usuario visualiza el listado de productos<br>
Y un producto tiene stock total igual a 0<br>
Cuando se muestra la información<br>
Entonces el producto debe mostrar un indicador visual de "Sin stock"<br>
Y el stock debe mostrarse como 0<br><br>
</td>
</tr>
</table>


<br><br>
<table>
<tr>
<th>User Story</th>
<th>12</th>
<th>Epic ID</th>
<th>02</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Alerta de caducación de Lote</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero ser notificado cuando un lote esté próximo a vencer o ya haya vencido
para poder tomar acciones como priorizar su uso o descartarlo.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Alerta de lote próximo a vencer mostrada correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y uno o más lotes tienen una fecha de caducidad dentro del rango próximo definido<br>
Cuando el usuario accede al dashboard de lotes<br>
Entonces se debe mostrar una alerta indicando los lotes próximos a vencer<br><br>

<strong>Scenario 2: Alerta de lote vencido mostrada correctamente</strong><br>
Dado que el usuario está en la sección de lotes<br>
Y uno o más lotes tienen una fecha de caducidad menor a la fecha actual<br>
Cuando el usuario accede al dashboard de lotes<br>
Entonces se debe mostrar una alerta indicando los lotes vencidos<br><br>

</td>
</tr>
</table>

<br><br>
<table>
<tr>
<th>User Story</th>
<th>13</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Buscador de Productos</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero tener un buscador de productos para perder menos tiempo buscando en el inventario.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Búsqueda de productos por nombre</strong><br>
Dado que el usuario está en el listado de productos<br>
Cuando ingresa el nombre de un producto en el campo de búsqueda<br>
Entonces el sistema debe filtrar y mostrar los productos que coincidan con el nombre ingresado<br><br>

<strong>Scenario 2: Búsqueda de productos por categoría</strong><br>
Dado que el usuario está en el listado de productos<br>
Cuando selecciona o ingresa una categoría en el buscador<br>
Entonces el sistema debe filtrar y mostrar los productos que pertenecen a esa categoría<br><br>

</td>
</tr>
</table>

## 3.2. Impact Mapping

*Contenido por agregar.*

## 3.3. Product Backlog

*Contenido por agregar.*