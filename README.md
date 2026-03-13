# Architect Handbook

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![GitHub last commit](https://img.shields.io/github/last-commit/dpetrakov/architect-handbook)](https://github.com/dpetrakov/architect-handbook/commits/main)
[![GitHub issues](https://img.shields.io/github/issues/dpetrakov/architect-handbook)](https://github.com/dpetrakov/architect-handbook/issues)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

**Ru** | [En](i18n/en/README.md)

Методика работы архитекторов: роли, процесс, артефакты, практики, шаблоны.
Масштабируется от точечных аудитов до enterprise-трансформации.

## Зачем это

Архитектурная практика работает на проектах разного масштаба — от точечных аудитов до трансформации ИТ-ландшафта. Архитекторы (solution, technical, enterprise) действуют в разных контекстах, но должны говорить на одном языке, использовать общие подходы и выдавать предсказуемый результат.

Методика — это компактная база знаний, которая отвечает на три вопроса:

1. **Что делает архитектор** — какие задачи решает на каждом этапе проекта
2. **Что он производит** — какие артефакты и в каком виде
3. **Как он это делает** — подходы, инструменты, критерии качества

## Состав методики

| Раздел | Содержание |
| ------ | ---------- |
| [Core Standard](docs/core-standard.md) | Обязательное ядро: уровни rigor (L0-L3), матрица артефактов, определение готовности |
| [Роли и компетенции](docs/roles.md) | 5 профилей архитекторов, зоны ответственности, матрица компетенций |
| [Процесс](docs/process.md) | 8 фаз архитектурного процесса (от пресейла до сопровождения) с AI-усилением |
| [Артефакты](docs/artifacts.md) | 30+ архитектурных документов с шаблонами и примерами |
| [Практики](docs/practices.md) | 18 практик: ADR, ревью, NFR, fitness functions, API, данные, EDA, безопасность, FinOps, платформы, AI |
| [Инструменты](docs/tools.md) | Нотации, профили инструментария по уровням, AI-инструменты |
| [Playbooks](docs/playbooks.md) | 7 playbooks: аудит, discovery, delivery, платформа, модернизация, cloud migration, трансформация |
| [Governance Charter](docs/governance-charter.md) | Права принятия решений, ARB, эскалация, SLA на решения, waivers |
| [Quality Gates](docs/quality-gates.md) | CI/CD gates, чеклисты ревью, gates по фазам процесса |
| [Дорожная карта](docs/roadmap.md) | 3 горизонта внедрения, операционная модель, управление знаниями, метрики |

## Шаблоны

В каталоге [`templates/`](templates/) — 33 готовых шаблона архитектурных артефактов:

- [Solution Concept](templates/solution-concept.md) — концепция решения
- [ADR Template](templates/adr-template.md) / [ADR Example](templates/adr-example.md) — Architecture Decision Record
- [C4 Context](templates/c4-context.md) / [C4 Container](templates/c4-container.md) — диаграммы C4
- [Solution Architecture Document](templates/solution-architecture-doc.md) — документ архитектуры решения
- [Threat Model](templates/threat-model.md) — модель угроз (STRIDE + LINDDUN)
- [NFR Checklist](templates/nfr-checklist.md) — чеклист нефункциональных требований
- [Fitness Functions](templates/fitness-functions.md) — определение fitness functions
- [Integration Design](templates/integration-design.md) — дизайн интеграций
- [API Specification](templates/api-specification.md) — спецификация API
- [Data Model](templates/data-model.md) / [Data Contract](templates/data-contract.md) — модель и контракт данных
- [Cost Model](templates/cost-model.md) / [FinOps Assessment](templates/finops-assessment.md) — стоимость и FinOps
- [Risk Register](templates/risk-register.md) / [Tech Debt Register](templates/tech-debt-register.md) — реестры
- ...и [другие](templates/)

## Starter Kit

Каталог [`starter-kit/`](starter-kit/) — готовая структура каталогов для нового проекта. Скопируйте в репозиторий и начните работать:

- Архитектурная документация (arc42, C4-диаграммы)
- ADR (шаблон + пример)
- Чеклисты качества (NFR, fitness functions, security, AI policy)
- API-спецификация (OpenAPI + правила линтинга)

## Исследование

В каталоге [`research/`](research/) — результаты исследования state-of-the-art архитектурных практик 2024-2026, на основе которого построена методика.

## Принципы

- **Компактность важнее полноты.** Лучше 20 страниц, которые читают, чем 200, которые нет
- **Масштабируемость по проекту.** На маленьком проекте — минимальный набор, на крупном — полная структура
- **Привязка к реальности.** Каждый артефакт и практика проверены на реальных проектах
- **Открытость к инструментам.** Методика не привязана к конкретным тулам

## Рамки

**Что входит:** solution architecture, technical architecture, архитектурное сопровождение разработки, пресейловая работа, enterprise architecture на уровне программ.

**Что не входит:** управление проектами, бизнес-анализ, процессы разработки и тестирования, EA как стратегическая функция, внедрение конкретных платформ.

## Как использовать

1. Начните с [Core Standard](docs/core-standard.md) — определите уровень rigor для вашего проекта (L0-L3)
2. Посмотрите [роли](docs/roles.md) — кто нужен на проекте
3. Пройдите по [процессу](docs/process.md) — какие фазы и что на каждой
4. Возьмите нужные [шаблоны](templates/) — не создавайте артефакты с нуля

## Лицензия

Distributed under the [CC BY-SA 4.0](LICENSE) license.

## Участие в проекте

Contributions welcome! См. [CONTRIBUTING.md](CONTRIBUTING.md).

## Автор

**Дмитрий Петраков** — [GitHub](https://github.com/dpetrakov) | [LinkedIn](https://www.linkedin.com/in/dmitriy-petrakov-43a97096/) | [Сайт](https://dimlight.online/) | [Habr](https://habr.com/ru/users/dpetrakov/)
