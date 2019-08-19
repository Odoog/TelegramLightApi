# TelegramLightApi
Light API to light using Telegram

### Принцип работы

* Написан на php с использованием библиотеки GuzzleHttp и telegram_API

### Настройка

* В классе TelegramBot вставить в $token полученный токен от telegram

# Methods

* getUpdates() - Возвращает обновления на стороне клиента
* sendMessage(chat_id, text, answers) - Отправляет сообщение в chat_id, возможно добавление кнопок, answers - массив с ними 
* sendPhoto($chat_id, $photoAdress, $text = NULL, $answers = NULL) - Отправляет фото по photoAdress в chat_id, поддерживаются кнопки
* sendMapPoint($chat_id, $latitude, $longitude, $answers = NULL) - Отправляет точку на карте в chat_id, также поддерживаются кнопки
