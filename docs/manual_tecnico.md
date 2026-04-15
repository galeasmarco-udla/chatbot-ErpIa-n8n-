# Manual Técnico
## Chatbot ERP con IA Conversacional

### 1. Descripción general
El sistema es un prototipo de chatbot empresarial basado en inteligencia artificial
y procesamiento de lenguaje natural, desarrollado sobre la plataforma n8n,
con integración a Google Sheets como ERP simulado.

---

### 2. Arquitectura del sistema
La solución sigue una arquitectura modular por capas:

- Capa de interacción (WhatsApp)
- Capa de orquestación (n8n)
- Capa de IA conversacional (OpenAI)
- Capa de datos (Google Sheets)
- Capa de memoria (Redis)

(Ver documento de arquitectura en la carpeta docs)

---

### 3. Componentes principales
- n8n: orquestación de flujos
- OpenAI: procesamiento NLP y multimodal
- Google Sheets: datos ERP simulados
- Redis: memoria conversacional
- Evolution API: mensajería WhatsApp

---

### 4. Despliegue del sistema
El sistema se despliega importando el workflow `ErpIA.json`
en una instancia de n8n y configurando las credenciales correspondientes.

---

### 5. Configuración de variables y credenciales
Las variables de entorno se documentan en `.env.example`.
Las credenciales reales se configuran directamente en n8n
y no se incluyen en el repositorio por razones de seguridad.

---

### 6. Gestión de datos
Los datos de negocio corresponden a datasets simulados,
con estructura típica de un ERP (clientes, productos, ventas).

---

### 7. Limitaciones técnicas
- No integración con ERP productivo
- No alta disponibilidad
- No escalamiento automático
- Uso académico y demostrativo

---

### 8. Mantenimiento y extensibilidad
El sistema puede extenderse incorporando nuevas fuentes de datos,
dominios de consulta o capacidades analíticas adicionales.

