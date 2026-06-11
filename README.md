# Automatización de Atención al Cliente con IA

## Descripción

Proyecto de automatización desarrollado con n8n, Docker y modelos de lenguaje (LLMs) mediante OpenRouter. El objetivo es reducir el tiempo dedicado a responder consultas repetitivas de clientes relacionadas con servicios de soporte técnico para computadoras.

El sistema recibe mensajes a través de un Webhook, procesa la solicitud utilizando un agente de inteligencia artificial y devuelve una respuesta automática en formato JSON.

## Arquitectura

Cliente → Webhook → Procesamiento de Datos → AI Agent → Modelo LLM (OpenRouter) → Respuesta Automática

## Tecnologías Utilizadas

* n8n
* Docker
* WSL2
* Ubuntu Linux
* OpenRouter API
* Large Language Models (LLMs)
* JSON
* REST APIs
* Git
* GitHub

## Funcionalidades Implementadas

* Recepción de mensajes mediante Webhooks.
* Procesamiento de datos JSON.
* Integración con modelos de IA a través de OpenRouter.
* Generación automática de respuestas.
* API local para pruebas y desarrollo.
* Arquitectura modular basada en workflows de n8n.
* Despliegue mediante contenedores Docker.

## Ejemplo de Uso

Solicitud:

```json
{
  "mensaje": "¿Cuánto cuesta instalar Windows?"
}
```

Respuesta:

```json
{
  "respuesta": "Hola, ¿podrías indicarme el modelo de tu computadora y si requieres respaldo de información para poder proporcionarte una cotización?"
}
```

## Aprendizajes y Competencias Desarrolladas

Durante el desarrollo de este proyecto se aplicaron conocimientos de:

* Automatización de procesos.
* Integración de APIs.
* Arquitecturas basadas en eventos.
* Contenedores Docker.
* Linux y WSL2.
* Ingeniería de prompts.
* Integración de modelos de inteligencia artificial.
* Diseño de flujos de trabajo con n8n.
* Desarrollo de servicios backend basados en Webhooks.

## Escalabilidad y Mejoras Futuras

### Corto Plazo

* Incorporar catálogo de servicios y precios.
* Mejorar el contexto y las respuestas del asistente.
* Validación automática de información proporcionada por el cliente.

### Mediano Plazo

* Integración con WhatsApp Business.
* Integración con Facebook Messenger.
* Integración con Instagram Direct Messages.
* Registro automático de prospectos.

### Largo Plazo

* Implementación de una base de conocimiento mediante RAG.
* Integración con CRM.
* Seguimiento automático de clientes.
* Agenda de citas automatizada.
* Dashboard de métricas y análisis.
* Despliegue en infraestructura cloud.

## Objetivo Profesional

Este proyecto demuestra experiencia práctica en automatización de procesos, integración de APIs, despliegue de aplicaciones con Docker y uso de inteligencia artificial generativa para resolver problemas reales de negocio.
