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

## Looks
To change the looks and feel use dunstrc in `~/.config/dunst/dunstrc`
### Battery Critical
![image](https://github.com/user-attachments/assets/aca1fd92-7bd4-4d52-9e35-9e23592d0ddc)

### Battery Low
![image](https://github.com/user-attachments/assets/d9874762-81f3-4d43-97bd-8b6489f9c8d5)

### Battery Almost Full
![image](https://github.com/user-attachments/assets/2f6d9233-e220-49d0-af28-3f22c9d69a6c)

