# 🔐 Authorization API

REST API сервис авторизации пользователей с поддержкой JWT, ролей и административного управления.

## 🚀 Стек технологий

- Java 17
- Spring Boot
- Spring Security
- Spring Data JPA
- PostgreSQL
- Redis
- Maven

## 📌 Функционал

- Регистрация пользователей
- Авторизация
- JWT (Access + Refresh Token)
- Ролевая модель (USER / ADMIN)
- Обновление токенов
- Защита эндпоинтов
- Административное управление пользователями

## 🏗 Архитектура

Controller → Service → Repository  
DTO → Entity → Mapper  

Реализованы:
- Token Filter
- JWT Provider
- Security Config
- Role-based access control

## 🔐 Безопасность

- BCrypt password encoding
- JWT фильтрация запросов
- Ограничение доступа по ролям
- Refresh Token механизм

## ⚙️ Запуск

1. Клонировать репозиторий: git clone https://github.com/Serbly/authorizationAPI.git
2. Настроить application.yml
3. mvn spring-boot:run


## 🧪 Тестирование API

Примеры запросов:

Регистрация: POST /api/auth/register

Авторизация: POST /api/auth/signin

Обновление токена: POST /api/auth/refresh

## 🎯 Назначение проекта

Проект создан как отдельный микросервис авторизации, который можно интегрировать в любые веб- и микросервисные системы.
