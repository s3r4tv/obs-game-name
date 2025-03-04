# OBS Game Name | Док-панель с названием игры

Это небольшой скрипт для пользовательской док-панели вашего OBS, который выводит текущую категорию со стрима и обновляет данные в заданном диапазоне (по стандарту — 1 минута). Очень полезный скрипт, чтобы всегда визуально контролировать текущую категорию на своём стриме.
### Пример отображения:
![](https://i.imgur.com/q5pQZH2.png)<br>
![](https://i.imgur.com/j7m6oKg.png)

## 🚀 Как настроить и использовать

<details>
<summary>Просмотреть 9 шагов, настройка которых займёт пару минут вашего времени 🤝</summary>

1. Скачайте файл `obs-game-name.html`.
2. Откройте файл в браузере.
3. Перейдите на сайт [Twitch Token Generator](https://twitchtokengenerator.com) и выберите **Custom Scope Token** во всплывающем окне.
4. Пролистайте до "Available Token Scopes" и активируйте эти 3 опции:
   - `channel:read:subscriptions`
   - `user:read:broadcast`
   - `channel:read:editors`

![](https://i.imgur.com/EZrbSO8.png)

5. Нажмите на зелёную кнопку **Generate Token**:<br>
![](https://i.imgur.com/roLvIcC.png)

6. После авторизации на Twitch, нажмите на фиолетовую кнопку для разрешений:<br>
![](https://i.imgur.com/Kz4UhT8.png)

7. Вернувшись на сайт Token Generator, скопируйте следующие токены:
   - `Access Token`
   - `Client ID`

![](https://i.imgur.com/ZQ4Fm3d.png)

8. Вставьте их в файл `obs-game-name.html` в нужные поля, указав ещё и ваш логин:

```javascript
const clientId = "YOU_CLIENT_ID";
const accessToken = "YOU_ACCESS_TOKEN"; 
const username = "you_channel_name"; // ex. playwithserch
```
9. Сохраните файл `obs-game-name.html` и откройте его в браузере.<br>Если всё сделано верно, то в нём отобразится текущая категория вашего Twitch канала.

![](https://i.imgur.com/Bfhzoqu.png)

10. Откройте OBS, затем перейдите в **Док-панели → Пользовательские док-панели браузера**. Укажите название вашей панели и путь к файлу `obs-game-name.html`. Нажмите **Применить** и разместите панель в удобном месте.

![](https://i.imgur.com/nGJEhp9.png)

</details>

## 📡 Контакты

- **E-Mail**: [playwithserch@gmail.com](mailto:playwithserch@gmail.com)
- **Telegram**: [@serch1one](https://t.me/serch1one)


## 📄 Лицензия
Этот проект распространяется под лицензией MIT. Вы можете использовать, копировать, изменять и распространять код в любых целях.

