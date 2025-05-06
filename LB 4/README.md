### ***1. MVP-стадия (Low-Cost)***
Архитектура:
Frontend: Firebase Hosting (SPA на React/Vue)

Backend: Cloud Functions (Node.js/Python)

База данных: Firestore (NoSQL)

AI: Dialogflow ES (готовые ML-модели)

Обоснование:
Нулевая стоимость на старте (бесплатные квоты Firebase).
Мгновенное развертывание без управления инфраструктурой.
Автомасштабирование под низкую нагрузку (<100 RPS).

Схема:
![image](https://github.com/user-attachments/assets/156cc534-93de-48e7-a04f-64dda9a9045f)

### ***2. Тестирование партнерами (1000 пользователей/месяц):***
Архитектура:

Frontend: Firebase Hosting + Cloud CDN

Backend: Cloud Run (контейнеры с GPU)

База данных: Cloud SQL (PostgreSQL) + Memorystore (Redis)

AI: Vertex AI (кастомные модели)

Хранение: Cloud Storage (скриншоты/документы)

Обоснование:
Гибкость: Cloud Run поддерживает кастомные ML-модели.

Производительность: GPU ускоряют инференс в 5-10 раз.

Аналитика: SQL позволяет строить сложные отчеты.

Стоимость: ~$420/мес (+23x к MVP).

Схема:
![image](https://github.com/user-attachments/assets/2eae3053-7ffc-4a99-bb60-fede920e0489)


### ***3. Продакшн*** 

Архитектура:
Frontend: Global HTTPS LB + CDN

Backend: GKE Standard (multi-region) + TPU v3

База днных: Cloud Spanner (глобальная) + BigQuery

AI: Feature Store + ML-конвейеры на Vertex AI

Обоснование:
Производительность: TPU снижают задержку ML до <50 мс.

Масштабируемость: Spanner выдерживает >100k транзакций/сек.

Стоимость: ~$3,200/мес (+7.6x к тестированию).

![image](https://github.com/user-attachments/assets/733eb433-789e-46d8-a5e0-c39a14e0a0f5)

Схема:
![image](https://github.com/user-attachments/assets/a70a9d87-5c20-4a43-adb4-a38f0dbcf4fa)
