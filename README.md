# ☄️ KVAZAR — Kvazarchik

Единый Discord-бот для сервера KVAZAR. Проект использует независимую реализацию функций, вдохновлённую публично описанными категориями XIVIVIDE: profiles/economy, protection, logs, moderation, support, staff, events, creative, giveaways, clans и games.

## Установка на Bothost

1. Распакуй архив.
2. Открой `config.py`.
3. Вставь Discord Bot Token в `BOT_TOKEN`.
4. Проверь `GUILD_ID` и `OWNER_ID` — они уже заполнены.
5. Установи зависимости из `requirements.txt`.
6. Файл запуска: `main.py`.
7. В Discord Developer Portal включи **Server Members Intent** и **Message Content Intent**.

`.env` не используется.

## Основные команды

### Пользователь
`/help` `/ping` `/profile` `/balance` `/daily` `/transfer` `/inventory` `/shop` `/buy` `/tasks` `/room`

### Модерация
`/warn` `/warnings` `/unwarn` `/resetwarns` `/timeout` `/untimeout` `/kick` `/ban` `/unban` `/clear` `/slowmode` `/lock` `/unlock` `/nick`

### Support
`/ticket` `/close_ticket` `/appeal` `/verify` `/verification_status`

### Staff
`/shift` `/shift_status` `/staff_stats`

### Events / Creative
`/event` `/event_close` `/event_result` `/creative`

### Giveaways
`/giveaway` `/giveaway_end` `/giveaway_reroll`

### Clans
`/clan_create` `/clan_info` `/clan_join` `/clan_leave` `/clan_kick` `/clan_promote` `/clan_deposit` `/clan_list`

### Games
`/mafia` `/mafia_join` `/mafia_start` `/mafia_end` `/coinflip` `/dice` `/slots`

### MOG
`/mog`

### Admin
`/setup` `/give` `/take` `/setshop` `/payment_add` `/db_stats` `/log_test`

## Важно

Это не закрытая копия исходного кода XIVIVIDE. Это самостоятельная реализация по публично описанным функциям. Реальный платёжный шлюз не подключён: `/payment_add` только фиксирует платёж в базе. Для внешнего платёжного провайдера нужен его API/webhook.

SQLite хранится в `data/kvazar.sqlite3`.
