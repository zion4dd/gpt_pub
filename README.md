Backend проект: автоматизация запросов к ChatGPT  

Клиент получает возможность автоматизировать запросы к ChatGPT задавая темы и параметры запроса, а так же расписание.  
Исходя из параметров запроса собирается промпт для GPT. Полученный ответ обрабатывается и сохраняется в БД.  
Параметры позволяют подбирать темы, подставлять значения, выбор языка, добавление HTML разметки, добавление разделов (введение, выводы).  

Проект реализован на Flask.  
БД: SQLite или Postgresql через ORM SQLAlchemy  
Расписание: CRON.  
Мониторинг: Sentry.  
Дебаг: Telegram бот и шаблонные представления html + jinja.  
Тестирование: Pytest.  
Асинхронные запросы: asyncio.  
