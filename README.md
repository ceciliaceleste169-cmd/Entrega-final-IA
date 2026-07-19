# Trabajo Final: Sistema Inteligente de Clasificación de Leads con IA y Control Humano

## 🚀 Enlaces Obligatorios de la Entrega
* **Base de Datos (Google Sheets):** [👉 HAZ CLIC AQUÍ PARA VER LA PLANILLA EN MODO LECTURA](TU_ENLACE_DE_COMPARTIR_GOOGLE_SHEETS_AQUÍ) *(Asegúrate de que cualquier persona con el enlace pueda leerlo)*
* **Lógica del Flujo (.json):** El archivo técnico de n8n se encuentra adjunto en la raíz de este repositorio como `flujo_clasificacion_leads.json`.
* **Diagrama de Arquitectura (PDF):** El documento explicativo formal se encuentra adjunto como `Diagrama_y_Especificacion_de_Arquitectura.pdf`.

---

## 📸 Evidencias del Flujo (Screenshots)
A continuación, se presentan las capturas de pantalla que demuestran el correcto funcionamiento del ecosistema automatizado de extremo a extremo:

### 1. Vista General del Flujo en n8n
Muestra la arquitectura completa con sus dos caminos (Clasificación e Ingesta / Validación Humana y Despacho).
![Flujo Completo](./capturas-evidencia/01-flujo-completo.png)

### 2. Configuración del Nodo de IA (Prompt Engineering)
Evidencia de las instrucciones y variables dinámicas utilizadas para categorizar los leads en VIP/Regular.
![Nodo IA](./capturas-evidencia/02-nodo-ia-prompt.png)

### 3. Mecanismo Human-in-the-Loop (Alerta Recibida)
Captura del correo de alerta interna enviado al operador para frenar el "efecto metralleta" y esperar aprobación.
![Alerta Humana](./capturas-evidencia/03-alerta-humana-recibida.png)

### 4. Persistencia de Datos y Mapeo de Hilos (Thread ID)
Evidencia de la planilla de Google Sheets con el `thread_id` guardado con éxito tras el envío de la propuesta final.
![Persistencia Sheets](./capturas-evidencia/04-sheets-thread-id-guardado.png)

---

## 🛠️ Tecnologías Utilizadas
* **n8n:** Orquestador central del flujo y control de estados.
* **Google Sheets:** Base de persistencia e integridad de datos.
* **Gemini / OpenAI API:** Motor cognitivo para análisis y justificación de leads.
* **Gmail:** Interfaz multicanal para alertas de control y comunicación con clientes.
