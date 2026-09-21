# AI Закупщик

## 1. Название проекта

**AI Закупщик**

## 2. Краткое описание

**AI Закупщик** — SaaS-система для автоматизации закупочной деятельности бизнеса.

Система анализирует данные о товарах, продажах и остатках на складе, определяет необходимость пополнения запасов и формирует рекомендации по закупкам.

Основная цель проекта — сократить время, затрачиваемое сотрудниками на анализ остатков и планирование закупок, а также снизить риск дефицита или избыточного запаса товаров.

## 3. Участники команды

| Участник            | Роль                                                    |
| ------------------- | ------------------------------------------------------- |
| **Ярошенко Андрей** | Backend-разработчик, Архитектор, DevOps                 |
| **Мягких Кирилл**   | Frontend-разработчик, Руководитель проекта              |
| **Суворов Максим**  | Аналитик, Тестировщик                                   |

## 4. Трекер задач

Задачи проекта ведутся в трекере:

**[GitHub Projects](https://github.com/orgs/Terafluxxx/projects/1/views/1)**

## 5. Технологический стек

### Backend

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,postgres,maven" />
</p>

* <img src="https://skillicons.dev/icons?i=java" width="20" height="20" alt="Java" /> **Java 21** — основной язык backend-разработки
* <img src="https://skillicons.dev/icons?i=spring" width="20" height="20" alt="Spring Boot" /> **Spring Boot** — разработка серверного приложения
* <img src="https://skillicons.dev/icons?i=spring" width="20" height="20" alt="Spring Security" /> **Spring Security** — аутентификация и авторизация
* <img src="https://skillicons.dev/icons?i=spring" width="20" height="20" alt="Spring Data JPA" /> **Spring Data JPA** — работа с базой данных
* <img src="https://skillicons.dev/icons?i=postgres" width="20" height="20" alt="PostgreSQL" /> **PostgreSQL** — реляционная база данных
* <img src="https://skillicons.dev/icons?i=maven" width="20" height="20" alt="Maven" /> **Maven** — управление зависимостями и сборка проекта

### Frontend

<p align="center">
  <img src="https://skillicons.dev/icons?i=vue,html,css" />
  <img src="https://cdn.simpleicons.org/axios/5A29E4" width="48" height="48" alt="Axios" />
</p>

* <img src="https://skillicons.dev/icons?i=vue" width="20" height="20" alt="Vue.js" /> **Vue.js** — разработка пользовательского интерфейса
* <img src="https://skillicons.dev/icons?i=html" width="20" height="20" alt="HTML5" /> **HTML5** — структура веб-приложения
* <img src="https://skillicons.dev/icons?i=css" width="20" height="20" alt="CSS3" /> **CSS3** — стилизация интерфейса
* <img src="https://skillicons.dev/icons?i=vue" width="20" height="20" alt="Vue Router" /> **Vue Router** — маршрутизация
* <img src="https://cdn.simpleicons.org/axios/5A29E4" width="20" height="20" alt="Axios" /> **Axios** — HTTP-запросы к Backend

### Инфраструктура и DevOps

<p align="center">
  <img src="https://skillicons.dev/icons?i=docker,nginx,git,github" />
</p>

* <img src="https://skillicons.dev/icons?i=docker" width="20" height="20" alt="Docker" /> **Docker** — контейнеризация приложения
* <img src="https://skillicons.dev/icons?i=docker" width="20" height="20" alt="Docker Compose" /> **Docker Compose** — управление набором контейнеров
* <img src="https://skillicons.dev/icons?i=nginx" width="20" height="20" alt="Nginx" /> **Nginx** — веб-сервер и reverse proxy
* <img src="https://skillicons.dev/icons?i=git" width="20" height="20" alt="Git" /> **Git** — система контроля версий
* <img src="https://skillicons.dev/icons?i=github" width="20" height="20" alt="GitHub" /> **GitHub** — хранение исходного кода и управление проектом

### Дополнительные технологии

<p align="center">
  <img src="https://cdn.simpleicons.org/openapiinitiative/6BA539" width="48" height="48" alt="REST API" />
  <img src="https://cdn.simpleicons.org/jsonwebtokens/000000" width="48" height="48" alt="JWT" />
  <img src="https://cdn.simpleicons.org/swagger/85EA2D" width="48" height="48" alt="OpenAPI / Swagger" />
</p>

* <img src="https://cdn.simpleicons.org/openapiinitiative/6BA539" width="20" height="20" alt="REST API" /> **REST API** — взаимодействие frontend и backend
* <img src="https://cdn.simpleicons.org/jsonwebtokens/000000" width="20" height="20" alt="JWT" /> **JWT** — аутентификация пользователей
* <img src="https://cdn.simpleicons.org/swagger/85EA2D" width="20" height="20" alt="OpenAPI / Swagger" /> **OpenAPI / Swagger** — документация и тестирование API

## 6. Общая схема системы

```text
                    Пользователь
                         │
                         ▼
              ┌─────────────────────┐
              │      Frontend       │
              │       Vue.js        │
              └──────────┬──────────┘
                         │
                      REST API
                         │
                         ▼
              ┌─────────────────────┐
              │       Backend       │
              │ Java + Spring Boot  │
              └──────────┬──────────┘
                         │
                         │        
                         │
                         ▼
              ┌─────────────────────┐
              │     PostgreSQL      │
              └─────────────────────┘
