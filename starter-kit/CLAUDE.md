# Архитектурный контекст проекта

## Система

<!-- Название и краткое описание -->

TODO — [краткое описание назначения системы]

## Архитектура

- **Стиль:** TODO (микросервисы / modular monolith / монолит)
- **Основные языки:** TODO
- **Инфраструктура:** TODO (Kubernetes / VM / serverless), TODO (облако)
- **БД:** TODO
- **Брокер сообщений:** TODO (RabbitMQ / Kafka / нет)
- **Мониторинг:** TODO

## Ключевые файлы

- `architecture/README.md` — Solution Architecture Document
- `architecture/context.mmd` — C4 Context diagram
- `architecture/containers.mmd` — C4 Container diagram
- `decisions/` — Architecture Decision Records
- `quality/nfr-checklist.md` — нефункциональные требования
- `api/openapi.yaml` — API спецификация

## Правила

- Все архитектурные решения фиксируем в ADR (`decisions/NNNN-*.md`)
- Диаграммы — только Mermaid (не PlantUML, не draw.io)
- API — contract-first подход (OpenAPI 3.1 для REST, AsyncAPI для событий)
- Все сервисы экспортируют метрики, логи и трассировки (OpenTelemetry)
- Code review обязателен для merge
- Документация хранится рядом с кодом в Git

## NFR (ключевые)

- Латентность API: p95 < TODO мс
- Доступность: TODO %
- RTO: < TODO
- RPO: < TODO
- Бюджет инфраструктуры: < TODO ₽/мес
