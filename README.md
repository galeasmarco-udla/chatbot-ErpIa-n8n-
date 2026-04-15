# Chatbot ERP con IA (n8n)

## Descripción
Prototipo de asistente conversacional basado en inteligencia artificial y
procesamiento de lenguaje natural (NLP) que permite realizar consultas sobre
información ERP utilizando datos simulados.

## Arquitectura
Usuario → WhatsApp → Chatwoot → n8n → Agente IA (OpenAI) → Google Sheets

## Componentes
- `n8n` (orquestación)
- `OpenAI` (IA conversacional)
- `Google Sheets` (ERP simulado)
- `Redis` (memoria conversacional)

## Ejecución
1. Importar el archivo `ErpIA.json` en una instancia de n8n
2. Configurar credenciales (OpenAI, Google Sheets, WhatsApp)
3. Activar el workflow
4. Consumir el endpoint Webhook

## Nota
Este proyecto tiene fines académicos y no se conecta a sistemas ERP reales.
