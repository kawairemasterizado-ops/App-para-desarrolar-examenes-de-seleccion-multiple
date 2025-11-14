Exámenes Asistente IA (Gemini-Powered Exam Helper)
Un asistente de escritorio avanzado diseñado para ayudar a responder preguntas de cuestionarios en pantalla mediante la captura de regiones específicas de la pantalla (ROI) y el análisis de la imagen con el modelo de IA Gemini de Google. Ideal para simulacros de examen o situaciones donde se necesita una referencia rápida y discreta.

Este proyecto ha sido desarrollado en Python utilizando tkinter para la interfaz gráfica, mss para la captura de pantalla y la API de Google Generative AI para el análisis de imágenes.

✨ Características Principales
Análisis Rápido por IA: Utiliza modelos de Gemini (como gemini-2.5-flash) para analizar imágenes de preguntas y devolver la respuesta correcta (ej. "A", "C, D") en segundos.

Superposición (Overlay) Discreta: Muestra la respuesta de la IA en una ventana de superposición transparente y click-through (WS_EX_TRANSPARENT), permitiendo seguir usando la aplicación de examen.

Configuración Personalizable: Panel de control (GUI) intuitivo para definir:

Área de Captura (ROI): Define la región exacta de la pantalla donde se encuentra el cuestionario.

Teclas Rápidas (Hotkeys): Personaliza la tecla para iniciar la captura/análisis y la tecla para borrar la respuesta.

Visualización: Ajusta el tamaño, color, posición y peso (negrita) de la fuente de la respuesta.

Sistema de Licencias y Prueba Gratuita: Incluye un sistema robusto para gestionar licencias a través de un servidor remoto (validación por HWID y clave cifrada), con un generoso modo de prueba gratuito.

Seguridad: La configuración se guarda cifrada localmente usando cryptography.fernet para proteger la API Key de Google y otros datos sensibles.

Autogestión: Incorpora un mecanismo de auto-actualización que detecta y descarga nuevas versiones del servidor (requiere configuración de un server.py externo).

🔑 Licencia y Uso (¡Comienza Gratis!)
El asistente opera bajo un modelo de licencia que se gestiona de forma remota, pero puedes probar toda su funcionalidad con nuestro modo de prueba gratuito.

Modo de Prueba Gratuita
Al iniciar por primera vez, el asistente te ofrece 10 usos gratuitos para probar la funcionalidad completa.

El panel de control (pestaña Licencia) muestra los usos restantes.

Una vez que se agotan los 10 usos, necesitarás una licencia completa para continuar usándolo.

Activación de Licencia Completa (Requerida después de la prueba)
Ve a la pestaña Licencia en el Panel de Configuración.

Copia tu HWID (Hardware ID) único.

Utiliza el botón "Enviar solicitud de licencia" (requiere ingresar tu nombre) para notificar al administrador.

Una vez aprobada la licencia por el administrador, la clave se recibirá automáticamente y el estado cambiará a ACTIVA.

💡 ¿Te gusta el asistente? Si encuentras útil este asistente, considera adquirir una licencia para obtener usos ilimitados y apoyar el desarrollo continuo. Contáctanos para adquirir una licencia completa.

⚙️ Instrucciones de Configuración Rápida
Para empezar, necesitas una API Key de Google Gemini.

1. Obtener la API Key de Gemini
Visita Google AI Studio o Google Cloud Console para obtener una clave API válida para los modelos de Gemini.

Copia tu clave.

2. Configurar el Asistente
Ejecuta el asistente (Examenes_licencia.py o el ejecutable compilado).

Haz clic en Iniciar Asistente si se inicia en segundo plano o usa la tecla rápida F9 (por defecto) para abrir el Panel de Configuración.

Navega a la pestaña API & IA.

Pega tu clave API en el campo "Clave API (requerida)".

Asegúrate de que la configuración del modelo sea la recomendada (ej., gemini-2.5-flash y Temperatura: 0.1).

Haz clic en Guardar Configuración.

3. Definir el Área de Captura (ROI)
Ve a la pestaña Captura ROI.

Ajusta los valores de Inicio X, Inicio Y, Ancho y Alto para que cubran exactamente la zona donde aparece la pregunta y las opciones de respuesta del cuestionario en tu pantalla.

Utiliza el botón Previsualizar Captura para ver el rectángulo magenta en la pantalla que indica la zona que será analizada por la IA.

Haz clic en Guardar Configuración.

4. Iniciar y Usar
En el Panel de Configuración, haz clic en Iniciar Asistente para activarlo en segundo plano.

Abre el cuestionario o examen.

Presiona la tecla F8 (por defecto) para iniciar la captura de pantalla y el análisis de la IA. La respuesta aparecerá en la superposición.

Presiona la tecla de borrado (Clic Izquierdo por defecto) para limpiar la respuesta de la pantalla.

🛠️ Tecnología
Lenguaje: Python

GUI: tkinter

Captura de Pantalla: mss, opencv-python

Análisis IA: google-generativeai (Google Gemini API)

Cifrado: cryptography (Fernet)

Comunicaciones: requests

Licenciamiento: Generación de HWID (uuid, platform, hashlib) y validación remota/local.

⚠️ Advertencia de Uso
Este software ha sido diseñado como una herramienta de apoyo y referencia. El uso en contextos prohibidos por regulaciones académicas o de otra índole es responsabilidad exclusiva del usuario. El desarrollador no se hace responsable del uso indebido de esta aplicación.

<img width="1903" height="869" alt="image" src="https://github.com/user-attachments/assets/afbac49d-e899-4bac-b58d-c7666521ca11" />
