# Ремонт под контролем

Документация проекта разложена по назначению из исходного файла `Аналитика и архитектура.docx`.

## Структура

```text
docs/
  00-scope-and-decisions.md
  01-system-requirements.md
  02-architecture.md
  03-data-model.md
  04-rbac-and-statuses.md
  05-ui-flows.md
  06-traceability-and-tests.md
  adr/
    ADR-001-architecture-style.md
    ADR-002-authentication.md
    ADR-003-file-storage.md
openapi/
  openapi.yaml
README.md
.env.example
```

## Исходный документ

Проект: «Ремонт под контролем». Версия БА 1.1 от 18.08.2026. Ответственные: Максим, Никита. Исходный статус: «Согласовано к проектированию».

## Быстрая навигация

- Scope и решения → `docs/00-scope-and-decisions.md`
- Системные требования и безопасность → `docs/01-system-requirements.md`
- Архитектура → `docs/02-architecture.md`
- Модель данных → `docs/03-data-model.md`
- RBAC и статусы → `docs/04-rbac-and-statuses.md`
- UI → `docs/05-ui-flows.md`
- Трассировка и тесты → `docs/06-traceability-and-tests.md`
- Архитектурные решения → `docs/adr/`
- API → `openapi/openapi.yaml`

## Основной стек

Frontend: HTML5/CSS3/JavaScript ES6+.  
Backend: Java 21/Spring Boot 3.4.  
DB: PostgreSQL 16.  
ORM: Hibernate 6/Spring Data JPA.  
API: REST/JSON.  
Tests: JUnit 5/Mockito.  
Migrations: Flyway.  
Files: `./uploads`.

## Основной жизненный цикл

`PLANNED → IN_PROGRESS → ON_REVIEW → AWAITING_PAYMENT → PAID`

Ветка возврата:

`ON_REVIEW → REWORK → IN_PROGRESS → ON_REVIEW`

## MVP

В MVP входят объекты, участники, карточки работ, сдача фотографиями, комментарии, история статусов, финансовые агрегаты, авторизация, RBAC, миграции, seed и localhost-развёртывание.

Не входят самостоятельная регистрация, сброс пароля, удаление/архивирование/восстановление, обязательное видео, realtime-чат и production-ready масштабирование.

