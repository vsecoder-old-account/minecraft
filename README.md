# Linux Minecraft server 1.12.2

## Install / Установка

```bash
sudo apt update
sudo apt install openjdk-8-jre-headless
sudo apt install screen ufw
sudo ufw allow 25565
git clone https://github.com/htmlcssphpjs/minecraft
cd minecraft
java -Xms1024M -Xmx1024M -jar minecraft_server_1.12.2.jar nogui
```

## Server settings / Настройки сервера

bash:
```bash
nano server.properties
```

```difficulty``` (по умолчанию easy) — Это свойство задает уровень сложности игры, например, уровень наносимого урона и то, как элементы влияют на вашего игрока. Возможные варианты: peaceful, easy, normal и hard.

```gamemode``` (по умолчанию survival) — Это свойство определяет режим игры. Возможные варианты: survival, creative, adventure и spectator.

```level-name``` (по умолчанию world) — Это свойство задает имя вашего сервера, которое будет отображаться в клиенте. Такие символы, как апостроф, возможно, потребуется экранировать с помощью обратной косой черты.

```motd``` (по умолчанию A Minecraft Server) — Сообщение, отображаемое в списке серверов клиента Minecraft.

```pvp``` (по умолчанию true) — Данное свойство активирует pvp режим. Если установлено значение true, игроки смогут вступать в бой и наносить друг другу урон.
