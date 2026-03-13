# Security Requirements: [Название проекта]

## Модель угроз (STRIDE per Element)

Анализ угроз привязан к уровням C4. Заполняйте сверху вниз: сначала L1 (trust boundaries), затем L2 (data flows).

### Trust Boundaries

| Граница | Между | Защита |
|---------|-------|--------|
| TB-1 | TODO → TODO | TODO |

### STRIDE per Element

| # | Угроза | Категория | Компонент | Вероятность | Влияние | Риск | Контрмера |
|---|--------|-----------|-----------|:-----------:|:-------:|:----:|-----------|
| T1 | TODO | TODO | TODO | TODO | TODO | TODO | TODO |

### Risk Matrix

| | Impact: Low | Impact: Medium | Impact: High | Impact: Critical |
|:---|:---:|:---:|:---:|:---:|
| **Likelihood: High** | Medium | High | High | Critical |
| **Likelihood: Medium** | Low | Medium | High | High |
| **Likelihood: Low** | Low | Low | Medium | High |

## LINDDUN (Privacy Threats)

> Заполняется при обработке ПДн (152-ФЗ). Пропустите, если система не обрабатывает персональные данные.

| # | Угроза | Категория | Данные | Риск | Контрмера |
|---|--------|-----------|--------|:----:|-----------|
| P1 | TODO | Linkability | TODO | TODO | TODO |
| P2 | TODO | Identifiability | TODO | TODO | TODO |
| P3 | TODO | Unawareness | TODO | TODO | TODO |
| P4 | TODO | Non-compliance | TODO | TODO | TODO |

## Требования

### Аутентификация и авторизация

- [ ] Метод аутентификации: TODO (OAuth 2.0 / OIDC / SAML)
- [ ] MFA: TODO (обязательно / опционально / нет)
- [ ] Модель авторизации: TODO (RBAC / ABAC)
- [ ] Блокировка после N неудачных попыток: TODO
- [ ] Принцип least privilege применён

### Защита данных

- [ ] Шифрование at rest: TODO
- [ ] Шифрование in transit: TLS 1.2+
- [ ] Маскирование PII в логах
- [ ] Политика хранения данных (retention): TODO
- [ ] Классификация данных проведена (PII поля идентифицированы)

### Инфраструктура

- [ ] Сетевая сегментация: TODO
- [ ] WAF: TODO
- [ ] Сканирование зависимостей в CI (SCA)
- [ ] SAST: TODO
- [ ] Secret scanning в CI
- [ ] Audit trail для критичных операций

### Compliance

- [ ] 152-ФЗ (персональные данные): TODO (да/нет)
- [ ] 187-ФЗ (критическая информационная инфраструктура): TODO (да/нет)
- [ ] PCI DSS: TODO (да/нет)
- [ ] DSAR workflow (право на удаление): TODO

## Принятые риски

| Риск | Обоснование | Mitigation | Пересмотр |
|------|-------------|-----------|-----------|
| TODO | TODO | TODO | TODO |
