# Capítulo III: Requirements Specification

## 3.1. User Stories

<!-- Epics-->
<div align="center">
<table>
  <tr>
    <th>Epic-01</th>
    <th>Gestión de Inventario</th>
  </tr>

  <tr>
    <td colspan="2" >
      <strong >Descripción:</strong>
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
  <tr>
    <td align="center">23</td>
    <td align="center">Creación de lotes</td>
  </tr>
</table>
<br><br>
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
    <td align="center">Alerta de caducación de Lote</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-03</th>
    <th>Proceso de suscripción</th>
  </tr>

  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como usuario quiero completar el proceso de suscripción para acceder a las funcionalidades de la plataforma según el plan elegido.
    </td>
  </tr>

  <tr>
    <td align="center">13</td>
    <td align="center">Seleccionar plan de suscripción</td>
  </tr>
  <tr>
    <td align="center">14</td>
    <td align="center">Iniciar proceso de suscripción</td>
  </tr>
  <tr>
    <td align="center">15</td>
    <td align="center">Registrar datos de facturación</td>
  </tr>
  <tr>
    <td align="center">16</td>
    <td align="center">Procesar cobro de suscripción</td>
  </tr>
  <tr>
    <td align="center">17</td>
    <td align="center">Activar suscripción</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-04</th>
    <th>Configuración de suscripción</th>
  </tr>

  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como usuario quiero visualizar y gestionar la configuración de mi suscripción para consultar su estado, renovarla o cancelarla según mis necesidades.
    </td>
  </tr>

  <tr>
    <td align="center">18</td>
    <td align="center">Visualizar panel de suscripción</td>
  </tr>
  <tr>
    <td align="center">19</td>
    <td align="center">Consultar estado de suscripción</td>
  </tr>
  <tr>
    <td align="center">20</td>
    <td align="center">Renovar suscripción</td>
  </tr>
  <tr>
    <td align="center">21</td>
    <td align="center">Solicitar cancelación de suscripción</td>
  </tr>
  <tr>
    <td align="center">22</td>
    <td align="center">Cancelar suscripción</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-05</th>
    <th>Control de Ingresos y Arqueo de Caja</th>
  </tr>

  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como cajero o comerciante quiero contar con un módulo de ventas integrado con dispositivos IoT y persistencia en base de datos, para procesar transacciones de manera rápida, emitir comprobantes legales y mantener el inventario sincronizado automáticamente.
    </td>
  </tr>

  <tr>
    <td align="center">24</td>
    <td align="center">Selección y Registro de Ítems</td>
  </tr>
  <tr>
    <td align="center">25</td>
    <td align="center">Registro de Productos por Peso (IoT)</td>
  </tr>
  <tr>
    <td align="center">26</td>
    <td align="center">Gestión del Detalle del Ticket de Venta</td>
  </tr>
  <tr>
    <td align="center">27</td>
    <td align="center">Selección de Método de Pago</td>
  </tr>

  <tr>
    <td align="center">29</td>
    <td align="center">Finalización de Venta, Registro y Emisión de Comprobante</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-06</th>
    <th>Gestion de Ventas</th>
  </tr>

  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como comerciante, quiero que el sistema centralice y clasifique los ingresos según el medio de pago en tiempo real, para realizar el arqueo de caja al final del día de manera exacta y sin errores manuales.
    </td>
  </tr>

  <tr>
    <td align="center">28</td>
    <td align="center">Clasificación Automática de Ingresos por Medio de Pago</td>
  </tr>

  <tr>
    <td align="center">30</td>
    <td align="center">Consulta de Resumen de Caja Diario</td>
  </tr>
  
</table>
<br><br>
<table>
  <tr>
    <th>Epic-07</th>
    <th>Conversación y Catálogo</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como cliente potencial, quiero  una interacción fluida con el chatbot de WhatsApp y visualizar un catálogo de productos actualizado en tiempo real, para poder conocer la oferta disponible y comenzar mi proceso de compra de manera inmediata.
    </td>
  </tr>
  <tr>
    <td align="center">31</td>
    <td align="center">Iniciar conversación con chatbot</td>
  </tr>
  <tr>
    <td align="center">32</td>
    <td align="center">Recibir catálogo de productos</td>
  </tr>
  <tr>
    <td align="center">33</td>
    <td align="center">Catálogo sincronizado con inventario real</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-08</th>
    <th>Gestión de Pedido y Stock</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como cliente, quiero seleccionar productos, indicar cantidades y registrar mi ubicación de entrega, para que el sistema genere un pedido consolidado y verifique automáticamente la disponibilidad física antes de proceder al pago.
    </td>
  </tr>
  <tr>
    <td align="center">34</td>
    <td align="center">Seleccionar productos y cantidades</td>
  </tr>
  <tr>
    <td align="center">35</td>
    <td align="center">Registrar dirección de delivery</td>
  </tr>
  <tr>
    <td align="center">36</td>
    <td align="center">Generar pedido consolidado</td>
  </tr>
  <tr>
    <td align="center">37</td>
    <td align="center">Validar stock antes del pago</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-09</th>
    <th>Pago Digital P2P</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como cliente y comerciante, queremos gestionar el envío y la validación de comprobantes de pago digitales (Yape/Plin) a través de WhatsApp y el dashboard, para garantizar una transacción segura y confirmada antes de finalizar la venta.
    </td>
  </tr>
  <tr>
    <td align="center">38</td>
    <td align="center">Recibir instrucciones de pago</td>
  </tr>
  <tr>
    <td align="center">39</td>
    <td align="center">Reportar pago digital realizado</td>
  </tr>
  <tr>
    <td align="center">40</td>
    <td align="center">Validar pago desde el dashboard</td>
  </tr>
  <tr>
    <td align="center">41</td>
    <td align="center">Notificar estado del pago al cliente</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-10</th>
    <th>Confirmación, Venta y Comprobante</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como dueño de negocio, quiero que el sistema confirme el pedido tras la validación del pago, descuente el stock y emita un comprobante digital, para mantener el control financiero y brindar un respaldo legal de la compra al cliente.
    </td>
  </tr>
  <tr>
    <td align="center">42</td>
    <td align="center">Confirmar pedido y descontar stock</td>
  </tr>
  <tr>
    <td align="center">43</td>
    <td align="center">Registrar venta en el sistema</td>
  </tr>
  <tr>
    <td align="center">44</td>
    <td align="center">Emitir comprobante al cliente</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-11</th>
    <th>Flujos Alternativos y Restricciones</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como sistema de gestión, quiero manejar escenarios de excepción como falta de stock, tiempos de espera agotados y rechazos de pago, para proteger la integridad del inventario y evitar pérdidas económicas.
    </td>
  </tr>
  <tr>
    <td align="center">45</td>
    <td align="center">Manejar stock insuficiente</td>
  </tr>
  <tr>
    <td align="center">46</td>
    <td align="center">Cancelar pedido por timeout de pago</td>
  </tr>
  <tr>
    <td align="center">47</td>
    <td align="center">Rechazar pago fraudulento o incorrecto</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-12</th>
    <th>Technical Stories – RESTful API</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como equipo de desarrollo, queremos implementar una arquitectura de servicios RESTful segura y escalable, para que todos los componentes de la plataforma (chatbot, dashboard, inventario) intercambien datos de manera consistente.
    </td>
  </tr>
  <tr>
    <td align="center">48</td>
    <td align="center">API: obtener catálogo de productos</td>
  </tr>
  <tr>
    <td align="center">49</td>
    <td align="center">API: crear y actualizar pedido</td>
  </tr>
  <tr>
    <td align="center">50</td>
    <td align="center">API: validar y registrar pago</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-13</th>
    <th>Inicio de Sesión y Registro</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como usuario quiero poder registrarme, verificar mi cuenta, iniciar sesión y recuperar mi contraseña para acceder de forma segura a la plataforma.
    </td>
  </tr>
  <tr>
    <td align="center">51</td>
    <td align="center">Registro de cuenta con email</td>
  </tr>
  <tr>
    <td align="center">52</td>
    <td align="center">Verificación de email</td>
  </tr>
  <tr>
    <td align="center">53</td>
    <td align="center">Inicio de sesión con credenciales</td>
  </tr>
  <tr>
    <td align="center">54</td>
    <td align="center">Inicio de sesión con Google OAuth</td>
  </tr>
  <tr>
    <td align="center">55</td>
    <td align="center">Recuperación de contraseña</td>
  </tr>
  <tr>
    <td align="center">56</td>
    <td align="center">Cierre de sesión</td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>Epic-14</th>
    <th>Perfil y Configuración</th>
  </tr>
  <tr>
    <td colspan="2">
      <strong>Descripción:</strong>
      Como usuario quiero gestionar mi perfil y preferencias personales para personalizar mi experiencia dentro de la plataforma.
    </td>
  </tr>
  <tr>
    <td align="center">57</td>
    <td align="center">Visualizar perfil actual</td>
  </tr>
  <tr>
    <td align="center">58</td>
    <td align="center">Actualizar nombre y biografía</td>
  </tr>
  <tr>
    <td align="center">59</td>
    <td align="center">Subir foto de perfil</td>
  </tr>
  <tr>
    <td align="center">60</td>
    <td align="center">Cambiar email con re-verificación</td>
  </tr>
  <tr>
    <td align="center">61</td>
    <td align="center">Cambiar contraseña</td>
  </tr>
  <tr>
    <td align="center">62</td>
    <td align="center">Configurar preferencias de idioma, zona horaria y tema</td>
  </tr>
  <tr>
    <td align="center">63</td>
    <td align="center">Configurar notificaciones</td>
  </tr>
</table>

<!-- US-->
<br><br>
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
<br><br>
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
<br><br>
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
<th>12</th>
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
<th>13</th>
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
<th>14</th>
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
<th>15</th>
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
<th>16</th>
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
<th>17</th>
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
<th>18</th>
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
<th>19</th>
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
<th>20</th>
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
<th>21</th>
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
<th>22</th>
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
<table>
<tr>
<th>User Story</th>
<th>23</th>
<th>Epic ID</th>
<th>01</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Creación de lotes</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
Como usuario quiero crear lotes de productos para controlar mejor el stock y la caducidad en el inventario.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Creación de lote exitosa</strong><br>
Dado que el usuario está en la sección de productos<br>
Cuando presiona el botón “Crear Lote”<br>
Y selecciona un producto existente<br>
Y completa los datos requeridos correctamente<br>
Entonces el sistema debe registrar el nuevo lote<br>
Y mostrarlo en la lista de lotes<br><br>

<strong>Scenario 2: Validación al crear lote</strong><br>
Dado que el usuario está en la sección de productos<br>
Cuando presiona el botón “Crear Lote”<br>
Y no selecciona un producto o ingresa datos incompletos o inválidos<br>
Entonces el sistema debe mostrar mensajes de error<br>
Y no permitir la creación del lote<br><br>

</td>
</tr>
</table>
<br><br>
<table>
<tr>
<th>User Story</th>
<th>24</th>
<th>Epic ID</th>
<th>06</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Selección y Registro de Ítems</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
<strong>Como</strong> cajero, <strong>quiero</strong> buscar y seleccionar productos del inventario, <strong>para</strong> agregarlos al detalle del Ticket de Venta.
</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Selección de producto existente</strong><br>
<strong>Dado</strong> que el cajero se encuentra en la interfaz de ventas,<br>
<strong>Cuando</strong> ingresa el  nombre del producto en el buscador,<br>
<strong>Y</strong> haya ingresado la cantidad <br>
<strong>Y</strong> presiona la tecla enter para confirmar,<br>
<strong>Entonces</strong> el sistema añade el producto con su información base al detalle de la venta.<br><br>

<strong>Scenario 2: Intento de agregar producto no registrado</strong><br>
<strong>Dado</strong> que el cajero se encuentra en la interfaz de ventas,<br>
<strong>Cuando</strong> ingresa un nombre de un producto que no existe en la base de datos,<br>
<strong>Y</strong> el sistema termina de realizar la búsqueda sin coincidencias,<br>
<strong>Entonces</strong> el sistema muestra un mensaje de error indicando "Producto no encontrado".<br><br>

</td>
</tr>
</table>
<br><br>
<table>
<tr>
<th>User Story</th>
<th>25</th>
<th>Epic ID</th>
<th>06</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Registro de Productos por Peso (IoT)</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
<strong>Como</strong> cajero, <strong>quiero</strong> registrar el peso de los productos en el sistema (ya sea por captura automática o ingreso manual), <strong>para</strong> agilizar el proceso de cobro y asegurar que la venta no se detenga por fallas técnicas

</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Captura automática mediante balanza conectada (Ruta Principal)</strong><br>
<strong>Dado</strong> que el sistema cuenta con una balanza IoT configurada y conectada,<br>
<strong>Cuando</strong> se selecciona un producto que se vende por peso,<br>
<strong>Y</strong> el sistema recibe la lectura del peso directamente del hardware, <br>
<strong>Entonces</strong> el sistema carga el valor automáticamente en el detalle de la venta<br><br>

<strong>Scenario 2: Registro manual en ausencia o falla de balanza (Ruta Alternativa)</strong><br>
<strong>Dado</strong> que el establecimiento no cuenta con balanza IoT o el dispositivo está desconectado,<br>
<strong>Cuando</strong> el cajero selecciona un producto que se vende por peso,<br>
<strong>Y</strong> el sistema detecta que no hay respuesta del hardware elige la opción "Ingreso Manual",<br>
<strong>Entonces</strong> el sistema habilita un teclado numérico para que el cajero digite el peso observado físicamente.
<br><br>

</td>
</tr>
</table>
<br><br>
<table>
<tr>
<th>User Story</th>
<th>26</th>
<th>Epic ID</th>
<th>06</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Gestión del Detalle del Ticket de Venta</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
<strong>Como</strong> cajero, <strong>quiero</strong> visualizar el desglose de productos (nombre, cantidad, precio unitario y subtotal), <strong>para</strong> verificar que la información de la venta sea correcta antes del pago.

</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Actualización del detalle y monto total</strong><br>
<strong>Dado</strong> que se han añadido productos al ticket de venta,<br>
<strong>Cuando</strong> el sistema procesa cada ítem de la lista,<br>
<strong>Y</strong> multiplica el precio unitario por la cantidad o peso ingresado, <br>
<strong>Entonces</strong> el sistema muestra el subtotal por producto y el monto total acumulado de la venta.

</td>
</tr>
</table>
<br><br>
<table>
<tr>
<th>User Story</th>
<th>27</th>
<th>Epic ID</th>
<th>06</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Selección de Método de Pago</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
<strong>Como</strong> cajero, <strong>quiero</strong> elegir cómo está pagando el cliente (Efectivo, Tarjeta/Yape/Plin), <strong>para</strong> que el monto de la venta se registre en la categoría correcta de ingresos.

</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Selección de método de pago exitosa</strong><br>
<strong>Dado</strong> que el ticket de venta tiene el monto total calculado,
<strong>Cuando</strong> el cajero hace clic sobre el ícono de "Efectivo", "Tarjeta/Yape/Plin",
<strong>Y</strong> el sistema marca la opción seleccionada como activa,
<strong>Entonces</strong> el sistema habilita el botón para emitir la boleta y finalizar la venta.

<strong>Scenario 1: Omisión del método de pago</strong><br>
<strong>Dado</strong> que el cajero terminó de enlistar los productos,
<strong>Cuando</strong> intenta finalizar la venta sin haber seleccionado ninguna opción de pago,
<strong>Y</strong> el sistema detecta que no hay un método asignado para esta transacción,
<strong>Entonces</strong> el sistema muestra un mensaje indicando "Por favor, seleccione un método de pago" y no permite generar la boleta.

<br><br>

</td>
</tr>
</table>
<br><br>
<table>
<tr>
<th>User Story</th>
<th>28</th>
<th>Epic ID</th>
<th>07</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Clasificación Automática de Ingresos por Medio de Pago</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
<strong>Como</strong> comerciante, <strong>quiero</strong> que cada venta finalizada sume su monto al acumulado del método de pago correspondiente, <strong>para</strong> tener visibilidad inmediata de cuánto dinero hay en efectivo y cuánto en digital (Yape/Plin/Tarjeta).

</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Actualización de acumulados tras venta
</strong><br>
<strong>Dado</strong> que el sistema ha registrado una venta exitosamente,
<strong>Cuando</strong> el proceso de guardado en PostgreSQL detecta el medio de pago utilizado (ej. Yape),
<strong>Y</strong> localiza la cuenta acumulativa de dicho método en el sistema,
<strong>Entonces</strong> el sistema suma el monto de la venta al total acumulado de ese medio de pago de forma inmediata.

</td>
</tr>
</table>
<br><br>
<table>
<tr>
<th>User Story</th>
<th>29</th>
<th>Epic ID</th>
<th>06</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Finalización de Venta, Registro y Emisión de Comprobante

</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
<strong>Como</strong> cajero, <strong>quiero</strong> procesar el pago y finalizar la venta con un solo paso, <strong>para</strong> registrar la transacción en el sistema y entregarle su boleta al cliente de forma inmediata.

</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Procesamiento de cierre de venta (Ruta Feliz)
</strong><br>
<strong>Dado</strong> que el detalle del ticket de venta está completo y el método de pago ha sido seleccionado,<br>
<strong>Cuando</strong> el cajero presiona el botón "Finalizar Venta y Emitir Boleta",<br>
<strong>Y</strong> registra la información en PostgreSQL actualizando los saldos y el stock,<br>
<strong>Entonces</strong> el sistema genera el comprobante de pago final y limpia la pantalla para una nueva venta.<br>

<strong>Scenario 2: Procesamiento de cierre de venta (Ruta Feliz)
</strong><br>
<strong>Dado</strong> que el total de la venta ha sido calculado y revisado,<br>
<strong>Cuando</strong> el cajero selecciona el medio de pago (Efectivo, Tarjeta o Digital),<br>
<strong>Y</strong> confirma que el monto recibido es correcto,<br>
<strong>Entonces</strong> el sistema habilita la opción para procesar el cierre de la transacción.<br>

</td>
</tr>
</table>
<br><br>
<table>
<tr>
<th>User Story</th>
<th>30</th>
<th>Epic ID</th>
<th>07</th>
</tr>
<tr>
<td><strong>Title</strong></td>
<td colspan="3">Consulta de Resumen de Caja Diario

</td>
</tr>
<tr>
<td><strong>Description</strong></td>
<td colspan="3">
<strong>Como</strong> cajero, <strong>quiero</strong> procesar el pago y finalizar la venta con un solo paso, <strong>para</strong> registrar la transacción en el sistema y entregarle su boleta al cliente de forma inmediata.

</td>
</tr>
<tr>
<td><strong>Acceptance Criteria</strong></td>
<td colspan="3">

<strong>Scenario 1: Visualización detallada de ingresos
</strong><br>
<strong>Dado</strong> que el comerciante accede a la sección de "Cierre de Caja" o "Reportes",
<strong>Cuando</strong> el sistema consulta los saldos acumulados en la base de datos,
<strong>Y</strong> desglosa los totales por: Efectivo, Tarjeta y Yape/Plin,
<strong>Entonces</strong> el sistema muestra el monto total general y la suma independiente de cada categoría para el arqueo final.

</td>
</tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>31</th>
    <th>Epic ID</th>
    <th>07</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Iniciar conversación con chatbot</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero iniciar una conversación con el chatbot de WhatsApp para poder realizar un pedido sin necesidad de llamar ni ir a la tienda.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Respuesta inmediata al primer mensaje</strong><br>
      Dado que el cliente envía cualquier mensaje al número de WhatsApp registrado,<br>
      Cuando el chatbot recibe el mensaje,<br> 
      Entonces responde en menos de 3 segundos con mensaje de bienvenida con el nombre del negocio y las opciones disponibles <br><br>
      <strong>Scenario 2: Retomar conversación activa</strong><br>
      Dado que el cliente ya tiene una conversación activa sin completar,<br>
      Cuando envía un nuevo mensaje,<br>
      Entonces el chatbot retoma el contexto del pedido en curso sin reiniciar el flujo.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>32</th>
    <th>Epic ID</th>
    <th>07</th>
  </tr>
  <br><br>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Recibir catálogo de productos</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero recibir el catálogo actualizado de productos directamente en WhatsApp para elegir lo que deseo comprar.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Catálogo enviado con productos disponibles</strong><br>
      Dado que el cliente solicita ver el catálogo,<br>
      Cuando el chatbot consulta el inventario,<br>
      Entonces envía la lista con nombre, precio y stock, mostrando únicamente productos con stock mayor a 0.<br><br>
      <strong>Scenario 2: Sin productos disponibles en inventario</strong><br>
      Dado que no hay productos con stock disponible,<br>
      Cuando el chatbot consulta el inventario,<br>
      Entonces informa al cliente que no hay productos disponibles en este momento.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>33</th>
    <th>Epic ID</th>
    <th>07</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Catálogo sincronizado con inventario real</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como comerciante, quiero que el catálogo del chatbot refleje siempre el inventario real para evitar vender productos sin existencia.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Precio actualizado reflejado en el siguiente catálogo</strong><br>
      Dado que el comerciante actualiza el precio de un producto en el dashboard,<br>
      Cuando un cliente solicita el catálogo,<br>
      Entonces el chatbot muestra el precio actualizado.<br><br>
      <strong>Scenario 2: Producto agotado no aparece en el catálogo</strong><br>
      Dado que un producto agota su stock,<br>
      Cuando el sistema actualiza el inventario,<br>
      Entonces ese producto deja de mostrarse en el catálogo.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>34</th>
    <th>Epic ID</th>
    <th>08</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Seleccionar productos y cantidades</td>
  </tr>
  
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero seleccionar uno o más productos e indicar la cantidad para que el sistema construya mi pedido correctamente.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Selección exitosa de producto unitario</strong><br>
      Dado que el cliente recibe el catálogo,<br>
      Cuando indica un producto y cantidad válida,<br>
      Entonces el chatbot confirma la selección y la agrega al pedido en curso.<br><br>
      <strong>Scenario 2: Selección de producto por peso</strong><br>
      Dado que el cliente indica un producto por peso (ej: 1.5 kg de arroz),<br>
      Cuando el chatbot procesa la solicitud,<br>
      Entonces registra la cantidad en kilogramos y calcula el subtotal.<br><br><strong>Scenario 3: Producto no encontrado en el catálogo</strong><br>
      Dado que el cliente escribe un producto inexistente,<br>
      Cuando el chatbot no lo encuentra,<br>
      Entonces informa que no está disponible y muestra el catálogo nuevamente.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>35</th>
    <th>Epic ID</th>
    <th>08</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Registrar dirección de delivery</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero ingresar mi dirección de entrega para que el comerciante sepa dónde enviar mi pedido.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Registro exitoso de dirección de entrega</strong><br>
      Dado que el cliente confirmó al menos un producto,<br>
      Cuando el chatbot solicita la dirección y el cliente la ingresa,<br>
      Entonces el sistema registra la dirección asociada al pedido y continúa el flujo.<br><br>
      <strong>Scenario 2: Cliente no responde con dirección</strong><br>
      Dado que el chatbot solicitó la dirección de entrega,<br>
      Cuando el cliente no ingresa dirección en 10 minutos,<br>
      Entonces el chatbot solicita nuevamente la dirección antes de continuar.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>36</th>
    <th>Epic ID</th>
    <th>08</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Generar pedido consolidado</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como sistema, quiero generar un pedido con todos los productos, cantidades, dirección y datos del cliente para poder procesarlo.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Pedido creado exitosamente</strong><br>
      Dado que el cliente confirma productos y dirección,<br>
      Cuando el sistema genera el pedido,<br>
      Entonces crea un registro con estado 'pendiente', productos, cantidades, dirección y timestamp.<br><br>
      <strong>Scenario 2: Validación de stock iniciada tras generación</strong><br>
      Dado que el pedido ha sido generado,<br>
      Cuando el sistema procede a la validación,<br>
      Entonces verifica que cada producto tenga suficiente existencia antes de continuar al pago.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>User Story</th>
    <th>37</th>
    <th>Epic ID</th>
    <th>08</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Validar stock antes del pago</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como sistema, quiero validar el stock de cada producto del pedido para evitar comprometer inventario inexistente.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Stock suficiente para todos los ítems</strong><br>
      Dado que se genera un pedido,<br>
      Cuando el sistema verifica el stock,<br>
      Entonces confirma que hay cantidad suficiente para cada ítem y avanza al flujo de pago.<br><br>
      <strong>Scenario 2: Stock insuficiente para un ítem del pedido</strong><br>
      Dado que un producto del pedido no tiene stock suficiente,<br>
      Cuando el sistema detecta la insuficiencia,<br>
      Entonces notifica al cliente indicando qué producto no está disponible y ofrece continuar con menor cantidad o eliminar el ítem.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>38</th>
    <th>Epic ID</th>
    <th>09</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Recibir instrucciones de pago</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero recibir las instrucciones de pago por WhatsApp para saber cómo realizar la transferencia.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Instrucciones de pago enviadas correctamente</strong><br>
      Dado que el stock del pedido fue validado exitosamente,<br>
      Cuando el chatbot envía las instrucciones,<br>
      Entonces el cliente recibe el número Yape/Plin del comerciante, el monto total y el número de pedido como referencia.<br><br>
      <strong>Scenario 2: Registro del evento de instrucción enviada</strong><br>
      Dado que el mensaje con instrucciones es entregado,<br>
      Cuando el sistema confirma la entrega,<br>
      Entonces registra el evento 'Instrucción de pago enviada' con timestamp.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>39</th>
    <th>Epic ID</th>
    <th>09</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Reportar pago digital realizado</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero reportar que realicé el pago enviando el comprobante al chatbot para que el comerciante pueda verificarlo.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Reporte exitoso del comprobante de pago</strong><br>
      Dado que el cliente realizó el pago por Yape o Plin,<br>
      Cuando envía el comprobante al chatbot,<br>
      Entonces el sistema registra 'Pago digital reportado' y notifica al comerciante en el dashboard.<br><br>
      <strong>Scenario 2: Timeout sin reporte de pago</strong><br>
      Dado que el cliente recibió las instrucciones de pago,<br>
      Cuando transcurren 30 minutos sin que el cliente reporte el pago,<br>
      Entonces el chatbot envía un recordatorio y el pedido permanece en estado 'esperando pago'.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>40</th>
    <th>Epic ID</th>
    <th>09</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Validar pago desde el dashboard</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como comerciante, quiero revisar y aprobar o rechazar el pago reportado desde el dashboard para confirmar que el dinero fue recibido.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Comerciante visualiza pedidos con pago pendiente</strong><br>
      Dado que el cliente reportó su pago,<br>
      Cuando el comerciante revisa el pedido en el dashboard,<br>
      Entonces visualiza el comprobante, el monto y los detalles del pedido.<br><br>
      <strong>Scenario 2: Aprobación del pago por el comerciante</strong><br>
      Dado que el comerciante verifica que el pago es correcto,<br>
      Cuando lo aprueba,<br>
      Entonces el sistema registra 'Pago validado manualmente' y continúa el flujo.<br><br>
      <strong>Scenario 3: Rechazo del pago por el comerciante</strong><br>
      Dado que el comerciante detecta un pago incorrecto,<br>
      Cuando lo rechaza indicando el motivo,<br>
      Entonces el chatbot notifica al cliente y le indica los pasos a seguir.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>41</th>
    <th>Epic ID</th>
    <th>09</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Notificar estado del pago al cliente</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero recibir una notificación sobre si mi pago fue aprobado o rechazado para saber si mi pedido está confirmado.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Notificación de pago aprobado</strong><br>
      Dado que el comerciante aprueba el pago,<br>
      Cuando el sistema actualiza el estado,<br>
      Entonces el chatbot envía al cliente un mensaje confirmando que su pago fue recibido y el pedido está en proceso.<br><br>
      <strong>Scenario 2: Notificación de pago rechazado</strong><br>
      Dado que el comerciante rechaza el pago,<br>
      Cuando el sistema actualiza el estado,<br>
      Entonces el chatbot informa al cliente que no fue validado y solicita que lo intente nuevamente.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>42</th>
    <th>Epic ID</th>
    <th>10</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Confirmar pedido y descontar stock</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como sistema, quiero confirmar el pedido automáticamente al aprobar el pago para actualizar el inventario en tiempo real.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Confirmación de pedido y descuento de inventario</strong><br>
      Dado que el comerciante aprueba el pago,<br>
      Cuando el sistema confirma el pedido,<br>
      Entonces actualiza el estado a 'confirmado' y descuenta el stock de cada producto del inventario.<br><br>
      <strong>Scenario 2: Actualización de peso en balanza IoT</strong><br>
      Dado que el pedido incluye productos por peso,<br>
      Cuando el sistema descuenta el stock,<br>
      Entonces actualiza el peso disponible en la balanza IoT.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>43</th>
    <th>Epic ID</th>
    <th>10</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Registrar venta en el sistema</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como comerciante, quiero que cada pedido confirmado quede registrado como venta para tener un control financiero preciso.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Venta registrada correctamente</strong><br>
      Dado que el pedido ha sido confirmado,<br>
      Cuando el sistema registra la venta,<br>
      Entonces crea un registro con monto total, método de pago, productos y timestamp.<br><br>
      <strong>Scenario 2: Venta digital separada del efectivo en caja</strong><br>
      Dado que el pago fue digital (Yape/Plin),<br>
      Cuando se registra la venta,<br>
      Entonces el monto queda asociado al canal de pagos digitales, separado del efectivo en caja.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>44</th>
    <th>Epic ID</th>
    <th>10</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Emitir comprobante al cliente</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero recibir un comprobante de mi compra por WhatsApp para tener un respaldo de la transacción.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Comprobante enviado al cliente por WhatsApp</strong><br>
      Dado que la venta ha sido registrada,<br>
      Cuando el sistema genera el comprobante,<br>
      Entonces el chatbot envía al cliente un resumen con número de pedido, productos, cantidades, monto total y fecha.<br><br>
      <strong>Scenario 2: Pedido marcado como completado</strong><br>
      Dado que el comprobante es emitido,<br>
      Cuando el chatbot lo entrega,<br>
      Entonces el sistema registra 'Comprobante emitido' y el pedido pasa a estado 'completado'.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>45</th>
    <th>Epic ID</th>
    <th>11</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Manejar stock insuficiente</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como cliente, quiero ser notificado si un producto no tiene stock suficiente para poder ajustar mi pedido.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Notificación de stock insuficiente al cliente</strong><br>
      Dado que el cliente solicita una cantidad mayor al stock disponible,<br>
      Cuando el sistema valida el inventario,<br>
      Entonces el chatbot notifica qué producto no tiene stock y ofrece ajustar la cantidad o eliminarlo.<br><br>
      <strong>Scenario 2: Cliente ajusta la cantidad del producto</strong><br>
      Dado que el chatbot informó al cliente sobre el stock insuficiente,<br>
      Cuando el cliente confirma una nueva cantidad menor o igual al stock disponible,<br>
      Entonces el sistema actualiza el pedido y continúa el flujo normalmente.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>46</th>
    <th>Epic ID</th>
    <th>11</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Cancelar pedido por timeout de pago</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como sistema, quiero cancelar automáticamente un pedido si el cliente no reporta el pago en el tiempo establecido para liberar el stock reservado.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Cancelación automática por timeout</strong><br>
      Dado que el cliente recibió las instrucciones de pago,<br>
      Cuando transcurren 60 minutos sin reporte de pago,<br>
      Entonces el sistema cancela el pedido, libera el stock y notifica al cliente por WhatsApp.<br><br>
      <strong>Scenario 2: Registro del evento de cancelación</strong><br>
      Dado que el pedido es cancelado por timeout,<br>
      Cuando el sistema actualiza el estado,<br>
      Entonces registra el evento de cancelación con motivo 'timeout de pago' para trazabilidad.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>47</th>
    <th>Epic ID</th>
    <th>11</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Rechazar pago fraudulento o incorrecto</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como comerciante, quiero poder rechazar un pago si el comprobante es incorrecto para proteger el negocio de fraudes.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Rechazo manual por comprobante sospechoso</strong><br>
      Dado que el comerciante revisa un comprobante sospechoso,<br>
      Cuando lo rechaza indicando el motivo,<br>
      Entonces el pedido vuelve a 'esperando pago' y el chatbot notifica al cliente.<br><br>
      <strong>Scenario 2: Alerta por rechazos repetidos del mismo cliente</strong><br>
      Dado que el mismo cliente presenta pagos rechazados dos veces,<br>
      Cuando el sistema detecta el patrón,<br>
      Entonces alerta al comerciante y bloquea el pedido para revisión manual.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>User Story</th>
    <th>48</th>
    <th>Epic ID</th>
    <th>12</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Conocer la propuesta de valor</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como visitante, quiero entender qué hace Entreprenly y cómo puede beneficiar a mi negocio para decidir si me interesa adquirirlo.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Sección hero visible al cargar la página</strong><br>
      Dado que el visitante accede a la landing page,<br>
      Cuando la página carga,<br>
      Entonces visualiza el headline, la propuesta de valor y los beneficios clave en la sección hero.<br><br>
      <strong>Scenario 2: Sección de funcionalidades al hacer scroll</strong><br>
      Dado que el visitante navega a la sección de funcionalidades,<br>
      Cuando hace scroll,<br>
      Entonces visualiza las características principales: chatbot WhatsApp, inventario, balanza IoT y dashboard financiero.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>User Story</th>
    <th>49</th>
    <th>Epic ID</th>
    <th>12</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">API: crear y actualizar pedido</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como developer, quiero endpoints POST /api/orders y PATCH /api/orders/:id para gestionar el ciclo de vida completo de un pedido.
    </td>
  </tr><br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Creación exitosa de un pedido</strong><br>
      Dado que el chatbot envía POST /api/orders con datos válidos,<br>
      Cuando el servidor valida el cuerpo,<br>
      Entonces responde HTTP 201 Created con el pedido: id, estado 'pendiente' y timestamp.<br><br>
      <strong>Scenario 2: Actualización de estado de un pedido</strong><br>
      Dado que se envía PATCH /api/orders/:id con estado válido,<br>
      Cuando el servidor procesa la actualización,<br>
      Entonces responde HTTP 200 con el objeto pedido actualizado.<br><br>
      <strong>Scenario 3: Pedido no encontrado</strong><br>
      Dado que el id del pedido no existe,<br>
      Cuando el servidor busca el recurso,<br>
      Entonces responde HTTP 404 Not Found.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>50</th>
    <th>Epic ID</th>
    <th>12</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">API: validar y registrar pago</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como developer, quiero un endpoint PATCH /api/payments/:id para que el comerciante apruebe o rechace pagos desde el dashboard.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Aprobación de pago y descuento de stock</strong><br>
      Dado que se envía PATCH /api/payments/:id con status: 'aprobado',<br>
      Cuando el servidor procesa la validación,<br>
      Entonces responde HTTP 200, actualiza el pedido a 'confirmado' y descuenta el stock.<br><br>
      <strong>Scenario 2: Rechazo de pago con motivo registrado</strong><br>
      Dado que se envía PATCH /api/payments/:id con status: 'rechazado' y motivo,<br>
      Cuando el servidor procesa el rechazo,<br>
      Entonces responde HTTP 200 y registra el motivo en el historial.<br><br>
      <strong>Scenario 3: Pago no encontrado</strong><br>
      Dado que el id de pago no existe,<br>
      Cuando el servidor busca el recurso,<br>
      Entonces responde HTTP 404 Not Found.
    </td>
  </tr>
</table>
</div>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>51</th>
    <th>Epic ID</th>
    <th>13</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Registro de cuenta con email</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario anónimo, quiero registrarme con mi email y contraseña para crear una cuenta en Entreprenly.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Registro exitoso</strong><br>
      Dado que el usuario ingresa un email no registrado y una contraseña válida,<br>
      Cuando envía el formulario de registro,<br>
      Entonces el sistema crea la cuenta, envía un email de verificación y muestra un mensaje de confirmación.<br><br>
      <strong>Scenario 2: Email ya registrado</strong><br>
      Dado que el usuario ingresa un email que ya existe en el sistema,<br>
      Cuando envía el formulario de registro,<br>
      Entonces el sistema muestra un mensaje de error indicando que el email ya está en uso.<br><br>
      <strong>Scenario 3: Datos inválidos</strong><br>
      Dado que el usuario ingresa una contraseña que no cumple los requisitos mínimos,<br>
      Cuando envía el formulario,<br>
      Entonces el sistema muestra los errores de validación correspondientes sin crear la cuenta.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>52</th>
    <th>Epic ID</th>
    <th>13</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Verificación de email</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario registrado, quiero verificar mi email mediante el enlace enviado a mi correo para activar mi cuenta.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Verificación exitosa</strong><br>
      Dado que el usuario hace clic en el enlace de verificación válido,<br>
      Cuando el sistema valida el token,<br>
      Entonces la cuenta queda activa y el usuario es redirigido al dashboard principal.<br><br>
      <strong>Scenario 2: Token expirado</strong><br>
      Dado que el usuario hace clic en un enlace de verificación cuyo token ha expirado,<br>
      Cuando el sistema intenta validarlo,<br>
      Entonces muestra un mensaje de error y ofrece la opción de reenviar el email de verificación.<br><br>
      <strong>Scenario 3: Token inválido</strong><br>
      Dado que el usuario accede a un enlace de verificación con un token malformado,<br>
      Cuando el sistema intenta procesarlo,<br>
      Entonces muestra un mensaje de error indicando que el enlace no es válido.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>53</th>
    <th>Epic ID</th>
    <th>13</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Inicio de sesión con credenciales</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario registrado, quiero iniciar sesión con mi email y contraseña para acceder al dashboard de Entreprenly.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Inicio de sesión exitoso</strong><br>
      Dado que el usuario ingresa credenciales válidas,<br>
      Cuando envía el formulario de login,<br>
      Entonces el sistema genera un JWT, inicia la sesión y redirige al dashboard principal.<br><br>
      <strong>Scenario 2: Credenciales inválidas</strong><br>
      Dado que el usuario ingresa una contraseña incorrecta,<br>
      Cuando envía el formulario de login,<br>
      Entonces el sistema muestra un mensaje de error sin revelar cuál campo es incorrecto.<br><br>
      <strong>Scenario 3: Cuenta bloqueada por intentos fallidos</strong><br>
      Dado que el usuario ha fallado 5 intentos consecutivos de inicio de sesión,<br>
      Cuando intenta iniciar sesión nuevamente,<br>
      Entonces el sistema bloquea la cuenta y notifica al usuario por email.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>User Story</th>
    <th>54</th>
    <th>Epic ID</th>
    <th>13</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Inicio de sesión con Google OAuth</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario anónimo, quiero iniciar sesión con mi cuenta de Google para acceder a Entreprenly sin necesidad de crear credenciales nuevas.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: OAuth exitoso con cuenta nueva</strong><br>
      Dado que el usuario inicia el flujo OAuth con una cuenta de Google no registrada previamente,<br>
      Cuando Google autoriza el acceso y devuelve el token,<br>
      Entonces el sistema crea una nueva cuenta vinculada al proveedor e inicia la sesión.<br><br>
      <strong>Scenario 2: OAuth exitoso con cuenta existente</strong><br>
      Dado que el usuario inicia el flujo OAuth con un email ya registrado en el sistema,<br>
      Cuando Google devuelve el token,<br>
      Entonces el sistema vincula el proveedor a la cuenta existente e inicia la sesión.<br><br>
      <strong>Scenario 3: OAuth denegado por el usuario</strong><br>
      Dado que el usuario cancela la autorización en la pantalla de Google,<br>
      Cuando el flujo OAuth es interrumpido,<br>
      Entonces el sistema redirige al usuario a la pantalla de login sin crear ninguna cuenta.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>User Story</th>
    <th>55</th>
    <th>Epic ID</th>
    <th>13</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Recuperación de contraseña</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario registrado, quiero recuperar el acceso a mi cuenta mediante un enlace enviado a mi email para restablecer mi contraseña.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Reset exitoso</strong><br>
      Dado que el usuario solicita el reset con un email registrado y confirma la nueva contraseña desde el enlace recibido,<br>
      Cuando el sistema procesa la solicitud,<br>
      Entonces actualiza la contraseña, invalida todas las sesiones anteriores y redirige al login.<br><br>
      <strong>Scenario 2: Token de reset expirado</strong><br>
      Dado que el usuario accede al enlace de reset después de que el token ha expirado,<br>
      Cuando el sistema intenta validarlo,<br>
      Entonces muestra un mensaje de error y solicita generar un nuevo enlace.<br><br>
      <strong>Scenario 3: Email no registrado</strong><br>
      Dado que el usuario solicita el reset con un email que no existe en el sistema,<br>
      Cuando envía el formulario,<br>
      Entonces el sistema responde con un mensaje genérico sin confirmar ni negar la existencia del email.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>56</th>
    <th>Epic ID</th>
    <th>13</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Cierre de sesión</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero cerrar mi sesión para que el sistema revoque mi token y me redirija a la pantalla de login.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Cierre de sesión exitoso</strong><br>
      Dado que el usuario hace clic en la opción de cerrar sesión,<br>
      Cuando el sistema procesa la solicitud,<br>
      Entonces revoca el JWT activo y redirige al usuario a la pantalla de login.<br><br>
      <strong>Scenario 2: Intento de acceso tras cerrar sesión</strong><br>
      Dado que el usuario ha cerrado su sesión y el token ha sido revocado,<br>
      Cuando intenta acceder a una ruta protegida,<br>
      Entonces el sistema rechaza la solicitud y redirige al login.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>57</th>
    <th>Epic ID</th>
    <th>14</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Visualizar perfil actual</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero visualizar mi perfil actual para revisar mis datos registrados en la plataforma.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Visualización exitosa</strong><br>
      Dado que el usuario navega a la sección de perfil,<br>
      Cuando el sistema carga los datos,<br>
      Entonces muestra nombre, bio, foto de perfil, email y preferencias actuales del usuario.<br><br>
      <strong>Scenario 2: Sesión expirada</strong><br>
      Dado que la sesión del usuario ha expirado,<br>
      Cuando intenta acceder a la sección de perfil,<br>
      Entonces el sistema redirige al login.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>User Story</th>
    <th>58</th>
    <th>Epic ID</th>
    <th>14</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Actualizar nombre y biografía</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero actualizar mi nombre y biografía para mantener mi perfil al día.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Actualización exitosa</strong><br>
      Dado que el usuario edita su nombre y/o bio con datos válidos,<br>
      Cuando guarda los cambios,<br>
      Entonces el sistema actualiza los datos y muestra el perfil con la información nueva.<br><br>
      <strong>Scenario 2: Campo obligatorio vacío</strong><br>
      Dado que el usuario deja el campo de nombre vacío,<br>
      Cuando intenta guardar,<br>
      Entonces el sistema muestra un error de validación sin guardar los cambios.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>59</th>
    <th>Epic ID</th>
    <th>14</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Subir foto de perfil</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero subir una foto de perfil para personalizar mi cuenta en la plataforma.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Subida exitosa</strong><br>
      Dado que el usuario selecciona una imagen con formato y tamaño permitidos,<br>
      Cuando la sube al sistema,<br>
      Entonces el servicio de almacenamiento guarda el archivo, actualiza la URL del avatar y muestra la nueva foto en el perfil.<br><br>
      <strong>Scenario 2: Formato de imagen no permitido</strong><br>
      Dado que el usuario intenta subir un archivo con formato no soportado,<br>
      Cuando el sistema valida el archivo,<br>
      Entonces muestra un mensaje de error indicando los formatos aceptados sin guardar el archivo.<br><br>
      <strong>Scenario 3: Tamaño de archivo excedido</strong><br>
      Dado que el usuario intenta subir una imagen que supera el tamaño máximo permitido,<br>
      Cuando el sistema valida el archivo,<br>
      Entonces muestra un mensaje de error indicando el límite de tamaño.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>60</th>
    <th>Epic ID</th>
    <th>14</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Cambiar email con re-verificación</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero cambiar mi email y verificarlo para mantener mis datos de contacto actualizados.
    </td>
  </tr>
<br><br>

  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Cambio de email exitoso</strong><br>
      Dado que el usuario solicita cambiar su email a uno no registrado previamente,<br>
      Cuando confirma el nuevo email desde el enlace enviado,<br>
      Entonces el sistema actualiza el email y lo marca como verificado.<br><br>
      <strong>Scenario 2: Nuevo email ya en uso</strong><br>
      Dado que el usuario ingresa un email que ya pertenece a otra cuenta,<br>
      Cuando intenta guardar el cambio,<br>
      Entonces el sistema muestra un mensaje de error sin actualizar el email.<br><br>
      <strong>Scenario 3: Confirmación desde enlace expirado</strong><br>
      Dado que el usuario hace clic en el enlace de confirmación después de que ha expirado,<br>
      Cuando el sistema valida el token,<br>
      Entonces muestra un mensaje de error y ofrece reenviar el email de confirmación.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>61</th>
    <th>Epic ID</th>
    <th>14</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Cambiar contraseña</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero cambiar mi contraseña para mantener la seguridad de mi cuenta.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Cambio exitoso</strong><br>
      Dado que el usuario ingresa su contraseña actual correcta y una nueva contraseña válida,<br>
      Cuando guarda el cambio,<br>
      Entonces el sistema actualiza la contraseña e invalida todas las sesiones activas excepto la actual.<br><br>
      <strong>Scenario 2: Contraseña actual incorrecta</strong><br>
      Dado que el usuario ingresa una contraseña actual incorrecta,<br>
      Cuando intenta guardar el cambio,<br>
      Entonces el sistema muestra un error de validación sin actualizar la contraseña.<br><br>
      <strong>Scenario 3: Nueva contraseña no cumple requisitos</strong><br>
      Dado que el usuario ingresa una nueva contraseña que no cumple los requisitos mínimos,<br>
      Cuando intenta guardar,<br>
      Entonces el sistema muestra los requisitos incumplidos sin aplicar el cambio.
    </td>
  </tr>
</table>

<table>
  <tr>
    <th>User Story</th>
    <th>62</th>
    <th>Epic ID</th>
    <th>14</th>
  </tr>
  <br><br>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Configurar preferencias de idioma, zona horaria y tema</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero configurar mi idioma, zona horaria y tema visual para adaptar la plataforma a mis preferencias.
    </td>
  </tr>
  <br><br>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Cambio de idioma exitoso</strong><br>
      Dado que el usuario selecciona un idioma disponible,<br>
      Cuando guarda la preferencia,<br>
      Entonces el sistema actualiza el idioma de la interfaz de forma inmediata.<br><br>
      <strong>Scenario 2: Cambio de zona horaria exitoso</strong><br>
      Dado que el usuario selecciona una zona horaria de la lista disponible,<br>
      Cuando guarda la preferencia,<br>
      Entonces el sistema almacena la zona horaria y la aplica en las fechas mostradas.<br><br>
      <strong>Scenario 3: Cambio de tema exitoso</strong><br>
      Dado que el usuario selecciona el tema claro u oscuro,<br>
      Cuando guarda la preferencia,<br>
      Entonces el sistema aplica el tema seleccionado de forma inmediata y lo persiste para futuras sesiones.
    </td>
  </tr>
</table>
<br><br>
<table>
  <tr>
    <th>User Story</th>
    <th>63</th>
    <th>Epic ID</th>
    <th>14</th>
  </tr>
  <tr>
    <td><strong>Title</strong></td>
    <td colspan="3">Configurar notificaciones</td>
  </tr>
  <tr>
    <td><strong>Description</strong></td>
    <td colspan="3">
      Como usuario autenticado, quiero configurar mis preferencias de notificación para recibir solo los avisos que me sean relevantes.
    </td>
  </tr>
  <tr>
    <td><strong>Acceptance Criteria</strong></td>
    <td colspan="3">
      <strong>Scenario 1: Guardado exitoso de preferencias</strong><br>
      Dado que el usuario activa o desactiva tipos de notificación disponibles,<br>
      Cuando guarda los cambios,<br>
      Entonces el sistema almacena las preferencias y las aplica en los envíos futuros.<br><br>
      <strong>Scenario 2: Sin cambios realizados</strong><br>
      Dado que el usuario accede a la sección de notificaciones sin modificar nada,<br>
      Cuando sale de la sección,<br>
      Entonces el sistema mantiene las preferencias anteriores sin alteración.
    </td>
  </tr>
</table>

## 3.2. Impact Mapping

_Contenido por agregar._

## 3.3. Product Backlog

_Contenido por agregar._
