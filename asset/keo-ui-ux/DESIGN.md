# Dirección de diseño · KEO Barber

## Identidad y jerarquía

Conservar negro y dorado: fondo cercano a #111210, superficies #20221F, texto principal #F5F3EB, secundario #BFC2B9 y acento #D8BB7A. Son valores propuestos para implementación, no colores medidos de los PNG. Usar texto oscuro sobre controles dorados. Reservar verde para estados completados y acompañarlo de texto o icono.

Un encabezado claro por pantalla, una acción principal y grupos separados por espacio. Mantener el orden Cita → Servicios → Horarios → Tus datos. El éxito es un estado posterior y retira el indicador de pasos. No añadir especialidades, slogans ni promesas sin fuente.

## Composición

- PC: profesional/calendario/horas en tres zonas; catálogo y horarios con resumen lateral; resumen sobre formulario; itinerario y confirmación en dos zonas.
- Smartphone: columna única, contenido desplazable y acciones fáciles de localizar. Apilar profesional, fecha y rango horario bajo el servicio; dejar el precio a la derecha. Permitir crecer en altura en lugar de reducir texto para encajar una captura.
- Mantener al menos 16 px CSS para texto de contenido móvil y áreas táctiles de 44 × 44 px. Comprobar nombres largos, zoom y pantallas estrechas.
- Verificar contraste mínimo 4.5:1 para texto normal y 3:1 para texto grande. Proporcionar foco visible y estados seleccionado, deshabilitado, cargando, vacío y error.

## Reglas funcionales para implementación futura

- Reconsultar disponibilidad al cambiar profesional, fecha, duración o cantidad. Explicar si una selección deja de estar disponible y ofrecer alternativas.
- No permitir horarios superpuestos para la misma persona ni doble asignación del mismo profesional. Las citas simultáneas del ejemplo pertenecen a personas diferentes.
- Los profesionales de servicios adicionales en pantalla 2 son ilustrativos: mostrar “Profesional pendiente” hasta la elección en pantalla 3.
- Mantener totales derivados de los servicios seleccionados. Los precios de referencia son literalmente 10, 4 y 7 CLP, total 21 CLP; no convertirlos a miles.
- Validar los campos con errores inline que indiquen problema y solución; conservar entradas y mover el foco al primer error al enviar. “Recordar mis datos” debe ser opcional y desmarcado inicialmente.
- Evitar envíos duplicados al confirmar; mostrar carga y permitir recuperación ante fallo. Confirmar éxito solo tras registrar la reserva y no afirmar envío de correo sin respaldo del sistema.
- “Para otra persona”, “Agregar al calendario” y “Gestionar reserva” son propuestas. Definir asistentes, exportación del calendario y acceso a gestión antes de desarrollar esos controles.

## Alcance

Los PNG comunican intención visual. No sustituyen especificaciones de componentes, pruebas de accesibilidad ni validación de negocio. Este trabajo no construye la aplicación. Consultar `ANALISIS-UX.md` para cobertura y `prompts-final.json` para metadata final.
