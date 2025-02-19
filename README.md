# Linux Battery Notification
Battery Notification Using dunst, cron, and aplay

## Setup 
1. Install dunst, cron, and aplay
2. download and place the notification sound in
```bash
~/.local/share/sounds/name_of_the_notification_sound.wav
```
3. Add the script to crontab
```bash
crontab -e
```
4. Schedule the battery notification script
```bash
*/15 * * * * /path/to/script/battery-notification
```
**⚠️ Notes:** The script will run every 15 minutes

5. Restart Crond
```bash
sudo systemctl restart crond
```
