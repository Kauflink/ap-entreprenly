# Capítulo III: Requirements Specification

## 3.1. User Stories

<table>
  <thead>
    <tr>
      <th>Epic / Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>Relacionado con (Epic ID)</th>
    </tr>
  </thead>
  <tbody>
  <!-- EPIC 01 -->
  <tr>
    <td><strong>Epic-01</strong></td>
    <td><strong>Gestión de inventario</strong></td>
    <td>Como usuario quiero gestionar mi inventario (lotes y productos) para visualizar los datos con mayor claridad.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 01 -->
  <tr>
    <td>US-01</td>
    <td>Agregar productos</td>
    <td>Como usuario quiero agregar productos para gestionar mi inventario de manera eficiente.</td>
    <td>
      <strong>Scenario 1: Agregar producto correctamente</strong><br>
      Dado que el usuario está en el formulario de productos, cuando ingrese los datos correctamente y presione "Guardar", entonces el producto se registrará exitosamente.<br><br>
      <strong>Scenario 2: Validación de datos</strong><br>
      Dado que el usuario está en el formulario de productos, cuando deje campos obligatorios vacíos y presione "Guardar", entonces el sistema mostrará mensajes de error.
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 02 -->
  <tr>
    <td>US-02</td>
    <td>Editar lotes</td>
    <td>Como usuario quiero editar los lotes para actualizar los datos del inventario.</td>
    <td>
      <strong>Scenario 1: Editar lote correctamente</strong><br>
      Dado que el usuario está en la sección de lotes y selecciona un lote existente, cuando modifique los datos correctamente y presione "Guardar", entonces los cambios del lote se actualizarán exitosamente.<br><br>
      <strong>Scenario 2: Validación al editar lote</strong><br>
      Dado que el usuario está editando un lote, cuando ingrese datos inválidos o deje campos obligatorios vacíos y presione "Guardar", entonces el sistema mostrará mensajes de error y no guardará los cambios.
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 03 -->
  <tr>
    <td>US-03</td>
    <td>Agregar lotes</td>
    <td>Como usuario quiero agregar lotes para gestionar correctamente las cantidades y fechas de vencimiento.</td>
    <td>
      <strong>Scenario 1: Agregar lote correctamente</strong><br>
      Dado que el usuario está en la sección de lotes y selecciona un lote existente, cuando ingrese una cantidad y fecha válida y presione "Agregar", entonces el nuevo lote se agregará exitosamente.<br><br>
      <strong>Scenario 2: Intento de registro de lote con información incompleta</strong><br>
      Dado que el usuario se encuentra en el formulario de Agregación de Lotes. 
      Cuando intenta procesar la solicitud dejando uno o más campos obligatorios vacíos.
      Entonces el sistema debe impedir el registro y resaltar cada campo omitido con el mensaje: "Este campo es obligatorio".
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 04 -->
  <tr>
    <td>US-04</td>
    <td>Eliminar lotes</td>
    <td>Como usuario quiero eliminar lotes para deshacerme de los lotes que no me sirvan.</td>
    <td>
      <strong>Scenario 1: Eliminar lote correctamente</strong><br>
      Dado que el usuario está en la sección de lotes y selecciona un lote existente, cuando presione "Eliminar", entonces el lote se eliminará exitosamente.<br><br>
      <strong>Scenario 2: Validación al eliminar lote</strong><br>
      Dado que el usuario está en la sección de lotes y no selecciona un lote existente, cuando presione "Eliminar", entonces saldrá un mensaje de error de no haber seleccionado un lote.
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 05 -->
  <tr>
    <td>US-05</td>
    <td>Editar productos</td>
    <td>Como usuario quiero editar productos para actualizar los datos en el inventario.</td>
    <td>
      <strong>Scenario 1: Producto editado correctamente</strong><br>
      Dado que el usuario está en la sección de productos y selecciona un producto existente, cuando presione "Editar", entonces el producto se actualizará exitosamente.<br><br>
      <strong>Scenario 2: Validación al editar productos</strong><br>
      Dado que el usuario se encuentra en la lista de inventario y ha seleccionado un producto existente, cuando el usuario intenta cambiar el "Tipo de Producto" y presiona el botón de guardar, entonces el sistema debe impedir la acción y mostrar un mensaje de error indicando: "Este campo no se puede modificar".
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 06 -->
  <tr>
    <td>US-06</td>
    <td>Visualizar detalles de lotes</td>
    <td>Como usuario quiero visualizar los detalles de los lotes para gestionar mejor el inventario.</td>
    <td>
      <strong>Scenario 1: Detalles de lote mostrados correctamente</strong><br>
      Dado que el usuario está en la sección de lotes y selecciona un lote existente, cuando presione "Ver Detalles", entonces los detalles se mostrarán exitosamente.<br><br>
      <strong>Scenario 2: Error al recuperar los detalles del lote</strong><br>
      Dado que el usuario visualiza la tarjeta de un producto con lotes existentes.
      Cuando el usuario presiona "Ver Detalles" pero ocurre un error de comunicación con el servidor (timeout o error 500).
      Entonces el sistema debe mostrar un mensaje de error indicando: "No se pudieron cargar los detalles en este momento. Inténtelo más tarde".
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 10 -->
  <tr>
    <td>US-10</td>
    <td>Visualizar detalles de producto</td>
    <td>Como usuario quiero visualizar la información detallada de cada producto en el listado para conocer rápidamente sus características, stock disponible y precio sin necesidad de ingresar a otra pantalla.</td>
    <td>
      <strong>Scenario 1: Visualización de información del producto</strong><br>
      Dado que el usuario accede al listado de productos, cuando se carga la información, entonces cada producto debe mostrar: tipo, nombre, descripción, código QR, stock total y precio.<br><br>
      <strong>Scenario 2: Manejo de información incompleta del producto</strong><br>
      Dado que un producto no cuenta con algún dato, cuando se carga la información, entonces el sistema muestra los datos disponibles y los campos faltantes aparecen como "-".
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 12 -->
  <tr>
    <td>US-12</td>
    <td>Buscar productos</td>
    <td>Como usuario quiero tener un buscador de productos para perder menos tiempo buscando en el inventario.</td>
    <td>
      <strong>Scenario 1: Búsqueda de productos por nombre</strong><br>
      Dado que el usuario está en el listado de productos, cuando ingresa el nombre de un producto en el campo de búsqueda, entonces el sistema filtra y muestra los productos que coincidan.<br><br>
      <strong>Scenario 2: Búsqueda de productos por categoría</strong><br>
      Dado que el usuario está en el listado de productos, cuando selecciona o ingresa una categoría, entonces el sistema filtra y muestra los productos de esa categoría.
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- US 23 -->
  <tr>
    <td>US-23</td>
    <td>Crear lotes</td>
    <td>Como usuario quiero crear lotes de productos para controlar mejor el stock y la caducidad en el inventario.</td>
    <td>
      <strong>Scenario 1: Creación de lote exitosa</strong><br>
      Dado que el usuario está en la sección de productos, cuando presiona "Crear Lote", selecciona un producto y completa los datos correctamente, entonces el sistema registra el nuevo lote y lo muestra en la lista.<br><br>
      <strong>Scenario 2: Validación al crear lote</strong><br>
      Dado que el usuario no selecciona un producto o ingresa datos incompletos, entonces el sistema muestra mensajes de error y no permite la creación del lote.
    </td>
    <td>Epic-01</td>
  </tr>
  <!-- EPIC 02 -->
  <tr>
    <td><strong>Epic-02</strong></td>
    <td><strong>Notificaciones de inventario</strong></td>
    <td>Como usuario quiero que el sistema me notifique el estado de mis lotes para organizarme mejor.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 07 -->
  <tr>
    <td>US-07</td>
    <td>Detectar stock agotado</td>
    <td>Como usuario quiero ser notificado cuando tengo bajo/nada de stock.</td>
    <td>
      <strong>Scenario 1: Alerta de stock próximo a agotarse</strong><br>
      Dado que uno o más lotes tienen stock por debajo del umbral definido, cuando el usuario accede al dashboard de lotes, entonces se muestra una alerta visible indicando los lotes próximos a agotarse.<br><br>
      <strong>Scenario 2: Alerta de stock agotado</strong><br>
      Dado que uno o más lotes están agotados, cuando el usuario accede al dashboard, entonces se muestra una alerta indicando los lotes agotados.
    </td>
    <td>Epic-02</td>
  </tr>
  <!-- US 08 -->
  <tr>
    <td>US-08</td>
    <td>Mostrar alertas de estado al visualizar detalles</td>
    <td>Como usuario quiero visualizar alertas de estado al ver el detalle de un lote para identificar rápidamente si tiene stock bajo, está agotado o próximo a vencer.</td>
    <td>
      <strong>Scenario 1: Alerta de estado mostrada</strong><br>
      Dado que el lote tiene stock bajo, está agotado o próximo a vencer, cuando presiona "Ver Detalles", entonces se mostrarán los detalles del lote con alertas de estado.<br><br>
      <strong>Scenario 2: Sin alertas si el estado es normal</strong><br>
      Dado que el lote no tiene condiciones críticas, cuando presiona "Ver Detalles", entonces se muestran los detalles sin alertas.
    </td>
    <td>Epic-02</td>
  </tr>
  <!-- US 09 -->
  <tr>
    <td>US-09</td>
    <td>Visualizar dashboard de lotes</td>
    <td>Como usuario quiero visualizar un dashboard de lotes con indicadores y alertas para conocer rápidamente el estado de mi inventario al ingresar al módulo de lotes.</td>
    <td>
      <strong>Scenario 1: Visualización de resumen de lotes</strong><br>
      Dado que el usuario ingresa al módulo de lotes, cuando se carga la pantalla, entonces se muestra un resumen con indicadores clave sobre los estados de los lotes.<br><br>
      <strong>Scenario 2: Sin alertas si no hay condiciones críticas</strong><br>
      Dado que no existen lotes vencidos ni próximos a vencer, cuando se carga el dashboard, entonces no se muestra el banner de alertas.
    </td>
    <td>Epic-02</td>
  </tr>
  <!-- US 11 -->
  <tr>
    <td>US-11</td>
    <td>Recibir alerta de caducidad de lote</td>
    <td>Como usuario quiero ser notificado cuando un lote esté próximo a vencer o ya haya vencido para tomar acciones como priorizar su uso o descartarlo.</td>
    <td>
      <strong>Scenario 1: Alerta de lote próximo a vencer</strong><br>
      Dado que uno o más lotes tienen fecha de caducidad dentro del rango próximo definido, cuando el usuario accede al dashboard de lotes, entonces se muestra una alerta indicando los lotes próximos a vencer.<br><br>
      <strong>Scenario 2: Alerta de lote vencido</strong><br>
      Dado que uno o más lotes tienen fecha de caducidad menor a la fecha actual, cuando el usuario accede al dashboard, entonces se muestra una alerta indicando los lotes vencidos.
    </td>
    <td>Epic-02</td>
  </tr>
  <!-- EPIC 03 -->
  <tr>
    <td><strong>Epic-03</strong></td>
    <td><strong>Proceso de suscripción</strong></td>
    <td>Como usuario con cuenta creada y Plan Free asignado por defecto, quiero iniciar la suscripción al Plan Control para habilitar las funcionalidades premium desde la landing o desde la sección "Suscripción" del dashboard.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 13 -->
  <tr>
    <td>US-13</td>
    <td>Seleccionar plan de suscripción</td>
    <td>Como usuario con Plan Free, quiero presionar el botón "Elegir plan" en la tarjeta del Plan Control para definir el plan que deseo contratar y continuar con el proceso de suscripción.</td>
    <td>
      <strong>Scenario 1: Selección de plan realizada correctamente</strong><br>
      Dado que el usuario visualiza los planes disponibles en la landing o en la sección "Suscripción", cuando presiona el botón "Elegir plan" de la tarjeta "Plan Control", entonces el sistema registra el plan seleccionado, resalta visualmente la tarjeta y habilita el botón "Continuar con la suscripción".<br><br>
      <strong>Scenario 2: Intento de continuar sin seleccionar un plan</strong><br>
      Dado que el usuario no ha presionado el botón "Elegir plan" en ninguna tarjeta, cuando intenta hacer clic en "Continuar con la suscripción", entonces el sistema no permite avanzar y muestra un mensaje indicando que debe seleccionar un plan primero.
    </td>
    <td>Epic-03</td>
  </tr>
  <!-- US 14 -->
  <tr>
    <td>US-14</td>
    <td>Iniciar proceso de suscripción</td>
    <td>Como usuario con un plan seleccionado, quiero presionar el botón "Continuar con la suscripción" para abrir el formulario de facturación y comenzar formalmente la contratación del plan elegido.</td>
    <td>
      <strong>Scenario 1: Proceso de suscripción iniciado correctamente</strong><br>
      Dado que el usuario ya seleccionó el Plan Control, cuando presiona el botón "Continuar con la suscripción", entonces el sistema registra el inicio del proceso y lo redirige al formulario de facturación.<br><br>
      <strong>Scenario 2: Intento sin plan seleccionado</strong><br>
      Dado que el usuario no ha seleccionado un plan, cuando presiona el botón "Continuar con la suscripción", entonces el sistema no permite iniciar el proceso y muestra un mensaje solicitando seleccionar un plan primero.
    </td>
    <td>Epic-03</td>
  </tr>
  <!-- US 15 -->
  <tr>
    <td>US-15</td>
    <td>Registrar datos de facturación</td>
    <td>Como usuario, quiero completar el formulario de facturación y presionar el botón "Continuar al pago" para que el sistema pueda preparar el cobro correspondiente a la suscripción.</td>
    <td>
      <strong>Scenario 1: Datos de facturación registrados correctamente</strong><br>
      Dado que el usuario completa correctamente los campos obligatorios del formulario de facturación y presiona el botón "Continuar al pago", cuando el sistema valida la información, entonces registra los datos y habilita el resumen previo al cobro.<br><br>
      <strong>Scenario 2: Datos de facturación inválidos</strong><br>
      Dado que el usuario ingresa datos incompletos o inválidos en el formulario, cuando presiona el botón "Continuar al pago", entonces el sistema no registra la información, resalta los campos con error y muestra un mensaje de validación.
    </td>
    <td>Epic-03</td>
  </tr>
  <!-- US 16 -->
  <tr>
    <td>US-16</td>
    <td>Procesar cobro de suscripción</td>
    <td>Como usuario, quiero revisar el resumen de cobro y presionar el botón "Pagar y activar suscripción" para validar el pago del Plan Control seleccionado.</td>
    <td>
      <strong>Scenario 1: Cobro procesado exitosamente</strong><br>
      Dado que el usuario ya registró correctamente sus datos de facturación, cuando presiona el botón "Pagar y activar suscripción" y el cobro es aprobado, entonces el sistema registra el pago exitoso y habilita la activación de la suscripción.<br><br>
      <strong>Scenario 2: Error durante el procesamiento del cobro</strong><br>
      Dado que el usuario presionó el botón "Pagar y activar suscripción", cuando ocurre un error durante el cobro (tarjeta rechazada o datos inválidos), entonces el sistema no activa la suscripción y muestra el motivo del error dentro de la misma vista.
    </td>
    <td>Epic-03</td>
  </tr>
  <!-- US 17 -->
  <tr>
    <td>US-17</td>
    <td>Activar suscripción</td>
    <td>Como usuario, quiero que al confirmarse el pago el sistema active automáticamente el Plan Control y me redirija al panel de suscripción para acceder a las funcionalidades premium.</td>
    <td>
      <strong>Scenario 1: Activación de suscripción exitosa</strong><br>
      Dado que el cobro fue procesado correctamente, cuando el sistema confirma el pago, entonces activa el Plan Control, actualiza el estado de la suscripción a "Activa" y redirige al usuario al panel de suscripción con acceso a funcionalidades premium.<br><br>
      <strong>Scenario 2: Suscripción no activada por pago no confirmado</strong><br>
      Dado que el cobro no fue confirmado, cuando el sistema intenta activar la suscripción, entonces el Plan Control no se activa, la cuenta permanece en Plan Free y el usuario no accede a funcionalidades premium.
    </td>
    <td>Epic-03</td>
  </tr>
  <!-- EPIC 04 -->
  <tr>
    <td><strong>Epic-04</strong></td>
    <td><strong>Configuración de suscripción</strong></td>
    <td>Como usuario, quiero visualizar y gestionar mi plan actual desde la sección "Suscripción" del dashboard para consultar su estado, renovarlo o cancelarlo según mis necesidades.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 18 -->
  <tr>
    <td>US-18</td>
    <td>Visualizar panel de suscripción</td>
    <td>Como usuario, quiero hacer clic en la opción lateral "Suscripción" para ver un panel con el plan actual, estado, fecha de renovación, facturación y acciones disponibles.</td>
    <td>
      <strong>Scenario 1: Panel de suscripción mostrado correctamente</strong><br>
      Dado que el usuario presiona la opción lateral "Suscripción" dentro del dashboard, cuando el sistema carga la vista, entonces se muestra el panel con los datos generales del plan actual y las acciones relacionadas.<br><br>
      <strong>Scenario 2: Usuario con Plan Free por defecto</strong><br>
      Dado que el usuario solo tiene el Plan Free asignado por defecto, cuando carga la vista de "Suscripción", entonces el panel muestra el estado del Plan Free y la opción para actualizar al Plan Control.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- US 19 -->
  <tr>
    <td>US-19</td>
    <td>Consultar estado de suscripción</td>
    <td>Como usuario, quiero ver una etiqueta de estado en el panel de suscripción para saber si mi plan se encuentra en estado "Activa", "Cancelación programada", "Cancelada" o "Plan Free".</td>
    <td>
      <strong>Scenario 1: Estado activa mostrado correctamente</strong><br>
      Dado que el usuario tiene una suscripción vigente de pago, cuando ingresa al panel de "Suscripción", entonces el sistema muestra una etiqueta visible con el estado "Activa".<br><br>
      <strong>Scenario 2: Estado no activa mostrado correctamente</strong><br>
      Dado que el usuario tiene una suscripción cancelada, con cancelación programada o solo el Plan Free, cuando ingresa al panel de "Suscripción", entonces el sistema muestra la etiqueta correspondiente al estado real del plan.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- US 20 -->
  <tr>
    <td>US-20</td>
    <td>Renovar suscripción</td>
    <td>Como usuario con una suscripción de pago activa o próxima a vencer, quiero presionar el botón "Renovar suscripción" para extender la vigencia de mi acceso a la plataforma.</td>
    <td>
      <strong>Scenario 1: Renovación realizada correctamente</strong><br>
      Dado que el usuario tiene una suscripción activa o próxima a vencer, cuando presiona el botón "Renovar suscripción" y confirma la acción, entonces el sistema registra la renovación y actualiza la nueva fecha de vencimiento en el panel.<br><br>
      <strong>Scenario 2: Renovación no permitida</strong><br>
      Dado que el usuario se encuentra en Plan Free o no cuenta con una suscripción renovable, cuando presiona el botón "Renovar suscripción", entonces el sistema muestra un mensaje indicando que primero debe contratar o reactivar un plan de pago.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- US 21 -->
  <tr>
    <td>US-21</td>
    <td>Solicitar cancelación de suscripción</td>
    <td>Como usuario con una suscripción de pago activa, quiero presionar el botón "Solicitar cancelación" y luego "Confirmar cancelación" para detener la renovación automática al finalizar el periodo vigente.</td>
    <td>
      <strong>Scenario 1: Solicitud de cancelación registrada correctamente</strong><br>
      Dado que el usuario tiene una suscripción activa, cuando presiona el botón "Solicitar cancelación" y confirma la acción, entonces el sistema registra la solicitud y mantiene el acceso hasta la fecha de vencimiento.<br><br>
      <strong>Scenario 2: Usuario cancela la operación antes de confirmar</strong><br>
      Dado que el usuario inició el proceso de cancelación, cuando presiona el botón "Volver" o cierra el modal antes de confirmar, entonces el sistema no registra la cancelación y la suscripción continúa sin cambios.<br><br>
      <strong>Scenario 3: Mantener plan vigente</strong><br>
      Dado que el usuario visualiza el modal de confirmación para cancelar su suscripción, cuando presiona el botón "Mantener plan", entonces el sistema cierra el modal, no registra ninguna solicitud de cancelación y conserva el Plan Control activo con su fecha de renovación original.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- US 22 -->
  <tr>
    <td>US-22</td>
    <td>Cancelar suscripción</td>
    <td>Como sistema, quiero cancelar la suscripción de pago al finalizar su periodo vigente para retirar el acceso premium y devolver la cuenta del usuario al Plan Free.</td>
    <td>
      <strong>Scenario 1: Cancelación ejecutada correctamente</strong><br>
      Dado que existe una solicitud de cancelación registrada y la fecha de vencimiento ha sido alcanzada, cuando el sistema procesa el fin del periodo, entonces la suscripción de pago es cancelada, el acceso premium es retirado y la cuenta vuelve automáticamente al Plan Free.<br><br>
      <strong>Scenario 2: Suscripción aún dentro del periodo vigente</strong><br>
      Dado que la fecha de vencimiento aún no ha llegado, cuando el sistema verifica el estado, entonces la suscripción continúa activa, mantiene acceso premium y conserva el estado "Cancelación programada" hasta el final del periodo.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- US 71 -->
  <tr>
    <td>US-71</td>
    <td>Agregar método de pago de suscripción</td>
    <td>Como usuario con acceso al panel "Suscripción", quiero presionar el botón "Agregar método de pago" dentro de la sección "Método de pago y datos fiscales" para registrar un medio de cobro que pueda usarse en pagos y renovaciones del Plan Control.</td>
    <td>
      <strong>Scenario 1: Formulario de método de pago abierto</strong><br>
      Dado que el usuario se encuentra en la sección "Método de pago y datos fiscales", cuando presiona el botón "Agregar método de pago", entonces el sistema muestra un formulario o modal para registrar los datos del medio de pago.<br><br>
      <strong>Scenario 2: Método de pago registrado correctamente</strong><br>
      Dado que el usuario completa los datos requeridos del método de pago y presiona "Guardar método de pago", cuando el sistema valida la información, entonces el método queda asociado a la suscripción y se muestra en el panel como método disponible para futuros cobros.<br><br>
      <strong>Scenario 3: Método de pago inválido o cancelado</strong><br>
      Dado que el usuario ingresa datos incompletos, inválidos o cierra el formulario antes de guardar, cuando el sistema valida la acción, entonces no registra cambios y mantiene el estado anterior del método de pago.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- US 72 -->
  <tr>
    <td>US-72</td>
    <td>Completar datos fiscales de suscripción</td>
    <td>Como usuario con una cuenta registrada, quiero presionar el botón "Completar datos" dentro de "Método de pago y datos fiscales" para registrar mi RUC o DNI, razón social o nombre, dirección fiscal y correo de facturación.</td>
    <td>
      <strong>Scenario 1: Formulario de datos fiscales mostrado</strong><br>
      Dado que el usuario se encuentra en la sección "Método de pago y datos fiscales", cuando presiona el botón "Completar datos", entonces el sistema muestra un formulario con los campos fiscales requeridos para la facturación de la suscripción.<br><br>
      <strong>Scenario 2: Datos fiscales guardados correctamente</strong><br>
      Dado que el usuario completa los campos fiscales obligatorios y presiona "Guardar datos fiscales", cuando el sistema valida la información, entonces registra los datos y actualiza la sección mostrando que la información fiscal está completa.<br><br>
      <strong>Scenario 3: Datos fiscales incompletos o inválidos</strong><br>
      Dado que el usuario deja campos obligatorios vacíos o ingresa un documento inválido, cuando presiona "Guardar datos fiscales", entonces el sistema no guarda la información, resalta los campos con error y muestra un mensaje de validación.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- US 73 -->
  <tr>
    <td>US-73</td>
    <td>Descargar historial de suscripción</td>
    <td>Como usuario, quiero presionar el botón "Descargar historial" dentro de "Actividad de la suscripción" para obtener un archivo con los eventos de mi plan, pagos, renovaciones, cambios y cancelaciones.</td>
    <td>
      <strong>Scenario 1: Historial descargado correctamente</strong><br>
      Dado que existen eventos registrados en la actividad de la suscripción, cuando el usuario presiona el botón "Descargar historial", entonces el sistema genera y descarga un archivo con el historial de actividad visible para el usuario.<br><br>
      <strong>Scenario 2: Historial sin actividad suficiente</strong><br>
      Dado que la suscripción aún no tiene eventos relevantes registrados, cuando el usuario presiona "Descargar historial", entonces el sistema muestra un mensaje indicando que no hay actividad suficiente para descargar.<br><br>
      <strong>Scenario 3: Error al generar descarga</strong><br>
      Dado que ocurre un error al preparar el archivo, cuando el usuario intenta descargar el historial, entonces el sistema muestra un mensaje de error y mantiene disponible el botón para volver a intentarlo.
    </td>
    <td>Epic-04</td>
  </tr>
  <!-- EPIC 05 -->
  <tr>
    <td><strong>Epic-05</strong></td>
    <td><strong>Gestión de Transacciones y Operaciones de Venta</strong></td>
    <td>Como comerciante, quiero gestionar el proceso completo de registro de ventas, desde la selección de productos hasta la emisión del comprobante, para asegurar una operación ágil y sin errores.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 24 -->
  <tr>
    <td>US-24</td>
    <td>Buscar productos en el inventario y validar su tipo de medida</td>
    <td>Como cajero, quiero buscar productos del inventario para que el sistema valide si son por cantidad o peso, para abrir la interfaz de ingreso correspondiente.</td>
    <td>
      <strong>Scenario 1: Búsqueda y validación de producto por peso</strong><br>
      Dado que el cajero ingresa "Manzana" en el buscador, cuando selecciona el producto de la lista y el sistema verifica que el producto está registrado con medida en "Kg", entonces el sistema despliega el modal "Registrar Peso".<br><br>
      <strong>Scenario 2: Búsqueda y validación de producto por cantidad</strong><br>
      Dado que el cajero realiza una búsqueda, cuando selecciona "Coca Cola" del inventario y el sistema verifica que el producto está registrado por unidades, entonces el sistema despliega el modal "Registrar Cantidad".<br><br>
      <strong>Scenario 3: Producto no encontrado</strong><br>
      Dado que el término ingresado no coincide con el inventario, cuando se ejecuta la búsqueda, entonces el sistema muestra un mensaje indicando "Producto no encontrado".
    </td>
    <td>Epic-05</td>
  </tr>
  <!-- US 25 -->
  <tr>
    <td>US-25</td>
    <td>Registrar la cantidad de unidades en el Ticket de Venta</td>
    <td>Como cajero, quiero ingresar el número de unidades de un producto seleccionado, para añadirlo al detalle de la venta.</td>
    <td>
      <strong>Scenario 1: Confirmación de cantidad unitaria</strong><br>
      Dado que el modal "Registrar Cantidad" está abierto, cuando el cajero ingresa el número entero "3" en el teclado numérico y presiona el botón "Confirmar cantidad", entonces el sistema calcula el subtotal y añade el ítem al detalle de la venta.<br><br>
      <strong>Scenario 2: Validación de stock insuficiente por cantidad</strong><br>
      Dado que el cajero ha ingresado una cantidad en el modal, cuando el sistema verifica que la cantidad solicitada es mayor al stock disponible y el usuario intenta confirmar la acción, entonces el sistema muestra una alerta indicando "Stock insuficiente" y no permite añadir el producto al ticket.
    </td>
    <td>Epic-05</td>
  </tr>
  <!-- US 26 -->
  <tr>
    <td>US-26</td>
    <td>Capturar el peso mediante balanza IoT o ingreso manual</td>
    <td>Como cajero, quiero obtener el peso del producto automáticamente o por teclado para procesar la venta de productos al granel.</td>
    <td>
      <strong>Scenario 1: Captura automática</strong><br>
      Dado que el modal "Registrar Peso" está abierto, cuando el sistema detecta una balanza IoT conectada y el cajero coloca el producto sobre la balanza física y el hardware envía la lectura de peso al sistema, entonces el valor se carga automáticamente en el campo de peso.<br><br>
      <strong>Scenario 2: Registro de peso manual</strong><br>
      Dado que el sistema no detecta una balanza y el modal "Registrar Peso" está abierto, cuando el cajero digita el peso observado físicamente en el teclado decimal y presiona el botón "Confirmar Peso", entonces el sistema registra el dato y añade el producto al ticket de venta.<br><br>
      <strong>Scenario 3: Validación de stock insuficiente por peso</strong><br>
      Dado que el cajero ha ingresado el peso en el modal, cuando el sistema verifica que el peso solicitado es mayor al stock disponible y el usuario intenta confirmar la acción, entonces el sistema muestra una alerta indicando "Stock insuficiente" y no permite añadir el producto al ticket.
    </td>
    <td>Epic-05</td>
  </tr>
  <!-- US 27 -->
  <tr>
    <td>US-27</td>
    <td>Gestionar el desglose y cálculo del Ticket de Venta</td>
    <td>Como cajero, quiero visualizar el desglose de productos (nombre, cantidad/peso, precio unitario y subtotal) para verificar que la información sea correcta antes de proceder al pago.</td>
    <td>
      <strong>Scenario 1: Actualización del detalle y monto total</strong><br>
      Dado que se han añadido productos al ticket de venta, cuando el sistema procesa cada ítem de la lista y calcula automáticamente el subtotal multiplicando el precio por la cantidad o peso y suma todos los subtotales, entonces el sistema muestra el desglose detallado y el monto total acumulado de la venta en la interfaz.<br><br>
      <strong>Scenario 2: Edición o eliminación de un ítem del detalle</strong><br>
      Dado que un producto ya se encuentra registrado en el detalle de la venta, cuando el cajero selecciona la opción de eliminar y el sistema confirma la acción, entonces el sistema actualiza la lista del detalle y recalcula el monto total de la venta inmediatamente.
    </td>
    <td>Epic-05</td>
  </tr>
  <!-- US 28 -->
  <tr>
    <td>US-28</td>
    <td>Seleccionar el método de pago para la transacción</td>
    <td>Como cajero, quiero elegir el medio por el cual está pagando el cliente (Efectivo o Tarjeta/Yape/Plin), para que el ingreso se registre en la categoría contable correcta.</td>
    <td>
      <strong>Scenario 1: Selección de método de pago exitosa</strong><br>
      Dado que el ticket de venta tiene el monto total calculado, cuando el cajero hace clic sobre el ícono de "Efectivo" o "Tarjeta Yape/Plin" y el sistema marca visualmente la opción seleccionada como activa, entonces el sistema habilita el botón "Finalizar Venta y Emitir Boleta".<br><br>
      <strong>Scenario 2: Intento de finalización sin método de pago</strong><br>
      Dado que el cajero ha terminado de agregar productos al ticket, cuando intenta presionar el botón de finalizar la venta sin haber marcado una opción de pago, entonces el sistema muestra un mensaje de advertencia indicando "Por favor, seleccione un método de pago" y bloquea la emisión de la boleta.
    </td>
    <td>Epic-05</td>
  </tr>
  <!-- US 29 -->
  <tr>
    <td>US-29</td>
    <td>Finalizar la venta y emitir el comprobante de pago</td>
    <td>Como cajero, quiero procesar el pago y finalizar la venta en un solo paso, para registrar la transacción en el sistema y entregar el comprobante al cliente de forma inmediata.</td>
    <td>
      <strong>Scenario 1: Procesamiento exitoso del cierre de venta</strong><br>
      Dado que el ticket de venta tiene productos añadidos y el método de pago ha sido seleccionado, cuando el cajero presiona el botón "Finalizar Venta y Emitir Boleta" y el sistema valida que los datos de la transacción son correctos, entonces el sistema genera el comprobante de pago, muestra un mensaje de éxito y limpia la interfaz para una nueva venta.<br><br>
      <strong>Scenario 2: Bloqueo de finalización por datos incompletos</strong><br>
      Dado que el cajero se encuentra en la pantalla de ventas, cuando intenta presionar el botón de finalizar venta sin productos en el ticket o sin método de pago, entonces el sistema muestra un mensaje "No hay productos en el ticket" manteniendo la interfaz de venta activa hasta que se complete el campo requerido.
    </td>
    <td>Epic-05</td>
  </tr>
  <!-- EPIC 06 -->
  <tr>
    <td><strong>Epic-06</strong></td>
    <td><strong>Control de Ingresos y Monitoreo de Caja</strong></td>
    <td>Como dueño del negocio, quiero supervisar los flujos de dinero entrante en tiempo real, para tener visibilidad total sobre la liquidez y los métodos de pago utilizados durante el día.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 30 -->
  <tr>
    <td>US-30</td>
    <td>Clasificar automáticamente los ingresos según el medio de pago</td>
    <td>Como comerciante, quiero que cada venta finalizada sume su monto al acumulado del método correspondiente, para tener visibilidad inmediata de cuánto dinero hay en efectivo y cuánto en digital.</td>
    <td>
      <strong>Scenario 1: Actualización del acumulado por método de pago</strong><br>
      Dado que se ha finalizado una venta exitosamente, cuando el sistema procesa el registro de la transacción y detecta el método de pago utilizado (Efectivo o Tarjeta/Digital), entonces el sistema actualiza visualmente el "Resumen de Caja" con los nuevos montos acumulados.<br><br>
      <strong>Scenario 2: Visualización del total general de ingresos</strong><br>
      Dado que los saldos por categoría (Efectivo y Digital) han sido actualizados, cuando el comerciante visualiza el panel de "Resumen de Caja", entonces el sistema muestra el "Total del Día" como la suma consolidada de todos los medios de pago.
    </td>
    <td>Epic-06</td>
  </tr>
  <!-- US 31 -->
  <tr>
    <td>US-31</td>
    <td>Monitorear el Resumen de Caja en tiempo real dentro del panel de ventas</td>
    <td>Como cajero, quiero visualizar de forma centralizada los ingresos acumulados por método de pago, para tener un control inmediato de los saldos del día sin salir de la interfaz principal.</td>
    <td>
      <strong>Scenario 1: Visualización dinámica de ingresos operativos</strong><br>
      Dado que el cajero se encuentra en la sección de "Ventas", cuando finaliza transacciones de forma sucesiva, entonces el sistema actualiza automáticamente los contadores de "Efectivo", "Tarjeta Yape/Plin" y el "Total del Día" en la parte inferior de la pantalla.<br><br>
      <strong>Scenario 2: Persistencia de saldos al cambiar de sección</strong><br>
      Dado que el cajero tiene un saldo acumulado en el Resumen de Caja, cuando navega hacia otra sección y regresa nuevamente a "Ventas", entonces el sistema muestra los saldos actualizados tal como estaban antes de salir de la pestaña.
    </td>
    <td>Epic-06</td>
  </tr>
  <!-- EPIC 07 -->
  <tr>
    <td><strong>Epic-07</strong></td>
    <td><strong>Configurar Chatbot de WhatsApp Business</strong></td>
    <td>Como comerciante, quiero configurar y vincular el chatbot de WhatsApp Business desde el dashboard para activar la atención automatizada de clientes.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 32 -->
  <tr>
    <td>US-32</td>
    <td>Vincular cuenta de WhatsApp Business mediante código QR</td>
    <td>Como comerciante, quiero conectar mi cuenta de WhatsApp Business escaneando un código QR para activar el chatbot de atención a clientes desde el dashboard.</td>
    <td>
      <strong>Scenario 1: Mostrar código QR en primer acceso</strong><br>
      Dado que el comerciante no tiene ninguna cuenta vinculada, cuando accede a la sección de chatbot, entonces el sistema genera y muestra un código QR válido para iniciar la vinculación.<br><br>
      <strong>Scenario 2: Vinculación exitosa tras escaneo</strong><br>
      Dado que el comerciante escanea el código QR desde su WhatsApp Business, cuando el sistema confirma la conexión, entonces registra la vinculación, activa el chatbot y habilita la visualización de conversaciones.<br><br>
      <strong>Scenario 3: Vinculación fallida por código QR expirado</strong><br>
      Dado que el comerciante está en el proceso de vinculación de WhatsApp Business, cuando el código QR expira sin haber sido escaneado y el sistema detecta que la sesión no fue establecida en el tiempo límite, entonces el sistema descarta el código expirado, muestra un mensaje indicando que el código expiró y genera un nuevo código QR automáticamente.
    </td>
    <td>Epic-07</td>
  </tr>
  <!-- US 33 -->
  <tr>
    <td>US-33</td>
    <td>Consultar estado de vinculación del chatbot</td>
    <td>Como comerciante, quiero conocer el estado de conexión de mi WhatsApp Business para saber si el chatbot se encuentra activo o requiere reconexión.</td>
    <td>
      <strong>Scenario 1: Estado activo cuando la cuenta está vinculada</strong><br>
      Dado que el comerciante tiene una cuenta vinculada, cuando accede a la sección de chatbot, entonces el sistema muestra el estado como activo junto al número vinculado.<br><br>
      <strong>Scenario 2: Estado desconectado cuando la sesión expiró</strong><br>
      Dado que la sesión ha expirado o fue cerrada externamente, cuando el comerciante accede a la sección de chatbot, entonces el sistema muestra el estado como desconectado y habilita la opción de volver a vincular.
    </td>
    <td>Epic-07</td>
  </tr>
  <!-- EPIC 08 -->
  <tr>
    <td><strong>Epic-08</strong></td>
    <td><strong>Gestionar Conversaciones desde el Dashboard</strong></td>
    <td>Como comerciante, quiero visualizar y gestionar los chats de mis clientes directamente desde el dashboard para atenderlos sin salir de la plataforma.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 34 -->
  <tr>
    <td>US-34</td>
    <td>Visualizar conversaciones de clientes en el dashboard</td>
    <td>Como comerciante, quiero ver los chats que el bot ha tenido con mis clientes dentro del dashboard para tener visibilidad de todas las conversaciones activas sin usar WhatsApp directamente.</td>
    <td>
      <strong>Scenario 1: Conversaciones cargadas cuando existe actividad</strong><br>
      Dado que el comerciante tiene su WhatsApp Business vinculado, cuando accede a la sección de chatbot, entonces el sistema muestra la lista de conversaciones ordenada por la más reciente con el último mensaje visible.<br><br>
      <strong>Scenario 2: Mensaje informativo cuando no hay conversaciones</strong><br>
      Dado que ningún cliente ha iniciado una conversación con el bot, cuando el comerciante accede a la sección, entonces el sistema indica que aún no existen conversaciones registradas.
    </td>
    <td>Epic-08</td>
  </tr>
  <!-- US 35 -->
  <tr>
    <td>US-35</td>
    <td>Responder mensajes de clientes desde el dashboard</td>
    <td>Como comerciante, quiero enviar mensajes a mis clientes directamente desde el dashboard para gestionar conversaciones sin necesitar abrir WhatsApp.</td>
    <td>
      <strong>Scenario 1: Mensaje enviado correctamente al cliente</strong><br>
      Dado que el comerciante selecciona una conversación activa y redacta un mensaje, cuando confirma el envío, entonces el sistema envía el mensaje al cliente a través de WhatsApp y lo registra en el hilo de conversación.<br><br>
      <strong>Scenario 2: Envío bloqueado cuando el mensaje está vacío</strong><br>
      Dado que el comerciante intenta confirmar el envío sin haber redactado ningún contenido, entonces el sistema no procesa el envío y mantiene el estado de la conversación sin cambios.
    </td>
    <td>Epic-08</td>
  </tr>
  <!-- EPIC 09 -->
  <tr>
    <td><strong>Epic-09</strong></td>
    <td><strong>Procesar Pedidos mediante Bot Automático</strong></td>
    <td>Como sistema, quiero que el chatbot responda automáticamente a los clientes según el stock disponible del negocio para facilitar el proceso de pedido sin intervención manual del comerciante.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 36 -->
  <tr>
    <td>US-36</td>
    <td>Responder consulta de producto disponible</td>
    <td>Como sistema, quiero que el chatbot responda automáticamente al cliente con la información del producto solicitado cuando este existe en el inventario para iniciar el proceso de pedido sin intervención del comerciante.</td>
    <td>
      <strong>Scenario 1: Bot informa disponibilidad del producto solicitado</strong><br>
      Dado que el cliente envía el nombre de un producto y el sistema lo encuentra con stock mayor a cero, entonces el bot responde con nombre, precio y stock disponible, y ofrece al cliente agregarlo al pedido.<br><br>
      <strong>Scenario 2: Bot registra selección confirmada por el cliente</strong><br>
      Dado que el bot informó la disponibilidad y el cliente confirma la cantidad deseada, entonces el sistema registra la selección en el pedido en curso y consulta si desea agregar más productos.
    </td>
    <td>Epic-09</td>
  </tr>
  <!-- US 37 -->
  <tr>
    <td>US-37</td>
    <td>Sugerir alternativas ante producto no disponible</td>
    <td>Como sistema, quiero que el chatbot informe al cliente cuando un producto no está disponible y le sugiera otros productos del inventario para evitar que la conversación quede sin respuesta útil.</td>
    <td>
      <strong>Scenario 1: Bot sugiere alternativas cuando el producto no existe</strong><br>
      Dado que el producto solicitado no se encuentra o tiene stock igual a cero, cuando el sistema verifica la disponibilidad, entonces el bot informa que no está disponible y presenta alternativas con stock.<br><br>
      <strong>Scenario 2: Bot notifica cuando el inventario completo está agotado</strong><br>
      Dado que todos los productos tienen stock igual a cero, cuando el sistema verifica la disponibilidad general, entonces el bot informa que no hay productos disponibles e invita al cliente a intentarlo más tarde.
    </td>
    <td>Epic-09</td>
  </tr>
  <!-- US 38 -->
  <tr>
    <td>US-38</td>
    <td>Confirmar pedido con el cliente</td>
    <td>Como sistema, quiero que el chatbot presente un resumen del pedido al cliente y solicite confirmación antes de proceder al pago para asegurar que los productos y cantidades sean correctos.</td>
    <td>
      <strong>Scenario 1: Bot envía resumen y solicita confirmación</strong><br>
      Dado que el cliente indicó todos los productos y su dirección de entrega, cuando indica que no desea agregar más, entonces el sistema genera un resumen con productos, cantidades, total y dirección, y solicita confirmación.<br><br>
      <strong>Scenario 2: Sistema registra pedido tras confirmación del cliente</strong><br>
      Dado que el bot envió el resumen y el cliente confirma que el pedido es correcto, entonces el sistema registra el pedido con estado pendiente y envía las instrucciones de pago.<br><br>
      <strong>Scenario 3: Solicitar dirección de entrega al cliente</strong><br>
      Dado que el cliente confirmó los productos de su pedido, cuando el chatbot verifica que aún no se registró una dirección de entrega, entonces solicita al cliente que indique su dirección antes de continuar y no genera el resumen del pedido hasta que el cliente la proporcione.
    </td>
    <td>Epic-09</td>
  </tr>
  <!-- EPIC 10 -->
  <tr>
    <td><strong>Epic-10</strong></td>
    <td><strong>Gestionar Pago Digital P2P</strong></td>
    <td>Como cliente y comerciante, queremos gestionar el envío y la validación de comprobantes de pago digitales (Yape/Plin) a través de WhatsApp y el dashboard, para garantizar una transacción segura y confirmada antes de finalizar la venta.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 39 -->
  <tr>
    <td>US-39</td>
    <td>Recibir instrucciones de pago por WhatsApp</td>
    <td>Como cliente, quiero recibir las instrucciones de pago a través del chatbot para saber cómo realizar la transferencia y completar mi pedido.</td>
    <td>
      <strong>Scenario 1: Bot envía instrucciones tras confirmación del pedido</strong><br>
      Dado que el cliente confirmó su pedido y el stock fue validado, cuando el sistema procesa la confirmación, entonces el bot envía el número Yape/Plin del comerciante, el monto total y el número de pedido como referencia.<br><br>
      <strong>Scenario 2: Sistema registra el evento de instrucción enviada</strong><br>
      Dado que el bot entrega las instrucciones de pago, cuando el sistema confirma la entrega del mensaje, entonces registra el evento con marca de tiempo para trazabilidad.
    </td>
    <td>Epic-10</td>
  </tr>
  <!-- US 40 -->
  <tr>
    <td>US-40</td>
    <td>Reportar comprobante de pago digital</td>
    <td>Como cliente, quiero enviar el comprobante de mi pago al chatbot para que el comerciante pueda verificarlo y confirmar mi pedido.</td>
    <td>
      <strong>Scenario 1: Sistema registra comprobante recibido y notifica al comerciante</strong><br>
      Dado que el cliente realizó el pago por Yape o Plin, cuando envía el comprobante al chatbot, entonces el sistema lo registra, actualiza el estado del pedido a pendiente de validación y notifica al comerciante.<br><br>
      <strong>Scenario 2: Bot envía recordatorio ante ausencia de reporte</strong><br>
      Dado que el cliente recibió las instrucciones de pago, cuando transcurren treinta minutos sin que reporte el comprobante, entonces el sistema envía un recordatorio y mantiene el pedido en estado esperando pago.
    </td>
    <td>Epic-10</td>
  </tr>
  <!-- US 41 -->
  <tr>
    <td>US-41</td>
    <td>Validar comprobante de pago desde el dashboard</td>
    <td>Como comerciante, quiero revisar el comprobante reportado por el cliente y aprobarlo o rechazarlo desde el dashboard para confirmar que el dinero fue recibido correctamente.</td>
    <td>
      <strong>Scenario 1: Comerciante visualiza comprobante y detalles del pedido</strong><br>
      Dado que el cliente reportó su comprobante, cuando el comerciante revisa el pedido, entonces el sistema muestra el comprobante, el monto y los detalles del pedido asociado.<br><br>
      <strong>Scenario 2: Sistema registra validación manual al aprobar el pago</strong><br>
      Dado que el comerciante verifica que el comprobante es correcto, cuando aprueba el pago, entonces el sistema registra la validación con marca de tiempo y continúa el flujo de confirmación.<br><br>
      <strong>Scenario 3: Sistema notifica al cliente al rechazar el pago</strong><br>
      Dado que el comerciante detecta que el comprobante es incorrecto, cuando lo rechaza indicando el motivo, entonces el sistema registra el rechazo y el bot notifica al cliente con los pasos a seguir.
    </td>
    <td>Epic-10</td>
  </tr>
  <!-- US 42 -->
  <tr>
    <td>US-42</td>
    <td>Notificar resultado de validación al cliente</td>
    <td>Como cliente, quiero recibir una notificación sobre el resultado de la validación de mi pago para saber si mi pedido fue confirmado o si debo realizar alguna acción adicional.</td>
    <td>
      <strong>Scenario 1: Bot confirma al cliente que el pago fue aprobado</strong><br>
      Dado que el comerciante aprueba el comprobante, cuando el sistema actualiza el estado del pedido, entonces el bot envía al cliente un mensaje confirmando que el pago fue recibido y el pedido está en proceso.<br><br>
      <strong>Scenario 2: Bot informa al cliente que el pago fue rechazado</strong><br>
      Dado que el comerciante rechaza el comprobante, cuando el sistema actualiza el estado, entonces el bot informa al cliente que el pago no fue validado, indica el motivo y solicita que reintente.
    </td>
    <td>Epic-10</td>
  </tr>
  <!-- EPIC 11 -->
  <tr>
    <td><strong>Epic-11</strong></td>
    <td><strong>Confirmar Venta y Emitir Comprobante</strong></td>
    <td>Como dueño de negocio, quiero que el sistema confirme el pedido tras la validación del pago, descuente el stock y emita un comprobante digital, para mantener el control financiero y brindar un respaldo de la compra al cliente.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 43 -->
  <tr>
    <td>US-43</td>
    <td>Confirmar pedido y descontar stock</td>
    <td>Como sistema, quiero confirmar el pedido automáticamente al aprobar el pago para actualizar el inventario en tiempo real y reflejar el consumo de stock.</td>
    <td>
      <strong>Scenario 1: Sistema actualiza inventario al confirmar el pedido</strong><br>
      Dado que el comerciante aprueba el comprobante de pago, cuando el sistema confirma el pedido, entonces actualiza el estado a confirmado y descuenta la cantidad correspondiente del stock de cada producto.<br><br>
      <strong>Scenario 2: Sistema sincroniza peso con balanza IoT para productos por peso</strong><br>
      Dado que el pedido incluye productos vendidos por peso, cuando el sistema descuenta el stock, entonces actualiza el peso disponible registrado en la balanza IoT.
    </td>
    <td>Epic-11</td>
  </tr>
  <!-- US 44 -->
  <tr>
    <td>US-44</td>
    <td>Registrar venta en el sistema</td>
    <td>Como comerciante, quiero que cada pedido confirmado quede registrado como venta en el sistema para mantener un control financiero preciso y trazable.</td>
    <td>
      <strong>Scenario 1: Sistema crea registro de venta al confirmar pedido</strong><br>
      Dado que el pedido ha sido confirmado tras la validación del pago, cuando el sistema procesa el cierre de la transacción, entonces crea un registro de venta con monto total, método de pago, productos vendidos y marca de tiempo.<br><br>
      <strong>Scenario 2: Sistema separa ingresos digitales de los ingresos en efectivo</strong><br>
      Dado que el método de pago fue Yape o Plin, cuando el sistema registra la venta, entonces asocia el monto al canal de pagos digitales, manteniéndolo separado del efectivo en caja.
    </td>
    <td>Epic-11</td>
  </tr>
  <!-- US 45 -->
  <tr>
    <td>US-45</td>
    <td>Emitir comprobante digital al cliente</td>
    <td>Como cliente, quiero recibir un comprobante de mi compra a través del chatbot para tener un respaldo de la transacción realizada.</td>
    <td>
      <strong>Scenario 1: Bot envía comprobante al cliente tras registrar la venta</strong><br>
      Dado que la venta ha sido registrada correctamente, cuando el sistema genera el comprobante, entonces el bot envía al cliente un resumen con número de pedido, productos, cantidades, monto total y fecha.<br><br>
      <strong>Scenario 2: Sistema marca el pedido como completado al emitir el comprobante</strong><br>
      Dado que el comprobante fue generado y enviado, cuando el sistema confirma la entrega, entonces registra el evento con marca de tiempo y actualiza el estado del pedido a completado.
    </td>
    <td>Epic-11</td>
  </tr>
  <!-- EPIC 12 -->
  <tr>
    <td><strong>Epic-12</strong></td>
    <td><strong>Manejar Flujos Alternativos y Restricciones</strong></td>
    <td>Como sistema de gestión, quiero manejar escenarios de excepción como falta de stock, tiempos de espera agotados y rechazos de pago, para proteger la integridad del inventario y evitar pérdidas económicas.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 46 -->
  <tr>
    <td>US-46</td>
    <td>Manejar stock insuficiente en pedido</td>
    <td>Como cliente, quiero ser notificado cuando un producto no tiene stock suficiente para ajustar mi pedido antes de proceder al pago.</td>
    <td>
      <strong>Scenario 1: Bot notifica al cliente sobre stock insuficiente</strong><br>
      Dado que el cliente solicita una cantidad mayor al stock disponible, cuando el sistema valida el inventario, entonces el bot informa qué producto no tiene stock suficiente y ofrece ajustar la cantidad o eliminarlo del pedido.<br><br>
      <strong>Scenario 2: Sistema actualiza el pedido con la nueva cantidad</strong><br>
      Dado que el bot informó al cliente sobre el stock insuficiente, cuando el cliente confirma una nueva cantidad menor o igual al stock disponible, entonces el sistema actualiza el pedido y continúa el flujo de forma normal.
    </td>
    <td>Epic-12</td>
  </tr>
  <!-- US 47 -->
  <tr>
    <td>US-47</td>
    <td>Cancelar pedido por expiración de tiempo de pago</td>
    <td>Como sistema, quiero cancelar automáticamente un pedido cuando el cliente no reporta el comprobante de pago en el tiempo establecido para liberar el stock reservado.</td>
    <td>
      <strong>Scenario 1: Sistema cancela el pedido y libera el stock al expirar el tiempo</strong><br>
      Dado que el cliente recibió las instrucciones de pago, cuando transcurren sesenta minutos sin que reporte el comprobante, entonces el sistema cancela el pedido, libera el stock reservado y notifica al cliente.<br><br>
      <strong>Scenario 2: Sistema registra el evento de cancelación para trazabilidad</strong><br>
      Dado que el pedido es cancelado por expiración, cuando el sistema actualiza el estado, entonces registra el evento de cancelación con el motivo y marca de tiempo correspondientes.
    </td>
    <td>Epic-12</td>
  </tr>
  <!-- US 48 -->
  <tr>
    <td>US-48</td>
    <td>Rechazar comprobante de pago inválido</td>
    <td>Como comerciante, quiero rechazar un comprobante de pago cuando sea incorrecto o sospechoso para proteger el negocio de transacciones fraudulentas.</td>
    <td>
      <strong>Scenario 1: Sistema revierte el estado del pedido al rechazar el comprobante</strong><br>
      Dado que el comerciante identifica un comprobante sospechoso o incorrecto, cuando lo rechaza indicando el motivo, entonces el sistema devuelve el pedido al estado "esperando pago" y el bot notifica al cliente.<br><br>
      <strong>Scenario 2: Sistema alerta al comerciante ante rechazos repetidos del mismo cliente</strong><br>
      Dado que el mismo cliente presenta comprobantes rechazados en dos ocasiones consecutivas, cuando el sistema detecta el patrón, entonces alerta al comerciante y bloquea el pedido para revisión manual.
    </td>
    <td>Epic-12</td>
  </tr>
  <!-- EPIC 13 -->
  <tr>
    <td><strong>Epic-13</strong></td>
    <td><strong>Technical Stories – Implementar RESTful API</strong></td>
    <td>Como equipo de desarrollo, queremos implementar una arquitectura de servicios RESTful segura y escalable para que todos los componentes de la plataforma intercambien datos de manera consistente.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 49 -->
  <tr>
    <td>US-49</td>
    <td>Conocer propuesta de valor en landing page</td>
    <td>Como visitante, quiero entender qué hace Entreprenly y cómo puede beneficiar a mi negocio para decidir si me interesa adquirirlo.</td>
    <td>
      <strong>Scenario 1: Visitante visualiza la propuesta de valor al cargar la página</strong><br>
      Dado que el visitante accede a la landing page, cuando la página termina de cargar, entonces el sistema muestra el headline principal, la propuesta de valor y los beneficios clave del producto.<br><br>
      <strong>Scenario 2: Visitante accede a la sección de funcionalidades</strong><br>
      Dado que el visitante navega por la landing page, cuando llega a la sección de funcionalidades, entonces el sistema presenta las características principales: chatbot WhatsApp, inventario, balanza IoT y dashboard financiero.
    </td>
    <td>Epic-13</td>
  </tr>
  <!-- US 50 -->
  <tr>
    <td>US-50</td>
    <td>Gestionar ciclo de vida de pedidos mediante API</td>
    <td>Como developer, quiero endpoints para crear y actualizar pedidos para que el chatbot y el dashboard intercambien información del pedido de forma automática y consistente.</td>
    <td>
      <strong>Scenario 1: Creación exitosa de pedido</strong><br>
      Dado que el developer envía una solicitud de creación con datos válidos, cuando el servidor valida el cuerpo, entonces el sistema responde con HTTP 201, retorna el ID del pedido, el estado pendiente y la marca de tiempo.<br><br>
      <strong>Scenario 2: Actualización de estado de pedido existente</strong><br>
      Dado que el developer envía una solicitud de actualización con estado válido, cuando el servidor procesa la solicitud, entonces el sistema responde con HTTP 200 y retorna el objeto del pedido actualizado.<br><br>
      <strong>Scenario 3: Solicitud sobre pedido inexistente</strong><br>
      Dado que el developer referencia un ID de pedido que no existe, cuando el servidor busca el recurso, entonces el sistema responde con HTTP 404 indicando que el pedido no fue encontrado.
    </td>
    <td>Epic-13</td>
  </tr>
  <!-- US 51 -->
  <tr>
    <td>US-51</td>
    <td>Validar y registrar pagos mediante API</td>
    <td>Como developer, quiero un endpoint para aprobar o rechazar pagos desde el dashboard para que el sistema actualice el inventario y notifique al cliente de forma automática.</td>
    <td>
      <strong>Scenario 1: Aprobación de pago con descuento de stock</strong><br>
      Dado que el developer envía una solicitud de aprobación con estado aprobado, cuando el servidor procesa la validación, entonces el sistema responde con HTTP 200, actualiza el pedido a confirmado y descuenta el stock correspondiente.<br><br>
      <strong>Scenario 2: Rechazo de pago con registro de motivo</strong><br>
      Dado que el developer envía una solicitud de rechazo con motivo especificado, cuando el servidor procesa el rechazo, entonces el sistema responde con HTTP 200 y registra el motivo en el historial del pago.<br><br>
      <strong>Scenario 3: Solicitud sobre pago inexistente</strong><br>
      Dado que el developer referencia un ID de pago que no existe, cuando el servidor busca el recurso, entonces el sistema responde con HTTP 404 indicando que el pago no fue encontrado.
    </td>
    <td>Epic-13</td>
  </tr>
  <!-- EPIC 14 -->
  <tr>
    <td><strong>Epic-14</strong></td>
    <td><strong>Inicio de sesión y registro</strong></td>
    <td>Como usuario quiero registrarme, verificar mi cuenta, iniciar sesión y recuperar mi contraseña para acceder de forma segura a la plataforma.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 52 -->
  <tr>
    <td>US-52</td>
    <td>Registrar cuenta con email</td>
    <td>Como usuario anónimo, quiero registrarme con mi email y contraseña para crear una cuenta en Entreprenly y obtener automáticamente el Plan Free.</td>
    <td>
      <strong>Scenario 1: Registro exitoso</strong><br>
      Dado que el usuario ingresa un email no registrado y una contraseña válida, cuando envía el formulario, entonces el sistema crea la cuenta, asigna automáticamente el Plan Free, envía un email de verificación y muestra un mensaje de confirmación.<br><br>
      <strong>Scenario 2: Email ya registrado</strong><br>
      Dado que el usuario ingresa un email que ya existe, cuando envía el formulario, entonces el sistema muestra un mensaje de error indicando que el email ya está en uso.<br><br>
      <strong>Scenario 3: Datos inválidos</strong><br>
      Dado que la contraseña no cumple los requisitos mínimos, cuando envía el formulario, entonces el sistema muestra los errores de validación sin crear la cuenta.
    </td>
    <td>Epic-14</td>
  </tr>
  <!-- US 53 -->
  <tr>
    <td>US-53</td>
    <td>Verificar email</td>
    <td>Como usuario registrado, quiero verificar mi email mediante el enlace enviado a mi correo para activar mi cuenta.</td>
    <td>
      <strong>Scenario 1: Verificación exitosa</strong><br>
      Dado que el usuario hace clic en el enlace de verificación válido, cuando el sistema valida el token, entonces la cuenta queda activa y el usuario es redirigido al dashboard principal.<br><br>
      <strong>Scenario 2: Token expirado</strong><br>
      Dado que el token ha expirado, cuando el sistema intenta validarlo, entonces muestra un mensaje de error y ofrece la opción de reenviar el email de verificación.<br><br>
      <strong>Scenario 3: Token inválido</strong><br>
      Dado que el token está malformado, cuando el sistema intenta procesarlo, entonces muestra un mensaje de error indicando que el enlace no es válido.
    </td>
    <td>Epic-14</td>
  </tr>
  <!-- US 54 -->
  <tr>
    <td>US-54</td>
    <td>Iniciar sesión con credenciales</td>
    <td>Como usuario registrado, quiero iniciar sesión con mi email y contraseña para acceder al dashboard de Entreprenly.</td>
    <td>
      <strong>Scenario 1: Inicio de sesión exitoso</strong><br>
      Dado que el usuario ingresa credenciales válidas, cuando envía el formulario, entonces el sistema genera un JWT, inicia la sesión y redirige al dashboard principal.<br><br>
      <strong>Scenario 2: Credenciales inválidas</strong><br>
      Dado que el usuario ingresa una contraseña incorrecta, cuando envía el formulario, entonces el sistema muestra un mensaje de error sin revelar cuál campo es incorrecto.<br><br>
      <strong>Scenario 3: Cuenta bloqueada por intentos fallidos</strong><br>
      Dado que el usuario ha fallado 5 intentos consecutivos, cuando intenta iniciar sesión nuevamente, entonces el sistema bloquea la cuenta y notifica al usuario por email.
    </td>
    <td>Epic-14</td>
  </tr>
  <!-- US 55 -->
  <tr>
    <td>US-55</td>
    <td>Iniciar sesión con Google OAuth</td>
    <td>Como usuario anónimo, quiero iniciar sesión con mi cuenta de Google para acceder a Entreprenly sin necesidad de crear credenciales nuevas.</td>
    <td>
      <strong>Scenario 1: OAuth exitoso con cuenta nueva</strong><br>
      Dado que el usuario inicia el flujo OAuth con una cuenta de Google no registrada previamente, cuando Google autoriza el acceso, entonces el sistema crea una nueva cuenta vinculada al proveedor e inicia la sesión.<br><br>
      <strong>Scenario 2: OAuth exitoso con cuenta existente</strong><br>
      Dado que el usuario inicia el flujo OAuth con un email ya registrado, cuando Google devuelve el token, entonces el sistema vincula el proveedor a la cuenta existente e inicia la sesión.<br><br>
      <strong>Scenario 3: OAuth denegado por el usuario</strong><br>
      Dado que el usuario cancela la autorización en la pantalla de Google, cuando el flujo es interrumpido, entonces el sistema redirige al usuario a la pantalla de login sin crear ninguna cuenta.
    </td>
    <td>Epic-14</td>
  </tr>
  <!-- US 56 -->
  <tr>
    <td>US-56</td>
    <td>Recuperar contraseña</td>
    <td>Como usuario registrado, quiero recuperar el acceso a mi cuenta mediante un enlace enviado a mi email para restablecer mi contraseña.</td>
    <td>
      <strong>Scenario 1: Reset exitoso</strong><br>
      Dado que el usuario solicita el reset con un email registrado y confirma la nueva contraseña desde el enlace recibido, cuando el sistema procesa la solicitud, entonces actualiza la contraseña, invalida todas las sesiones anteriores y redirige al login.<br><br>
      <strong>Scenario 2: Token de reset expirado</strong><br>
      Dado que el usuario accede al enlace después de que el token ha expirado, cuando el sistema intenta validarlo, entonces muestra un mensaje de error y solicita generar un nuevo enlace.<br><br>
      <strong>Scenario 3: Email no registrado</strong><br>
      Dado que el usuario solicita el reset con un email que no existe, cuando envía el formulario, entonces el sistema responde con un mensaje genérico sin confirmar ni negar la existencia del email.
    </td>
    <td>Epic-14</td>
  </tr>
  <!-- US 57 -->
  <tr>
    <td>US-57</td>
    <td>Cerrar sesión</td>
    <td>Como usuario autenticado, quiero cerrar mi sesión para que el sistema revoque mi token y me redirija a la pantalla de login.</td>
    <td>
      <strong>Scenario 1: Cierre de sesión exitoso</strong><br>
      Dado que el usuario hace clic en la opción de cerrar sesión, cuando el sistema procesa la solicitud, entonces revoca el JWT activo y redirige al usuario a la pantalla de login.<br><br>
      <strong>Scenario 2: Intento de acceso tras cerrar sesión</strong><br>
      Dado que el usuario ha cerrado su sesión y el token ha sido revocado, cuando intenta acceder a una ruta protegida, entonces el sistema rechaza la solicitud y redirige al login.
    </td>
    <td>Epic-14</td>
  </tr>
  <!-- EPIC 15 -->
  <tr>
    <td><strong>Epic-15</strong></td>
    <td><strong>Perfil y configuración</strong></td>
    <td>Como usuario quiero gestionar mi perfil y preferencias personales para personalizar mi experiencia dentro de la plataforma.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 58 -->
  <tr>
    <td>US-58</td>
    <td>Visualizar perfil actual</td>
    <td>Como usuario autenticado, quiero visualizar mi perfil actual para revisar mis datos registrados en la plataforma.</td>
    <td>
      <strong>Scenario 1: Visualización exitosa</strong><br>
      Dado que el usuario navega a la sección de perfil, cuando el sistema carga los datos, entonces muestra nombre, bio, foto de perfil, email y preferencias actuales del usuario.<br><br>
      <strong>Scenario 2: Sesión expirada</strong><br>
      Dado que la sesión del usuario ha expirado, cuando intenta acceder a la sección de perfil, entonces el sistema redirige al login.
    </td>
    <td>Epic-15</td>
  </tr>
  <!-- US 59 -->
  <tr>
    <td>US-59</td>
    <td>Actualizar nombre y biografía</td>
    <td>Como usuario autenticado, quiero actualizar mi nombre y biografía para mantener mi perfil al día.</td>
    <td>
      <strong>Scenario 1: Actualización exitosa</strong><br>
      Dado que el usuario edita su nombre y/o bio con datos válidos, cuando guarda los cambios, entonces el sistema actualiza los datos y muestra el perfil con la información nueva.<br><br>
      <strong>Scenario 2: Campo obligatorio vacío</strong><br>
      Dado que el usuario deja el campo de nombre vacío, cuando intenta guardar, entonces el sistema muestra un error de validación sin guardar los cambios.
    </td>
    <td>Epic-15</td>
  </tr>
  <!-- US 60 -->
  <tr>
    <td>US-60</td>
    <td>Subir foto de perfil</td>
    <td>Como usuario autenticado, quiero subir una foto de perfil para personalizar mi cuenta en la plataforma.</td>
    <td>
      <strong>Scenario 1: Subida exitosa</strong><br>
      Dado que el usuario selecciona una imagen con formato y tamaño permitidos, cuando la sube al sistema, entonces el servicio de almacenamiento guarda el archivo, actualiza la URL del avatar y muestra la nueva foto en el perfil.<br><br>
      <strong>Scenario 2: Formato de imagen no permitido</strong><br>
      Dado que el usuario intenta subir un archivo con formato no soportado, cuando el sistema valida el archivo, entonces muestra un mensaje de error indicando los formatos aceptados sin guardar el archivo.<br><br>
      <strong>Scenario 3: Tamaño de archivo excedido</strong><br>
      Dado que el usuario intenta subir una imagen que supera el tamaño máximo (5120 KB), cuando el sistema valida el archivo, entonces muestra un mensaje de error indicando el límite de tamaño.
    </td>
    <td>Epic-15</td>
  </tr>
  <!-- US 61 -->
  <tr>
    <td>US-61</td>
    <td>Cambiar email con re-verificación</td>
    <td>Como usuario autenticado, quiero cambiar mi email y verificarlo para mantener mis datos de contacto actualizados.</td>
    <td>
      <strong>Scenario 1: Cambio de email exitoso</strong><br>
      Dado que el usuario solicita cambiar su email a uno no registrado previamente y confirma desde el enlace enviado, entonces el sistema actualiza el email y lo marca como verificado.<br><br>
      <strong>Scenario 2: Nuevo email ya en uso</strong><br>
      Dado que el usuario ingresa un email que ya pertenece a otra cuenta, cuando intenta guardar el cambio, entonces el sistema muestra un mensaje de error sin actualizar el email.<br><br>
      <strong>Scenario 3: Confirmación desde enlace expirado</strong><br>
      Dado que el usuario hace clic en el enlace de confirmación después de que ha expirado, cuando el sistema valida el token, entonces muestra un mensaje de error y ofrece reenviar el email de confirmación.
    </td>
    <td>Epic-15</td>
  </tr>
  <!-- US 62 -->
  <tr>
    <td>US-62</td>
    <td>Cambiar contraseña</td>
    <td>Como usuario autenticado, quiero cambiar mi contraseña para mantener la seguridad de mi cuenta.</td>
    <td>
      <strong>Scenario 1: Cambio exitoso</strong><br>
      Dado que el usuario ingresa su contraseña actual correcta y una nueva contraseña válida, cuando guarda el cambio, entonces el sistema actualiza la contraseña e invalida todas las sesiones activas excepto la actual.<br><br>
      <strong>Scenario 2: Contraseña actual incorrecta</strong><br>
      Dado que el usuario ingresa una contraseña actual incorrecta, cuando intenta guardar, entonces el sistema muestra un error de validación sin actualizar la contraseña.<br><br>
      <strong>Scenario 3: Nueva contraseña no cumple requisitos</strong><br>
      Dado que el usuario ingresa una nueva contraseña que no cumple los requisitos mínimos, cuando intenta guardar, entonces el sistema muestra los requisitos incumplidos sin aplicar el cambio.
    </td>
    <td>Epic-15</td>
  </tr>
  <!-- US 63 -->
  <tr>
    <td>US-63</td>
    <td>Configurar preferencias de idioma, zona horaria y tema</td>
    <td>Como usuario autenticado, quiero configurar mi idioma, zona horaria y tema visual para adaptar la plataforma a mis preferencias.</td>
    <td>
      <strong>Scenario 1: Cambio de idioma exitoso</strong><br>
      Dado que el usuario selecciona un idioma disponible, cuando guarda la preferencia, entonces el sistema actualiza el idioma de la interfaz de forma inmediata.<br><br>
      <strong>Scenario 2: Cambio de zona horaria exitoso</strong><br>
      Dado que el usuario selecciona una zona horaria de la lista disponible, cuando guarda la preferencia, entonces el sistema la almacena y la aplica en las fechas mostradas.<br><br>
      <strong>Scenario 3: Cambio de tema exitoso</strong><br>
      Dado que el usuario selecciona el tema claro u oscuro, cuando guarda la preferencia, entonces el sistema aplica el tema de forma inmediata y lo persiste para futuras sesiones.
    </td>
    <td>Epic-15</td>
  </tr>
  <!-- US 64 -->
  <tr>
    <td>US-64</td>
    <td>Configurar notificaciones</td>
    <td>Como usuario autenticado, quiero configurar mis preferencias de notificación para recibir solo los avisos que me sean relevantes.</td>
    <td>
      <strong>Scenario 1: Guardado exitoso de preferencias</strong><br>
      Dado que el usuario activa o desactiva tipos de notificación disponibles, cuando guarda los cambios, entonces el sistema almacena las preferencias y las aplica en los envíos futuros.<br><br>
      <strong>Scenario 2: Sin cambios realizados</strong><br>
      Dado que el usuario accede a la sección de notificaciones sin modificar nada, cuando sale de la sección, entonces el sistema mantiene las preferencias anteriores sin alteración.
    </td>
    <td>Epic-15</td>
  </tr>
  <!-- EPIC 16 -->
  <tr>
    <td><strong>Epic-16</strong></td>
    <td><strong>Panel de Inicio (Home)</strong></td>
    <td>Como comerciante, quiero contar con un panel de inicio centralizado que me muestre un resumen visual del estado de mi negocio al ingresar a la plataforma, para tomar decisiones rápidas sin necesidad de navegar entre módulos.</td>
    <td></td>
    <td></td>
  </tr>
  <!-- US 65 -->
  <tr>
    <td>US-65</td>
    <td>Visualizar resumen de ventas del día</td>
    <td>Como comerciante, quiero visualizar un resumen de las ventas del día en el panel de inicio para conocer el rendimiento de mi negocio sin ingresar al módulo de ventas.</td>
    <td>
      <strong>Scenario 1: Resumen de ventas cargado correctamente</strong><br>
      Dado que el comerciante accede al panel de inicio y existen ventas registradas en el día, cuando el sistema carga la información, entonces se muestra el total de ventas del día, el número de transacciones y el desglose por método de pago.<br><br>
      <strong>Scenario 2: Sin ventas registradas en el día</strong><br>
      Dado que el comerciante accede al panel de inicio y no se ha registrado ninguna venta en el día actual, cuando el sistema carga la información, entonces el resumen muestra cero en todos los indicadores y se indica que aún no hay ventas registradas para el día.
    </td>
    <td>Epic-16</td>
  </tr>
  <!-- US 66 -->
  <tr>
    <td>US-66</td>
    <td>Visualizar estado del chatbot en el home</td>
    <td>Como comerciante, quiero visualizar el estado de conexión del chatbot y los chats activos desde el panel de inicio para saber si mi canal de ventas por WhatsApp está operativo sin ingresar al módulo de chatbot.</td>
    <td>
      <strong>Scenario 1: Chatbot conectado con actividad reciente</strong><br>
      Dado que el comerciante accede al panel de inicio y el chatbot se encuentra vinculado y activo, cuando el sistema carga la vista, entonces se muestra el estado "Conectado", el número de conversaciones activas del día y el número de pedidos generados por el bot.<br><br>
      <strong>Scenario 2: Chatbot desconectado</strong><br>
      Dado que el comerciante accede al panel de inicio y el chatbot no está vinculado o su sesión expiró, cuando el sistema carga la vista, entonces se muestra el estado "Desconectado" con una alerta visible y un acceso directo para reconectar desde el mismo panel.
    </td>
    <td>Epic-16</td>
  </tr>
  <!-- US 67 -->
  <tr>
    <td>US-67</td>
    <td>Visualizar alertas de inventario en el home</td>
    <td>Como comerciante, quiero ver las alertas críticas de inventario directamente en el panel de inicio para identificar rápidamente productos agotados o lotes próximos a vencer sin ingresar al módulo de lotes.</td>
    <td>
      <strong>Scenario 1: Alertas de inventario mostradas en el home</strong><br>
      Dado que el comerciante accede al panel de inicio y existen productos sin stock o lotes próximos a vencer, cuando el sistema carga la vista, entonces se muestra una sección de alertas con el nombre del producto o lote afectado y el tipo de alerta correspondiente.<br><br>
      <strong>Scenario 2: Sin alertas activas de inventario</strong><br>
      Dado que el comerciante accede al panel de inicio y no existen condiciones críticas en el inventario, cuando el sistema carga la vista, entonces la sección de alertas muestra un mensaje indicando que todo el inventario está en estado normal.
    </td>
    <td>Epic-16</td>
  </tr>
  <!-- US 68 -->
  <tr>
    <td>US-68</td>
    <td>Visualizar contador de pedidos pendientes en el home</td>
    <td>Como comerciante, quiero ver el número de pedidos que están pendientes de atención en el panel de inicio para priorizar mi respuesta sin necesidad de ingresar al módulo de chatbot.</td>
    <td>
      <strong>Scenario 1: Pedidos pendientes mostrados correctamente</strong><br>
      Dado que el comerciante accede al panel de inicio y existen pedidos en estado "pendiente de validación" o "esperando pago", cuando el sistema carga la vista, entonces se muestra un contador con el número total de pedidos que requieren atención inmediata del comerciante.<br><br>
      <strong>Scenario 2: Sin pedidos pendientes</strong><br>
      Dado que el comerciante accede al panel de inicio y todos los pedidos del día han sido atendidos o no existe ninguno, cuando el sistema carga la vista, entonces el contador muestra cero y se indica que no hay pedidos pendientes de atención.
    </td>
    <td>Epic-16</td>
  </tr>
  <!-- US 69 -->
  <tr>
    <td>US-69</td>
    <td>Visualizar pedidos recientes en el home</td>
    <td>Como comerciante, quiero ver los pedidos más recientes con su estado actual en el panel de inicio para hacer seguimiento sin ingresar al módulo de pedidos.</td>
    <td>
      <strong>Scenario 1: Pedidos recientes mostrados correctamente</strong><br>
      Dado que el comerciante accede al panel de inicio y existen pedidos registrados en el día, cuando el sistema carga la vista, entonces se muestran los últimos cinco pedidos con número de pedido, nombre del cliente, monto total y estado actual.<br><br>
      <strong>Scenario 2: Sin pedidos registrados en el día</strong><br>
      Dado que el comerciante accede al panel de inicio y no se ha registrado ningún pedido en el día actual, cuando el sistema carga la vista, entonces la sección de pedidos recientes muestra un mensaje indicando que aún no hay pedidos para el día.
    </td>
    <td>Epic-16</td>
  </tr>
  <!-- US 70 -->
  <tr>
    <td>US-70</td>
    <td>Acceder a módulos desde accesos directos del home</td>
    <td>Como comerciante, quiero contar con accesos directos a los módulos principales desde el panel de inicio para navegar rápidamente a cualquier sección sin recorrer el menú lateral.</td>
    <td>
      <strong>Scenario 1: Acceso directo navega al módulo correcto</strong><br>
      Dado que el comerciante se encuentra en el panel de inicio, cuando presiona alguno de los accesos directos disponibles, entonces el sistema lo redirige al módulo correspondiente sin pérdida de datos ni recargas innecesarias.<br><br>
      <strong>Scenario 2: Acceso directo con indicador de alerta activa</strong><br>
      Dado que el comerciante se encuentra en el panel de inicio y un módulo tiene alertas o notificaciones pendientes, cuando el sistema carga la vista, entonces el acceso directo correspondiente muestra un indicador visual con el número de alertas o pendientes activos.
    </td>
    <td>Epic-16</td>
  </tr>
  <!-- Epic 17 -->
  <tr>
    <td><strong>Epic-17</strong></td>
    <td><strong>Centro de Soporte y Ayuda</strong></td>
    <td>Como comerciante, quiero contar con un centro de soporte accesible desde el botón de Ayuda para resolver mis dudas, reportar problemas y consultar guías de uso de la plataforma sin necesidad de contactar a un agente externo.</td>
    <td></td>
  </tr>

  <!-- US 69 -->
  <tr>
    <td>US-74</td>
    <td>Visualizar el centro de soporte</td>
    <td>Como comerciante, quiero visualizar el centro de soporte al presionar el botón de Ayuda para acceder de forma rápida a las opciones de asistencia disponibles.</td>
    <td>
      <strong>Scenario 1: Centro de soporte cargado correctamente</strong><br>
      Dado que el comerciante presiona el botón de Ayuda en el sidebar,<br>
      Cuando el sistema carga la vista de soporte,<br>
      Entonces se muestran las secciones: buscador de ayuda, artículos frecuentes, acceso directo a reportar problema y datos de contacto del soporte.<br><br>
      <strong>Scenario 2: Centro de soporte sin artículos disponibles</strong><br>
      Dado que el comerciante accede al centro de soporte,<br>
      Y no existen artículos de ayuda configurados,<br>
      Cuando el sistema carga la vista,<br>
      Entonces se muestra un mensaje indicando que el contenido de ayuda no está disponible aún<br>
      Y se mantiene visible la opción de reportar un problema.
    </td>
    <td>Epic-17</td>
  </tr>

  <!-- US 70 -->
  <tr>
    <td>US-75</td>
    <td>Buscar artículo de ayuda</td>
    <td>Como comerciante, quiero buscar artículos de ayuda por palabras clave para encontrar rápidamente la información que necesito sin revisar todas las categorías.</td>
    <td>
      <strong>Scenario 1: Búsqueda con resultados encontrados</strong><br>
      Dado que el comerciante está en el centro de soporte,<br>
      Cuando ingresa una palabra clave en el buscador y confirma la búsqueda,<br>
      Entonces el sistema muestra los artículos que coinciden con el término ingresado.<br><br>
      <strong>Scenario 2: Búsqueda sin resultados</strong><br>
      Dado que el comerciante ingresa un término en el buscador,<br>
      Y no existen artículos que coincidan con la búsqueda,<br>
      Cuando el sistema procesa la consulta,<br>
      Entonces se muestra un mensaje indicando que no se encontraron resultados<br>
      Y se sugiere reformular la búsqueda o reportar el problema directamente.
    </td>
    <td>Epic-17</td>
  </tr>

  <!-- US 71 -->
  <tr>
    <td>US-76</td>
    <td>Consultar artículo de ayuda</td>
    <td>Como comerciante, quiero abrir y leer un artículo de ayuda para entender cómo usar una funcionalidad de la plataforma o resolver un problema específico.</td>
    <td>
      <strong>Scenario 1: Artículo cargado correctamente</strong><br>
      Dado que el comerciante selecciona un artículo desde el listado o los resultados de búsqueda,<br>
      Cuando el sistema carga el artículo,<br>
      Entonces se muestra el título, el contenido detallado y las secciones relacionadas.<br><br>
      <strong>Scenario 2: Artículo marcado como útil o no útil</strong><br>
      Dado que el comerciante leyó el artículo de ayuda,<br>
      Cuando selecciona la opción "¿Te fue útil este artículo?"<br>
      Y elige "Sí" o "No",<br>
      Entonces el sistema registra la respuesta<br>
      Y si elige "No", muestra la opción de reportar el problema directamente.
    </td>
    <td>Epic-17</td>
  </tr>

  <!-- US 72 -->
  <tr>
    <td>US-77</td>
    <td>Reportar un problema</td>
    <td>Como comerciante, quiero reportar un problema o incidencia desde el centro de soporte para que el equipo de Entreprenly pueda revisarlo y darle seguimiento.</td>
    <td>
      <strong>Scenario 1: Reporte enviado correctamente</strong><br>
      Dado que el comerciante está en el formulario de reporte de problema,<br>
      Y completa los campos obligatorios: categoría, descripción y módulo afectado,<br>
      Cuando presiona el botón "Enviar reporte",<br>
      Entonces el sistema registra el reporte<br>
      Y muestra una confirmación indicando que fue recibido.<br><br>
      <strong>Scenario 2: Intento de envío con campos incompletos</strong><br>
      Dado que el comerciante está en el formulario de reporte,<br>
      Y deja campos obligatorios vacíos,<br>
      Cuando presiona el botón "Enviar reporte",<br>
      Entonces el sistema no registra el reporte<br>
      Y muestra mensajes de error indicando los campos que deben completarse.
    </td>
    <td>Epic-17</td>
  </tr>

  <!-- US 73 -->
  <tr>
    <td>US-78</td>
    <td>Confirmar envío del reporte</td>
    <td>Como comerciante, quiero recibir una confirmación visual tras enviar un reporte para tener la certeza de que mi solicitud fue registrada correctamente.</td>
    <td>
      <strong>Scenario 1: Confirmación mostrada correctamente</strong><br>
      Dado que el comerciante envió un reporte de problema exitosamente,<br>
      Cuando el sistema procesa el envío,<br>
      Entonces se muestra una pantalla de confirmación con el número de ticket generado, el mensaje "Tu reporte fue recibido" y la opción de volver al centro de soporte.<br><br>
      <strong>Scenario 2: Error en el envío del reporte</strong><br>
      Dado que el comerciante intentó enviar un reporte,<br>
      Y ocurre un error en el sistema durante el procesamiento,<br>
      Cuando el sistema detecta el fallo,<br>
      Entonces no se genera el ticket<br>
      Y se muestra un mensaje indicando que hubo un error y se invita a intentarlo nuevamente.
    </td>
    <td>Epic-17</td>
  </tr>
  </tbody>
</table>

## 3.2. Impact Mapping

El Impact Mapping es una técnica de planificación estratégica que permite vincular los objetivos de negocio con las funcionalidades del producto, respondiendo las preguntas: ¿por qué construimos esto?, ¿quién nos ayuda a lograrlo?, ¿cómo cambia su comportamiento? y ¿qué entregamos para provocar ese cambio? Su elaboración permite asegurar que cada User Story tenga un propósito claro y directo sobre el objetivo del negocio.A continuación se presenta el Impact Map elaborado en UXPressia para Entreprenly:

![Impact Mapping](./images/Impact_Mapping.png "Impact Mapping")

El Impact Map parte de un único objetivo de negocio: permitir que el pequeño comerciante gestione su negocio de forma eficiente, reduzca pérdidas de inventario y automatice la atención de pedidos sin depender de procesos manuales. Se identificó al Comerciante como único actor, dado que es el usuario directo de la plataforma y el único cuyo comportamiento debe cambiar para que el objetivo se cumpla.
A partir de este actor se derivaron cinco impactos esperados: que deje de gestionar su inventario manualmente, que reaccione a tiempo ante problemas de stock, que registre sus ventas presenciales de forma rápida y ordenada, que delegue la atención de pedidos por WhatsApp al chatbot, y que tome decisiones con información centralizada desde el panel de inicio. Cada uno de estos impactos se traduce en entregables concretos que corresponden a las funcionalidades de la plataforma, las cuales están sustentadas por las User Stories especificadas en la sección 3.1.

## 3.3. Product Backlog

A continuación se presenta el Product Backlog de Entreprenly con todas las User Stories priorizadas según su valor para el negocio. Las User Stories de mayor impacto directo en la operación del comerciante y en la propuesta de valor central del producto se ubican en las primeras posiciones. Las historias relacionadas con autenticación, suscripción y perfil, si bien necesarias, se ubican en posiciones posteriores por tratarse de funcionalidades de soporte.

<table>
  <thead>
    <tr>
      <th># Orden</th>
      <th>User Story Id</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Story Points</th>
    </tr>
  </thead>
  <tbody>
    <!-- BLOQUE 1: LANDING -->
    <tr><td>1</td><td>US-49</td><td>Conocer propuesta de valor en landing page</td><td>Como visitante, quiero entender qué hace Entreprenly y cómo puede beneficiar a mi negocio para decidir si me interesa adquirirlo.</td><td>3</td></tr>
    <!-- BLOQUE 2: AUTENTICACIÓN -->
    <tr><td>2</td><td>US-52</td><td>Registrar cuenta con email</td><td>Como usuario anónimo, quiero registrarme con mi email y contraseña para crear una cuenta en Entreprenly y obtener automáticamente el Plan Free.</td><td>3</td></tr>
    <tr><td>3</td><td>US-53</td><td>Verificar email</td><td>Como usuario registrado, quiero verificar mi email mediante el enlace enviado a mi correo para activar mi cuenta.</td><td>3</td></tr>
    <tr><td>4</td><td>US-54</td><td>Iniciar sesión con credenciales</td><td>Como usuario registrado, quiero iniciar sesión con mi email y contraseña para acceder al dashboard de Entreprenly.</td><td>3</td></tr>
    <tr><td>5</td><td>US-55</td><td>Iniciar sesión con Google OAuth</td><td>Como usuario anónimo, quiero iniciar sesión con mi cuenta de Google para acceder a Entreprenly sin necesidad de crear credenciales nuevas.</td><td>5</td></tr>
    <tr><td>6</td><td>US-56</td><td>Recuperar contraseña</td><td>Como usuario registrado, quiero recuperar el acceso a mi cuenta mediante un enlace enviado a mi email para restablecer mi contraseña.</td><td>3</td></tr>
    <tr><td>7</td><td>US-57</td><td>Cerrar sesión</td><td>Como usuario autenticado, quiero cerrar mi sesión para que el sistema revoque mi token y me redirija a la pantalla de login.</td><td>1</td></tr>
    <!-- BLOQUE 3: GESTIÓN DE INVENTARIO -->
    <tr><td>8</td><td>US-01</td><td>Agregar productos</td><td>Como usuario quiero agregar productos para gestionar mi inventario de manera eficiente.</td><td>3</td></tr>
    <tr><td>9</td><td>US-05</td><td>Editar productos</td><td>Como usuario quiero editar productos para actualizar los datos en el inventario.</td><td>2</td></tr>
    <tr><td>10</td><td>US-10</td><td>Visualizar detalles de producto</td><td>Como usuario quiero visualizar la información detallada de cada producto en el listado para conocer rápidamente sus características, stock disponible y precio sin necesidad de ingresar a otra pantalla.</td><td>2</td></tr>
    <tr><td>11</td><td>US-12</td><td>Buscar productos</td><td>Como usuario quiero tener un buscador de productos para perder menos tiempo buscando en el inventario.</td><td>3</td></tr>
    <tr><td>12</td><td>US-23</td><td>Crear lotes</td><td>Como usuario quiero crear lotes de productos para controlar mejor el stock y la caducidad en el inventario.</td><td>3</td></tr>
    <tr><td>13</td><td>US-03</td><td>Agregar lotes</td><td>Como usuario quiero agregar lotes para gestionar correctamente las cantidades y fechas de vencimiento.</td><td>2</td></tr>
    <tr><td>14</td><td>US-02</td><td>Editar lotes</td><td>Como usuario quiero editar los lotes para actualizar los datos del inventario.</td><td>2</td></tr>
    <tr><td>15</td><td>US-06</td><td>Visualizar detalles de lotes</td><td>Como usuario quiero visualizar los detalles de los lotes para gestionar mejor el inventario.</td><td>2</td></tr>
    <tr><td>16</td><td>US-04</td><td>Eliminar lotes</td><td>Como usuario quiero eliminar lotes para deshacerme de los lotes que no me sirvan.</td><td>1</td></tr>
    <!-- BLOQUE 4: ALERTAS DE INVENTARIO -->
    <tr><td>17</td><td>US-09</td><td>Visualizar dashboard de lotes</td><td>Como usuario quiero visualizar un dashboard de lotes con indicadores y alertas para conocer rápidamente el estado de mi inventario al ingresar al módulo de lotes.</td><td>3</td></tr>
    <tr><td>18</td><td>US-07</td><td>Detectar stock agotado</td><td>Como usuario quiero ser notificado cuando tengo bajo/nada de stock.</td><td>3</td></tr>
    <tr><td>19</td><td>US-11</td><td>Recibir alerta de caducidad de lote</td><td>Como usuario quiero ser notificado cuando un lote esté próximo a vencer o ya haya vencido para tomar acciones como priorizar su uso o descartarlo.</td><td>3</td></tr>
    <tr><td>20</td><td>US-08</td><td>Mostrar alertas de estado al visualizar detalles</td><td>Como usuario quiero visualizar alertas de estado al ver el detalle de un lote para identificar rápidamente si tiene stock bajo, está agotado o próximo a vencer.</td><td>2</td></tr>
    <!-- BLOQUE 5: VENTAS PRESENCIALES (POS) -->
    <tr><td>21</td><td>US-24</td><td>Buscar productos en el inventario y validar su tipo de medida</td><td>Como cajero, quiero buscar productos del inventario para que el sistema valide si son por cantidad o peso, para abrir la interfaz de ingreso correspondiente.</td><td>3</td></tr>
    <tr><td>22</td><td>US-25</td><td>Registrar la cantidad de unidades en el Ticket de Venta</td><td>Como cajero, quiero ingresar el número de unidades de un producto seleccionado, para añadirlo al detalle de la venta.</td><td>2</td></tr>
    <tr><td>23</td><td>US-26</td><td>Capturar el peso mediante balanza IoT o ingreso manual</td><td>Como cajero, quiero obtener el peso del producto automáticamente o por teclado para procesar la venta de productos al granel.</td><td>5</td></tr>
    <tr><td>24</td><td>US-27</td><td>Gestionar el desglose y cálculo del Ticket de Venta</td><td>Como cajero, quiero visualizar el desglose de productos para verificar que la información sea correcta antes de proceder al pago.</td><td>3</td></tr>
    <tr><td>25</td><td>US-28</td><td>Seleccionar el método de pago para la transacción</td><td>Como cajero, quiero elegir el medio por el cual está pagando el cliente para que el ingreso se registre en la categoría contable correcta.</td><td>2</td></tr>
    <tr><td>26</td><td>US-29</td><td>Finalizar la venta y emitir el comprobante de pago</td><td>Como cajero, quiero procesar el pago y finalizar la venta en un solo paso para registrar la transacción en el sistema y entregar el comprobante al cliente de forma inmediata.</td><td>3</td></tr>
    <!-- BLOQUE 6: CONTROL DE CAJA -->
    <tr><td>27</td><td>US-30</td><td>Clasificar automáticamente los ingresos según el medio de pago</td><td>Como comerciante, quiero que cada venta finalizada sume su monto al acumulado del método correspondiente para tener visibilidad inmediata del efectivo y digital.</td><td>3</td></tr>
    <tr><td>28</td><td>US-31</td><td>Monitorear el Resumen de Caja en tiempo real dentro del panel de ventas</td><td>Como cajero, quiero visualizar de forma centralizada los ingresos acumulados por método de pago para tener un control inmediato de los saldos del día sin salir de la interfaz principal.</td><td>2</td></tr>
    <!-- BLOQUE 7: PANEL DE INICIO (HOME) -->
    <tr><td>29</td><td>US-65</td><td>Visualizar resumen de ventas del día</td><td>Como comerciante, quiero visualizar un resumen de las ventas del día en el panel de inicio para conocer el rendimiento de mi negocio sin ingresar al módulo de ventas.</td><td>2</td></tr>
    <tr><td>30</td><td>US-67</td><td>Visualizar alertas de inventario en el home</td><td>Como comerciante, quiero ver las alertas críticas de inventario directamente en el panel de inicio para identificar rápidamente productos agotados o lotes próximos a vencer.</td><td>2</td></tr>
    <tr><td>31</td><td>US-68</td><td>Visualizar contador de pedidos pendientes en el home</td><td>Como comerciante, quiero ver el número de pedidos que están pendientes de atención en el panel de inicio para priorizar mi respuesta sin necesidad de ingresar al módulo de chatbot.</td><td>1</td></tr>
    <tr><td>32</td><td>US-69</td><td>Visualizar pedidos recientes en el home</td><td>Como comerciante, quiero ver los pedidos más recientes con su estado actual en el panel de inicio para hacer seguimiento sin ingresar al módulo de pedidos.</td><td>2</td></tr>
    <tr><td>33</td><td>US-66</td><td>Visualizar estado del chatbot en el home</td><td>Como comerciante, quiero visualizar el estado de conexión del chatbot y los chats activos desde el panel de inicio para saber si mi canal de ventas por WhatsApp está operativo.</td><td>2</td></tr>
    <tr><td>34</td><td>US-70</td><td>Acceder a módulos desde accesos directos del home</td><td>Como comerciante, quiero contar con accesos directos a los módulos principales desde el panel de inicio para navegar rápidamente a cualquier sección sin recorrer el menú lateral.</td><td>1</td></tr>
    <!-- BLOQUE 8: CHATBOT WHATSAPP -->
    <tr><td>35</td><td>US-32</td><td>Vincular cuenta de WhatsApp Business mediante código QR</td><td>Como comerciante, quiero conectar mi cuenta de WhatsApp Business escaneando un código QR para activar el chatbot de atención a clientes desde el dashboard.</td><td>5</td></tr>
    <tr><td>36</td><td>US-33</td><td>Consultar estado de vinculación del chatbot</td><td>Como comerciante, quiero conocer el estado de conexión de mi WhatsApp Business para saber si el chatbot se encuentra activo o requiere reconexión.</td><td>2</td></tr>
    <tr><td>37</td><td>US-34</td><td>Visualizar conversaciones de clientes en el dashboard</td><td>Como comerciante, quiero ver los chats que el bot ha tenido con mis clientes dentro del dashboard para tener visibilidad de todas las conversaciones activas sin usar WhatsApp directamente.</td><td>3</td></tr>
    <tr><td>38</td><td>US-35</td><td>Responder mensajes de clientes desde el dashboard</td><td>Como comerciante, quiero enviar mensajes a mis clientes directamente desde el dashboard para gestionar conversaciones sin necesitar abrir WhatsApp.</td><td>3</td></tr>
    <!-- BLOQUE 9: FLUJO DE PEDIDOS POR BOT -->
    <tr><td>39</td><td>US-36</td><td>Responder consulta de producto disponible</td><td>Como sistema, quiero que el chatbot responda automáticamente al cliente con la información del producto solicitado cuando este existe en el inventario.</td><td>3</td></tr>
    <tr><td>40</td><td>US-37</td><td>Sugerir alternativas ante producto no disponible</td><td>Como sistema, quiero que el chatbot informe al cliente cuando un producto no está disponible y le sugiera otros productos del inventario.</td><td>2</td></tr>
    <tr><td>41</td><td>US-38</td><td>Confirmar pedido con el cliente</td><td>Como sistema, quiero que el chatbot presente un resumen del pedido al cliente y solicite confirmación antes de proceder al pago.</td><td>3</td></tr>
    <tr><td>42</td><td>US-39</td><td>Recibir instrucciones de pago por WhatsApp</td><td>Como cliente, quiero recibir las instrucciones de pago a través del chatbot para saber cómo realizar la transferencia y completar mi pedido.</td><td>2</td></tr>
    <tr><td>43</td><td>US-40</td><td>Reportar comprobante de pago digital</td><td>Como cliente, quiero enviar el comprobante de mi pago al chatbot para que el comerciante pueda verificarlo y confirmar mi pedido.</td><td>3</td></tr>
    <tr><td>44</td><td>US-41</td><td>Validar comprobante de pago desde el dashboard</td><td>Como comerciante, quiero revisar el comprobante reportado por el cliente y aprobarlo o rechazarlo desde el dashboard.</td><td>3</td></tr>
    <tr><td>45</td><td>US-42</td><td>Notificar resultado de validación al cliente</td><td>Como cliente, quiero recibir una notificación sobre el resultado de la validación de mi pago para saber si mi pedido fue confirmado.</td><td>2</td></tr>
    <!-- BLOQUE 10: CONFIRMACIÓN Y CIERRE DE PEDIDOS -->
    <tr><td>46</td><td>US-43</td><td>Confirmar pedido y descontar stock</td><td>Como sistema, quiero confirmar el pedido automáticamente al aprobar el pago para actualizar el inventario en tiempo real y reflejar el consumo de stock.</td><td>3</td></tr>
    <tr><td>47</td><td>US-44</td><td>Registrar venta en el sistema</td><td>Como comerciante, quiero que cada pedido confirmado quede registrado como venta en el sistema para mantener un control financiero preciso y trazable.</td><td>2</td></tr>
    <tr><td>48</td><td>US-45</td><td>Emitir comprobante digital al cliente</td><td>Como cliente, quiero recibir un comprobante de mi compra a través del chatbot para tener un respaldo de la transacción realizada.</td><td>3</td></tr>
    <!-- BLOQUE 11: FLUJOS ALTERNATIVOS Y RESTRICCIONES -->
    <tr><td>49</td><td>US-46</td><td>Manejar stock insuficiente en pedido</td><td>Como cliente, quiero ser notificado cuando un producto no tiene stock suficiente para ajustar mi pedido antes de proceder al pago.</td><td>3</td></tr>
    <tr><td>50</td><td>US-47</td><td>Cancelar pedido por expiración de tiempo de pago</td><td>Como sistema, quiero cancelar automáticamente un pedido cuando el cliente no reporta el comprobante de pago en el tiempo establecido para liberar el stock reservado.</td><td>3</td></tr>
    <tr><td>51</td><td>US-48</td><td>Rechazar comprobante de pago inválido</td><td>Como comerciante, quiero rechazar un comprobante de pago cuando sea incorrecto o sospechoso para proteger el negocio de transacciones fraudulentas.</td><td>3</td></tr>
    <!-- BLOQUE 12: API TÉCNICA -->
    <tr><td>52</td><td>US-50</td><td>Gestionar ciclo de vida de pedidos mediante API</td><td>Como developer, quiero endpoints para crear y actualizar pedidos para que el chatbot y el dashboard intercambien información del pedido de forma automática y consistente.</td><td>5</td></tr>
    <tr><td>53</td><td>US-51</td><td>Validar y registrar pagos mediante API</td><td>Como developer, quiero un endpoint para aprobar o rechazar pagos desde el dashboard para que el sistema actualice el inventario y notifique al cliente de forma automática.</td><td>5</td></tr>
    <!-- BLOQUE 13: SUSCRIPCIÓN -->
    <tr><td>54</td><td>US-13</td><td>Seleccionar plan de suscripción</td><td>Como usuario con Plan Free, quiero presionar el botón "Elegir plan" en la tarjeta del Plan Control para definir el plan que deseo contratar y continuar con el proceso de suscripción.</td><td>2</td></tr>
    <tr><td>55</td><td>US-14</td><td>Iniciar proceso de suscripción</td><td>Como usuario con un plan seleccionado, quiero presionar el botón "Continuar con la suscripción" para abrir el formulario de facturación y comenzar formalmente la contratación del plan elegido.</td><td>2</td></tr>
    <tr><td>56</td><td>US-71</td><td>Agregar método de pago de suscripción</td><td>Como usuario con acceso al panel "Suscripción", quiero presionar el botón "Agregar método de pago" para registrar un medio de cobro que pueda usarse en pagos y renovaciones del Plan Control.</td><td>3</td></tr>
    <tr><td>57</td><td>US-72</td><td>Completar datos fiscales de suscripción</td><td>Como usuario con una cuenta registrada, quiero presionar el botón "Completar datos" para registrar mi RUC o DNI, razón social o nombre, dirección fiscal y correo de facturación.</td><td>2</td></tr>
    <tr><td>58</td><td>US-15</td><td>Registrar datos de facturación</td><td>Como usuario, quiero completar el formulario de facturación y presionar el botón "Continuar al pago" para que el sistema pueda preparar el cobro correspondiente a la suscripción.</td><td>3</td></tr>
    <tr><td>59</td><td>US-16</td><td>Procesar cobro de suscripción</td><td>Como usuario, quiero revisar el resumen de cobro y presionar el botón "Pagar y activar suscripción" para validar el pago del Plan Control seleccionado.</td><td>5</td></tr>
    <tr><td>60</td><td>US-17</td><td>Activar suscripción</td><td>Como usuario, quiero que al confirmarse el pago el sistema active automáticamente el Plan Control y me redirija al panel de suscripción para acceder a las funcionalidades premium.</td><td>3</td></tr>
    <tr><td>61</td><td>US-18</td><td>Visualizar panel de suscripción</td><td>Como usuario, quiero hacer clic en la opción lateral "Suscripción" para ver un panel con el plan actual, estado, fecha de renovación, facturación y acciones disponibles.</td><td>2</td></tr>
    <tr><td>62</td><td>US-19</td><td>Consultar estado de suscripción</td><td>Como usuario, quiero ver una etiqueta de estado en el panel de suscripción para saber si mi plan se encuentra en estado "Activa", "Cancelación programada", "Cancelada" o "Plan Free".</td><td>1</td></tr>
    <tr><td>63</td><td>US-20</td><td>Renovar suscripción</td><td>Como usuario con una suscripción de pago activa o próxima a vencer, quiero presionar el botón "Renovar suscripción" para extender la vigencia de mi acceso a la plataforma.</td><td>3</td></tr>
    <tr><td>64</td><td>US-21</td><td>Solicitar cancelación de suscripción</td><td>Como usuario con una suscripción de pago activa, quiero presionar el botón "Solicitar cancelación" y luego "Confirmar cancelación" para detener la renovación automática al finalizar el periodo vigente.</td><td>2</td></tr>
    <tr><td>65</td><td>US-22</td><td>Cancelar suscripción</td><td>Como sistema, quiero cancelar la suscripción de pago al finalizar su periodo vigente para retirar el acceso premium y devolver la cuenta del usuario al Plan Free.</td><td>3</td></tr>
    <tr><td>66</td><td>US-73</td><td>Descargar historial de suscripción</td><td>Como usuario, quiero presionar el botón "Descargar historial" para obtener un archivo con los eventos de mi plan, pagos, renovaciones, cambios y cancelaciones.</td><td>2</td></tr>
    <!-- BLOQUE 14: SOPORTE Y AYUDA (NUEVO) -->
    <tr><td>67</td><td>US-74</td><td>Visualizar el centro de soporte</td><td>Como comerciante, quiero visualizar el centro de soporte al presionar el botón de Ayuda para acceder de forma rápida a las opciones de asistencia disponibles.</td><td>2</td></tr>
    <tr><td>68</td><td>US-75</td><td>Buscar artículo de ayuda</td><td>Como comerciante, quiero buscar artículos de ayuda por palabras clave para encontrar rápidamente la información que necesito sin revisar todas las categorías.</td><td>2</td></tr>
    <tr><td>69</td><td>US-76</td><td>Consultar artículo de ayuda</td><td>Como comerciante, quiero abrir y leer un artículo de ayuda para entender cómo usar una funcionalidad de la plataforma o resolver un problema específico.</td><td>2</td></tr>
    <tr><td>70</td><td>US-77</td><td>Reportar un problema</td><td>Como comerciante, quiero reportar un problema o incidencia desde el centro de soporte para que el equipo de Entreprenly pueda revisarlo y darle seguimiento.</td><td>3</td></tr>
    <tr><td>71</td><td>US-78</td><td>Confirmar envío del reporte</td><td>Como comerciante, quiero recibir una confirmación visual tras enviar un reporte para tener la certeza de que mi solicitud fue registrada correctamente.</td><td>1</td></tr>
    <!-- BLOQUE 15: PERFIL Y CONFIGURACIÓN -->
    <tr><td>72</td><td>US-58</td><td>Visualizar perfil actual</td><td>Como usuario autenticado, quiero visualizar mi perfil actual para revisar mis datos registrados en la plataforma.</td><td>1</td></tr>
    <tr><td>73</td><td>US-59</td><td>Actualizar nombre y biografía</td><td>Como usuario autenticado, quiero actualizar mi nombre y biografía para mantener mi perfil al día.</td><td>2</td></tr>
    <tr><td>74</td><td>US-60</td><td>Subir foto de perfil</td><td>Como usuario autenticado, quiero subir una foto de perfil para personalizar mi cuenta en la plataforma.</td><td>3</td></tr>
    <tr><td>75</td><td>US-61</td><td>Cambiar email con re-verificación</td><td>Como usuario autenticado, quiero cambiar mi email y verificarlo para mantener mis datos de contacto actualizados.</td><td>3</td></tr>
    <tr><td>76</td><td>US-62</td><td>Cambiar contraseña</td><td>Como usuario autenticado, quiero cambiar mi contraseña para mantener la seguridad de mi cuenta.</td><td>3</td></tr>
    <tr><td>77</td><td>US-63</td><td>Configurar preferencias de idioma, zona horaria y tema</td><td>Como usuario autenticado, quiero configurar mi idioma, zona horaria y tema visual para adaptar la plataforma a mis preferencias.</td><td>2</td></tr>
    <tr><td>78</td><td>US-64</td><td>Configurar notificaciones</td><td>Como usuario autenticado, quiero configurar mis preferencias de notificación para recibir solo los avisos que me sean relevantes.</td><td>2</td></tr>
  </tbody>
</table>