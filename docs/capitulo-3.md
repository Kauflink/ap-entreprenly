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
    <td align="center">VIsualización de detalles de Producto</td>
  </tr>
  <tr>
    <td align="center">5</td>
    <td align="center">Edición de Productos</td>
  </tr>
  <tr>
    <td align="center">6</td>
    <td align="center">Visualización de detalles de Lotes</td>
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

  <tr>
    <td align="center">13</td>
    <td align="center">Mostrar labels de Lotes vencidos</td>
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

## 3.2. Impact Mapping

*Contenido por agregar.*

## 3.3. Product Backlog

*Contenido por agregar.*