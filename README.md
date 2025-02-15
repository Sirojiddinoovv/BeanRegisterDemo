# 🏗 BeanRegisterDemo

**BeanRegisterDemo** — это Spring Boot-приложение, которое автоматически назначает случайные значения полям, аннотированным `@UniqueRequestId`. Используется **CGLIB-прокси**, позволяя динамически изменять значения при каждом обращении к полю.

---

## Функциональность
- **Автоматическая генерация случайных значений** (Long, String) для полей с '@UniqueRequestId'.
- **Динамическое обновление значений при каждом вызове**.
- **Spring BeanPostProcessor + CGLIB** для подмены доступа к полям.
- **Многослойная архитектура** (configuration, service, model, endpoint).

---

## 📌 Как работает `@UniqueRequestId`
Аннотация `@UniqueRequestId` применяется к полям и указывает, что их значения должны **автоматически обновляться**.
