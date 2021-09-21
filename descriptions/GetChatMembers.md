### 🔥 GET CHAT MEMBERS
Эта функция парсит участников группы или супергруппы.
> 📄 **Файл:** [plugins/GetChatMembers.py](../plugins/GetChatMembers.py)<br/>
⚙ **Параметры:** Обязательно<br/>
💾 **Возвращает:** Файл \*.json<br/>
🚧 **Ограничения:** Не более 10000 записей

#### 🖥 Использование:
Функция настроена так чтобы бот принимал команды в чате "Избранное". В этом чате отправляем себе команду, и здесь же получаем результат.

#### ✏️ Синтаксис:
```bash
/parse_users arg
```
`arg` - Аргумент функции принимает строку с id чата (`1234567890`), доменным именем (`domain`, `@domain`) или ссылкой на чат (`https://t.me/domain`).

#### 📦 Возвращает:
JSON файл, внутри которого список словарей с данными пользователей чата. До 10000 записей, - это ограничение телеграма.
```json
[
	{
		"chat_id": "Чат ид",
		"username": "Домен юзера",
		"first_name": "Имя",
		"last_name": "Фамилия",
		"phone": "Номер телефона",
		"photo": "Файл ид фотографии"
	},
	...
]
```

#### 📝 История изменений:
> **21.09.2021**<br/>_- Загружен плагин "GetChatMembers.py"_