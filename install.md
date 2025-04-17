# Установка
1. Настройте self‑hosted runner с Docker, Python 3.8+ и Node.js 20+.  

2. В GitHub → Settings → Secrets добавьте:  
   `GITHUB_TOKEN`, `DOCKER_HUB_LOGIN`, `DOCKER_HUB_PASSWORD`, `DOCKER_HUB_TOKEN`, `TELEGRAM_TOKEN`, `TELEGRAM_CHANNEL`.  

3. Клонируйте репозиторий и инициализируйте версию:  
   ```bash
   git clone <repo-url> && cd <repo>
   mkdir version && echo "1.0.0" > version/version
   git add version/version && git commit -m "Init version"
   git push

4. Откройте Pull Request в ветку release.
