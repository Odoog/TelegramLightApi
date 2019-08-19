# TelegramLightApi
Light API to light using Telegram

### Принцип работы

* Написан на php с использованием библиотеки GuzzleHttp и telegram_API

### Настройка

* В классе TelegramBot вставить в $token полученный токен от telegram

# Methods

* getUpdates() - Возвращает обновления на стороне клиента
* sendMessage(chat_id, text, answers = NULL) - Отправляет сообщение в chat_id, возможно добавление кнопок, answers - массив с ними. При кнопках (answers) keyboardType определяет их тип (reply/inline)
* sendPhoto(chat_id, photoAdress, text = NULL, answers = NULL) - Отправляет фото по photoAdress в chat_id, поддерживаются кнопки. При кнопках (answers) keyboardType определяет их тип (reply/inline)
* sendMapPoint(chat_id, latitude, longitude, answers = NULL) - Отправляет точку на карте в chat_id, также поддерживаются кнопки. При кнопках (answers) keyboardType определяет их тип (reply/inline)
* deleteMessage(chat_id, messageId) - Удаляет сообщение с messageId из чата chat_id (Если возможно)
* editMessage(messageId, chat_id, text, keyboardType = NULL, answers = NULL) - Изменяет сообщение с messageId в чате chat_id на text. При кнопках (answers) keyboardType определяет их тип (reply/inline)
* editCaption(messageId, chat_id, text, keyboardType = NULL, answers = NULL) - Изменяет caption сообщения с messageId в чате chat_id на text. При кнопках (answers) keyboardType определяет их тип (reply/inline)
* reactQuery(queryId) - Помечает актив при нажатой inline кнопке отмеченным
