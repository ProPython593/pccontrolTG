
## Настройка

1.Получение токена

1.1.Зайдите в телеграмм бота @BotFather

1.2.Напишите /newbot

1.3.Напишите название боту

1.4.Напишите ник бота_bot(идёт после @)

1.5.Далее будет сообщение

```
Done! Congratulations on your new bot. You will find it at t.me/ник бота. You can now add a description, about section and profile picture for your bot, see /help for a list of commands. By the way, when you've finished creating your cool bot, ping our Bot Support if you want a better username for it. Just make sure the bot is fully operational before you do this.

Use this token to access the HTTP API:
(Токен) <--Копируем его
Keep your token secure and store it safely, it can be used by anyone to control your bot.

For a description of the Bot API, see this page: https://core.telegram.org/bots/api
```
Если что переводиться это так 
```
Сделанный! Поздравляю с новым ботом. Вы найдете его на t.me/ник бота. Теперь вы можете добавить описание, раздел about и изображение профиля для своего бота, смотрите /help для списка команд. Кстати, когда вы закончите создавать своего крутого бота, отправьте запрос в нашу службу поддержки ботов, если вам нужно лучшее имя пользователя для него. Просто убедитесь, что бот полностью работоспособен, прежде чем делать это.

Используйте этот токен для доступа к HTTP API:
(Токен) <--Копируем его
Обеспечьте безопасность своего токена и храните его в безопасном месте, так как любой может использовать его для управления вашим ботом.

Описание Bot API см. на этой странице: https://core.telegram.org/bots/api.
```
2.Скачайте файл main.py

3.в строке 16 замените <Токен> на ваш скопированый токен

4.в строках 83,84,85 замените <путь к папке со временными фаллами> по примеру:
```python
myScreenshot.save(r'C:\Users\User\Desktop\tg bot\time files\screen.png')
bot.send_document(message.chat.id, open(r'C:\Users\User\Desktop\tg bot\timefiles\screen.png', 'rb'))
os.remove(r'C:\Users\User\Desktop\tg bot\time files\screen.png')
```
5.в строках 21,33 замените <id1> <di2> <id3> на id людей(получить у getmyid_bot) у которых будет доступ по примеру
```python
if message.from_user.id==xxxxxxxxxx or message.from_user.id==xxxxxxxxxx or message.from_user.id==xxxxxxxxxx(и т.д по примеру or message.from_user.id==xxxxxxxxxx):
```

6.Запустите файл если все сделано правильно то бот начнёт работу

## Планы

1.Сделать авто установщик

2.Доделать функцию уведомления

3.сделать дискорд версию

4.сделать под линукс

5.Сделать автозапуск

6.Сделать exe-шник

7.перейти на др. библиотеку бота
