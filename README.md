# MediCita — Gestión inteligente de citas médicas

## Sección A: Evidencia de Campo (Discovery)

### El Problema
Los usuarios pierden horas esperando citas médicas por sistemas colapsados, largas filas
y falta de avisos oportunos. El proceso es manual, ineficiente y frustrante.

### Resultados de la Sonda
**Enlace al formulario:** [Encuesta de optimización de procesos](https://forms.cloud.       microsoft/Pages/AnalysisPage.aspx?AnalyzerToken=lAXUkvAyX3JuS1A5GFwxckBKYJNZK5TK&   id=-4HJLoOSoEOaOTMy_FTXdHj6TixbYD1CkDiEX2NI1RBUOVBERzBLNDNXREVUUVVQNlRFVlZRRlJNWC4u)

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

  ## Evidencia de Entrevistas Presenciales

Se realizaron 4 entrevistas físicas como parte del proceso de discovery.
Las grabaciones reposan como evidencia del trabajo de campo realizado.

**Hallazgos clave de las entrevistas:**
- Los entrevistados coinciden en que el mayor problema es la espera sin información.
- Ninguno conoce una app local que gestione citas médicas con notificaciones.
- Todos expresaron disposición a usar una solución digital si fuera simple y rápida.

---

## Evidencia de Entrevistas Presenciales

Se realizaron 4 entrevistas físicas como parte del proceso de discovery.
**Evidencia de audio de las entrevistas:**

[Ver grabaciones en Google Drive](https://drive.google.com/drive/folders/1pFsCxftz5-J2OteGXfft7Yqhxqz8hXEk?usp=drive_link)

| # | Entrevistado | Área | Frecuencia | Dolor Principal |
|---|---|---|---|---|
| 1 | José Maya | Coordinación | Todo el tiempo | No logra coordinar horarios con su grupo universitario |
| 2 | Samuel González | Salud y Bienestar | Ocasional | Esperó 2 horas por falla en el sistema al validar su cita |
| 3 | Juan Diego | Trámites y Burocracia | Siempre | Esperó 6 horas para sacar la cédula y nunca hubo sistema |
| 4 | Juan Daniel | Trámites y Burocracia | Muy seguido | Gastó 4 horas intentando pagar la matrícula por errores del portal |

**Frases más impactantes:**

> *"Esperé tres horas, me dijeron que no había sistema, esperé otras tres y tampoco. Me fui habiendo perdido seis horas para nada."* — Juan Diego

> *"Por más de llegar temprano e intentar adelantar el proceso, fue imposible. Dependíamos de que se solucionara el problema."* — Samuel González

> *"Hoy me gasté cuatro horas intentando realizar un pago y siempre hay trabas para todos los trámites."* — Juan Daniel

**Conclusión del campo:**
El 75% de los entrevistados presenciales sufre problemas con sistemas digitales
lentos, caídos o mal diseñados, tanto en salud como en trámites administrativos.
La solución soñada en común es: autogestión digital sin depender de intervención
humana ni filas físicas.