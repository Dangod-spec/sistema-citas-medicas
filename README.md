# 🏥 MediCita — Gestión Inteligente de Citas Médicas

## Sección A: Evidencia de Campo (Discovery)

### El Problema
Los usuarios pierden horas esperando citas médicas por sistemas colapsados, largas filas
y falta de avisos oportunos. El proceso es manual, ineficiente y frustrante.

### Resultados de la Sonda
**Enlace al formulario:** [Encuesta de optimización de procesos](https://forms.cloud.microsoft/r/D7rXT0U1rL)

**Resumen de datos obtenidos (19 respuestas):**
- El **37% de los encuestados** identifica Salud y Bienestar como su área de mayor pérdida de tiempo.
- El **32%** señaló Trámites y Burocracia como problema frecuente.
- La **frecuencia promedio del problema es 3.9/5**, lo que indica que ocurre de forma
  semanal o casi diaria.
- Respuesta más impactante (Encuestado #12):
  > "Más de dos días llamando para una cita, nadie me atendió. Me tocó dirigirme
  > a un punto de atención y hacer fila."

---

## Sección B: Definición de Requisitos (Definition)

### Historia de Usuario Principal

> **Como** paciente que necesita atención médica, **quiero** agendar y gestionar mis
> citas médicas desde una app, **para** evitar filas, llamadas sin respuesta y recibir
> un aviso antes de mi turno.

---

### Criterios de Aceptación

1. El sistema debe enviar una notificación al celular del usuario con al menos
   15 minutos de anticipación antes de su cita.
2. El sistema debe mostrar en tiempo real el estado de la cita (Pendiente,
   Confirmada, En curso, Cancelada).
3. El sistema debe funcionar en dispositivos móviles (diseño responsive).
4. El tiempo de carga de la agenda de citas no debe superar los 2 segundos.
5. El usuario debe recibir una confirmación por correo electrónico al agendar
   o cancelar una cita.

---

### Requisitos Funcionales

- **RF-01 (Autenticación):** El sistema debe permitir el registro e inicio de sesión
  de usuarios mediante correo electrónico y contraseña, validando credenciales
  contra una base de datos segura.

- **RF-02 (Agendamiento):** El sistema debe registrar, actualizar y cancelar citas
  médicas, almacenando fecha, hora, especialidad y estado en la base de datos.

- **RF-03 (Notificaciones):** El sistema debe notificar al usuario mediante
  alertas push y correo electrónico cuando su cita esté próxima, sea confirmada
  o sea cancelada.

- **RF-04 (Gestión de disponibilidad):** El sistema debe consultar y mostrar
  los horarios disponibles de los médicos, actualizándose en tiempo real para
  evitar doble agendamiento.

- **RF-05 (Historial):** El sistema debe mostrar al usuario el historial de sus
  citas anteriores y permitir filtrarlas por fecha y especialidad.