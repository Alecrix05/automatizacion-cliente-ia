# Automatización de Atención al Cliente con IA

## Descripción

Proyecto de automatización de atención al cliente desarrollado con n8n, Docker, PostgreSQL y modelos de lenguaje (LLMs) mediante OpenRouter.

El sistema recibe consultas de clientes a través de un webhook, procesa la solicitud utilizando inteligencia artificial y genera respuestas automáticas personalizadas. Además, almacena cada interacción en una base de datos PostgreSQL para su posterior análisis y seguimiento.

El objetivo es reducir el tiempo dedicado a responder consultas repetitivas relacionadas con servicios de soporte técnico para computadoras, mejorando la eficiencia operativa y la atención al cliente.

---

## Arquitectura

```text
Cliente
   │
   ▼
Webhook (n8n)
   │
   ▼
Procesamiento de Datos
   │
   ▼
AI Agent
   │
   ▼
LLM (OpenRouter)
   │
   ├──► PostgreSQL (Registro de conversaciones)
   │
   ▼
Respuesta Automática
```

---

## Tecnologías Utilizadas

* n8n
* Docker
* Docker Compose
* PostgreSQL
* WSL2
* Ubuntu Linux
* OpenRouter API
* Large Language Models (LLMs)
* REST APIs
* JSON
* Git
* GitHub

---

## Funcionalidades Implementadas

* Recepción de mensajes mediante Webhooks.
* Procesamiento de solicitudes en formato JSON.
* Integración con modelos de inteligencia artificial a través de OpenRouter.
* Generación automática de respuestas contextuales.
* Registro de conversaciones en PostgreSQL.
* Persistencia de datos mediante volúmenes Docker.
* Arquitectura modular basada en workflows de n8n.
* API local para pruebas y desarrollo.
* Despliegue mediante contenedores Docker.

---

## Base de Datos

Actualmente el sistema registra cada interacción en PostgreSQL.

### Tabla: clientes

| Campo     | Tipo        |
| --------- | ----------- |
| id        | SERIAL      |
| fecha     | TIMESTAMP   |
| mensaje   | TEXT        |
| respuesta | TEXT        |
| estado    | VARCHAR(50) |

Ejemplo:

| id | fecha      | mensaje                 | respuesta                    | estado |
| -- | ---------- | ----------------------- | ---------------------------- | ------ |
| 1  | 2026-06-13 | Mi impresora no imprime | Un técnico revisará el caso. | nuevo  |

---

## Ejemplo de Uso

### Solicitud

```json
{
  "mensaje": "¿Cuánto cuesta instalar Windows?"
}
```

### Respuesta

```json
{
  "respuesta": "La instalación básica de Windows tiene un costo de $500 MXN. ¿Deseas incluir Office o respaldo de información?"
}
```

---

## Aprendizajes y Competencias Desarrolladas

Durante el desarrollo de este proyecto se aplicaron conocimientos de:

* Automatización de procesos.
* Integración de APIs REST.
* Arquitecturas orientadas a eventos.
* Diseño de workflows con n8n.
* Contenedores Docker y Docker Compose.
* Administración básica de PostgreSQL.
* Linux y WSL2.
* Ingeniería de prompts.
* Integración de modelos de inteligencia artificial.
* Desarrollo backend basado en Webhooks.
* Persistencia y almacenamiento de datos.

---

## Escalabilidad y Mejoras Futuras

### Corto Plazo

* Catálogo dinámico de servicios y precios.
* Validación automática de información del cliente.
* Mejor gestión del contexto conversacional.
* Clasificación automática de solicitudes.

### Mediano Plazo

* Integración con WhatsApp Business.
* Integración con Facebook Messenger.
* Integración con Instagram Direct Messages.
* Registro automático de prospectos.
* Panel básico de seguimiento de clientes.

### Largo Plazo

* Implementación de RAG (Retrieval-Augmented Generation).
* Base de conocimiento empresarial.
* Integración con CRM.
* Seguimiento automático de clientes.
* Agenda de citas automatizada.
* Dashboard de métricas y analítica.
* Despliegue en infraestructura cloud.
* Integración con modelos de IA locales.

---

## Instalación

```bash
git clone <repositorio>
cd automatizacion-cliente-ia

docker compose up -d
```

Acceder a:

```text
http://localhost:5678
```

---

## Objetivo Profesional

Este proyecto demuestra experiencia práctica en:

* Automatización de procesos empresariales.
* Integración de APIs y servicios externos.
* Desarrollo de soluciones impulsadas por IA.
* Uso de Docker para despliegue y portabilidad.
* Diseño de arquitecturas backend basadas en eventos.
* Gestión de datos mediante PostgreSQL.

El proyecto está diseñado para evolucionar hacia una plataforma completa de atención automatizada multicanal para pequeñas empresas y profesionales independientes.
