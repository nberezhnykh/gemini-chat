# Gemini Chatbot для резюме

[![Java](https://img.shields.io/badge/Java-17-orange.svg)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![React](https://img.shields.io/badge/React-18.x-blue.svg)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-4.x-purple.svg)](https://vitejs.dev/)

**Демонстрация навыков Full-Stack разработки и интеграции с AI путем создания чат-бота, взаимодействующего с Gemini API.**

## О проекте

Этот проект представляет собой полнофункциональное веб-приложение, состоящее из бэкенда на Spring Boot и фронтенда на React. Приложение позволяет пользователю взаимодействовать с чат-ботом, работающим на основе Gemini API от Google.

**Основные возможности:**

* Интуитивно понятный пользовательский интерфейс для общения с чат-ботом.
* Бэкенд на Spring Boot для обработки запросов и взаимодействия с Gemini API.
* Фронтенд на React для динамичного отображения сообщений.
* Использование Vite для быстрой разработки фронтенда.

## Технологии

**Бэкенд:**

* [Java](https://www.oracle.com/java/)
* [Spring Boot](https://spring.io/projects/spring-boot)
* [Spring Webflux](https://spring.io/projects/spring-webflux)
* [Maven](https://maven.apache.org/)
* [Spring WebClient](https://spring.io/projects/spring-framework#learn-more)

**Фронтенд:**

* [React](https://react.dev/)
* [Vite](https://vitejs.dev/)
* [npm](https://www.npmjs.com/)
* [Axios](https://axios-http.com/ru/docs/intro)

## Запуск проекта

**Предварительные требования:**

* Установленная [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-downloads.html) (версия 17 или выше рекомендуется).
* Установленный [Node.js](https://nodejs.org/) и [npm](https://www.npmjs.com/) (или [yarn](https://yarnpkg.com/)).
* Аккаунт Google Cloud с доступом к [Gemini API](https://ai.google.dev/).
* Ключ API для Gemini API.

**Инструкции по запуску:**

1.  **Клонируйте репозиторий:**
    ```bash
    git clone <URL вашего репозитория>
    cd <название вашего репозитория>
    ```

2.  **Настройка бэкенда (Spring Boot):**
    * Перейдите в директорию бэкенда (обычно корень проекта).
    * В файл `src/main/resources/application.properties` добавьте ваш ключ API Gemini:
        ```properties
        gemini.api.key=YOUR_GEMINI_API_KEY
        gemini.api.url=[https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key=](https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key=)
        ```
      (Убедитесь, что URL соответствует актуальной версии Gemini API)
    * Запустите бэкенд с помощью Maven или Gradle:
        ```bash
        # Для Maven
        ./mvnw spring-boot:run
        ```
      Бэкенд должен запуститься на `http://localhost:8080`.

3.  **Настройка фронтенда (React):**
    * Перейдите в директорию фронтенда (обычно папка `frontend` или `client`).
    * Установите зависимости:
        ```bash
        npm install
        ```
    * Запустите фронтенд:
        ```bash
        npm run dev
        ```

4.  **Откройте приложение в браузере:** Перейдите по адресу `http://localhost:5173`.
