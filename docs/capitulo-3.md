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

<table>
  <tr>
    <th>Epic-03</th>
    <th>Proceso de suscripción</th>
  </tr>

  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      <br></br>
      Como usuario quiero completar el proceso de suscripción para acceder a las funcionalidades de la plataforma según el plan elegido.
    </td>
  </tr>

  <tr>
    <td align="center">14</td>
    <td align="center">Seleccionar plan de suscripción</td>
  </tr>
  <tr>
    <td align="center">15</td>
    <td align="center">Iniciar proceso de suscripción</td>
  </tr>
  <tr>
    <td align="center">16</td>
    <td align="center">Registrar datos de facturación</td>
  </tr>
  <tr>
    <td align="center">17</td>
    <td align="center">Procesar cobro de suscripción</td>
  </tr>
  <tr>
    <td align="center">18</td>
    <td align="center">Activar suscripción</td>
  </tr>
</table>
<br> </br>

<table>
  <tr>
    <th>Epic-04</th>
    <th>Configuración de suscripción</th>
  </tr>

  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      <br></br>
      Como usuario quiero visualizar y gestionar la configuración de mi suscripción para consultar su estado, renovarla o cancelarla según mis necesidades.
    </td>
  </tr>

  <tr>
    <td align="center">19</td>
    <td align="center">Visualizar panel de suscripción</td>
  </tr>
  <tr>
    <td align="center">20</td>
    <td align="center">Consultar estado de suscripción</td>
  </tr>
  <tr>
    <td align="center">21</td>
    <td align="center">Renovar suscripción</td>
  </tr>
  <tr>
    <td align="center">22</td>
    <td align="center">Solicitar cancelación de suscripción</td>
  </tr>
  <tr>
    <td align="center">23</td>
    <td align="center">Cancelar suscripción</td>
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

<br><br>

<table>
<tr>
<th>User Story</th>
<th>14</th>
<th>Epic ID</th>
<th>03</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Seleccionar plan de suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero seleccionar un plan de suscripción para definir el tipo de acceso y beneficios que tendré dentro de la plataforma.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Selección de plan realizada correctamente</strong><br>
Dado que el usuario visualiza los planes de suscripción disponibles<br>
Cuando selecciona uno de los planes mostrados<br>
Entonces el sistema registrará el plan seleccionado<br>
Y permitirá continuar con el proceso de suscripción<br><br>

<strong>Scenario 2: Intento de continuar sin seleccionar un plan</strong><br>
Dado que el usuario visualiza los planes de suscripción disponibles<br>
Y no selecciona ningún plan<br>
Cuando intenta continuar con el proceso<br>
Entonces el sistema no permitirá avanzar<br>
Y mostrará un mensaje indicando que debe seleccionar un plan<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>15</th>
<th>Epic ID</th>
<th>03</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Iniciar proceso de suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero iniciar el proceso de suscripción para comenzar formalmente la contratación del plan previamente elegido.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Proceso de suscripción iniciado correctamente</strong><br>
Dado que el usuario ya seleccionó un plan de suscripción<br>
Cuando presiona la opción para iniciar la suscripción<br>
Entonces el sistema registrará el inicio del proceso de suscripción<br>
Y habilitará el formulario de facturación<br><br>

<strong>Scenario 2: Intento de iniciar suscripción sin plan seleccionado</strong><br>
Dado que el usuario no ha seleccionado un plan de suscripción<br>
Cuando intenta iniciar el proceso de suscripción<br>
Entonces el sistema no permitirá iniciar el proceso<br>
Y mostrará un mensaje solicitando seleccionar un plan primero<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>16</th>
<th>Epic ID</th>
<th>03</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Registrar datos de facturación</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero ingresar mis datos de facturación para que el sistema pueda procesar el cobro correspondiente a la suscripción.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Datos de facturación registrados correctamente</strong><br>
Dado que el usuario se encuentra en el proceso de suscripción<br>
Y completa correctamente los datos de facturación<br>
Cuando confirma el formulario<br>
Entonces el sistema registrará los datos ingresados<br>
Y permitirá continuar al paso de cobro<br><br>

<strong>Scenario 2: Datos de facturación inválidos</strong><br>
Dado que el usuario se encuentra en el proceso de suscripción<br>
Y completa incorrectamente los datos de facturación<br>
Cuando intenta confirmar el formulario<br>
Entonces el sistema no registrará los datos<br>
Y mostrará un mensaje indicando que existen datos inválidos<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>17</th>
<th>Epic ID</th>
<th>03</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Procesar cobro de suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero que el sistema procese el cobro de la suscripción para validar el pago del plan seleccionado.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Cobro procesado exitosamente</strong><br>
Dado que el usuario ha registrado correctamente sus datos de facturación<br>
Cuando el sistema procesa el cobro de la suscripción<br>
Entonces el cobro será procesado exitosamente<br>
Y el sistema permitirá activar la suscripción<br><br>

<strong>Scenario 2: Error durante el procesamiento del cobro</strong><br>
Dado que el usuario ha iniciado el proceso de pago<br>
Cuando ocurre un error como tarjeta rechazada, datos inválidos o cobro fallido<br>
Entonces el sistema no activará la suscripción<br>
Y mostrará un mensaje indicando el motivo del error<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>18</th>
<th>Epic ID</th>
<th>03</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Activar suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero que mi suscripción sea activada una vez confirmado el cobro para acceder a las funcionalidades de la plataforma según el plan contratado.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Activación de suscripción exitosa</strong><br>
Dado que el cobro de la suscripción fue procesado correctamente<br>
Cuando el sistema confirma el pago<br>
Entonces la suscripción será activada<br>
Y el usuario obtendrá acceso a las funcionalidades correspondientes<br><br>

<strong>Scenario 2: Suscripción no activada por pago no confirmado</strong><br>
Dado que el cobro de la suscripción no fue confirmado<br>
Cuando el sistema intenta activar la suscripción<br>
Entonces la suscripción permanecerá en estado pendiente<br>
Y el usuario no podrá acceder a las funcionalidades premium<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>19</th>
<th>Epic ID</th>
<th>04</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Visualizar panel de suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero visualizar el panel de suscripción para consultar de forma clara la información general relacionada con mi plan actual.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Panel de suscripción mostrado correctamente</strong><br>
Dado que el usuario accede a la sección de suscripción<br>
Cuando el sistema carga la vista correspondiente<br>
Entonces se mostrará el panel de suscripción<br>
Y se visualizarán los datos generales de la suscripción del usuario<br><br>

<strong>Scenario 2: Usuario sin suscripción registrada</strong><br>
Dado que el usuario accede a la sección de suscripción<br>
Y no tiene una suscripción activa o registrada<br>
Cuando el sistema carga la vista correspondiente<br>
Entonces se mostrará el panel sin información activa<br>
Y se indicará que no existe una suscripción disponible<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>20</th>
<th>Epic ID</th>
<th>04</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Consultar estado de suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero consultar el estado de mi suscripción para saber si se encuentra activa, vencida o cancelada.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Estado de suscripción activa mostrado correctamente</strong><br>
Dado que el usuario tiene una suscripción vigente<br>
Cuando consulta el estado de su suscripción<br>
Entonces el sistema mostrará que la suscripción se encuentra activa<br><br>

<strong>Scenario 2: Estado de suscripción vencida o cancelada mostrado correctamente</strong><br>
Dado que el usuario tiene una suscripción vencida o cancelada<br>
Cuando consulta el estado de su suscripción<br>
Entonces el sistema mostrará el estado correspondiente<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>21</th>
<th>Epic ID</th>
<th>04</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Renovar suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero renovar mi suscripción para extender la vigencia de mi acceso a la plataforma.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Renovación realizada correctamente</strong><br>
Dado que el usuario tiene una suscripción activa o próxima a vencer<br>
Cuando selecciona la opción de renovar suscripción<br>
Entonces el sistema registrará la renovación<br>
Y actualizará la nueva fecha de vencimiento<br><br>

<strong>Scenario 2: Renovación no permitida</strong><br>
Dado que el usuario no cuenta con una suscripción válida para renovación<br>
Cuando intenta renovar su suscripción<br>
Entonces el sistema no permitirá la acción<br>
Y mostrará un mensaje indicando que la renovación no puede realizarse<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>22</th>
<th>Epic ID</th>
<th>04</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Solicitar cancelación de suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero solicitar la cancelación de mi suscripción para detener su continuidad al finalizar el periodo vigente.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Solicitud de cancelación registrada correctamente</strong><br>
Dado que el usuario tiene una suscripción activa<br>
Cuando solicita la cancelación de su suscripción<br>
Entonces el sistema registrará la solicitud de cancelación<br>
Y mantendrá el acceso hasta la fecha de vencimiento<br><br>

<strong>Scenario 2: Usuario cancela la operación antes de confirmar</strong><br>
Dado que el usuario inició el proceso de cancelación<br>
Cuando decide no confirmar la solicitud<br>
Entonces el sistema no registrará la cancelación<br>
Y la suscripción continuará sin cambios<br><br>

</td>
</tr>
</table>

<br><br>

<table>
<tr>
<th>User Story</th>
<th>23</th>
<th>Epic ID</th>
<th>04</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Cancelar suscripción</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como sistema quiero cancelar la suscripción al finalizar su periodo vigente para retirar el acceso del usuario a las funcionalidades premium.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Cancelación ejecutada correctamente</strong><br>
Dado que existe una solicitud de cancelación registrada<br>
Y la fecha de vencimiento ha sido alcanzada<br>
Cuando el sistema procesa el fin del periodo<br>
Entonces la suscripción será cancelada<br>
Y el acceso a funcionalidades premium será retirado<br><br>

<strong>Scenario 2: Suscripción aún dentro del periodo vigente</strong><br>
Dado que existe una solicitud de cancelación registrada<br>
Pero la fecha de vencimiento aún no ha llegado<br>
Cuando el sistema verifica el estado de la suscripción<br>
Entonces la suscripción continuará activa<br>
Y el acceso permanecerá habilitado hasta el final del periodo<br><br>

</td>
</tr>
</table>

<br><br>

## 3.2. Impact Mapping

_Contenido por agregar._

## 3.3. Product Backlog

_Contenido por agregar._
