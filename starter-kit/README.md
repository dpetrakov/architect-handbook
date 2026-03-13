# Architecture Starter Kit

Шаблон архитектурной документации для быстрого старта на проекте.

## Как начать

1. Скопируйте содержимое этого каталога в корень вашего проекта
2. Заполните `architecture/README.md` — основной документ архитектуры
3. Создайте первые ADR в `decisions/` (начните с архитектурных принципов)
4. Заполните `quality/nfr-checklist.md` совместно со стейкхолдерами
5. Разместите `CLAUDE.md` в корне репозитория (если используете AI-агенты)

## Структура

```
architecture/
  README.md              # Solution Architecture Document (arc42)
  context.mmd            # C4 Context diagram (Mermaid)
  containers.mmd         # C4 Container diagram (Mermaid)
  components/            # C4 Component diagrams (по необходимости)

decisions/
  README.md              # Decision Log
  0001-template.md       # Шаблон ADR
  0002-example.md        # Пример заполненного ADR

quality/
  nfr-checklist.md       # Чеклист нефункциональных требований
  fitness-functions.md   # Определения fitness functions
  security.md            # Security requirements / threat model (STRIDE + LINDDUN)
  ai-policy.md           # AI policy проекта

api/
  openapi.yaml           # API спецификация (OpenAPI 3.1)
  .spectral.yaml         # Правила линтинга API

CLAUDE.md                # Контекст для AI-агента
```

## Минимальный набор (аудит / экспресс-оценка)

- `architecture/context.mmd` — C4 Context
- `decisions/` — хотя бы 1-2 ADR

## Базовый набор (средний проект)

- Всё из минимального
- `architecture/README.md` + `containers.mmd`
- `quality/nfr-checklist.md`
- `quality/security.md` — threat model и security requirements
- `api/openapi.yaml`

## Полный набор (трансформация)

- Всё из базового
- `quality/fitness-functions.md` — автоматические проверки (включая cost и sustainability)
- `quality/ai-policy.md`
- `architecture/components/`
- Дополнительно на проекте: FinOps Assessment, Cost Model, Platform Assessment, Waiver Register (шаблоны в методике)
