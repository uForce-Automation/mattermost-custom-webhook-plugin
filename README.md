# mattermost-custom-webhook-plugin

В данном репозитории содержится темплейт простого плагина для Mattermost. Данный плагин добавляет одну кастомную команду в mm. При использовании неё отправляется POST запрос на адрес, указанный в `webhookUrl` в `command.go`. В запросе содержится следующая информация:
```{
		"root_id": root_id,   // root id треда, внутри которого отправлено сообщение с командой
		"raw_text": raw_text, // текст сообщения с командой без самой командый внутри
	}```
