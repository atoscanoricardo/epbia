# Taller Práctico 4: Mi Primera Automatización con n8n 🔗

Aprenderás a conectar dos mundos: la recepción de información y el procesamiento inteligente.

## 🛠 El Flujo de Trabajo (Workflow)

Tu reto es crear un flujo que:
1.  **Escuche**: Cuando recibas un formulario web (o un webhook de prueba).
2.  **Piense**: Envíe el texto a una IA (OpenAI o Anthropic nodo).
3.  **Actúe**: Envíe un resumen por correo o Telegram.

### Pasos Sugeridos:
1.  Entra a una instancia de [n8n](https://n8n.io/) (puedes usar la versión de prueba en la nube).
2.  Arrastra un nodo de **"Webhook"** como disparador.
3.  Conéctalo a un nodo de **"AI Agent"** o **"Basic LLM Chain"**.
4.  Configura el prompt del nodo de IA: "Resume el siguiente mensaje en una sola frase muy potente".
5.  Conecta el final a un nodo de **"Email"** o **"Slack"**.

---

## 🏆 Criterio de Éxito
Envía un mensaje de prueba a tu Webhook y verifica que recibes el resumen en tu correo o chat en menos de 10 segundos. ¡Has construido un sistema que trabaja por ti!
