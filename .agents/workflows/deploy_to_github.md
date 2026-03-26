---
description: How to deploy the Ni-It landing page to GitHub Pages
---

Чтобы опубликовать ваш сайт в интернете через GitHub Pages бесплатно, выполните следующие шаги:

### 1. Подготовка на GitHub
1. Перейдите на [github.com](https://github.com) и войдите в свой аккаунт.
2. Нажмите **New** (создать новый репозиторий).
3. Введите имя проекта (например, `ni-it-landing`).
4. Оставьте его **Public** и нажмите **Create repository**.
5. Скопируйте ссылку на ваш репозиторий (она выглядит как `https://github.com/ваш-логин/ni-it-landing.git`).

### 2. Загрузка файлов из терминала (VS Code или Git Bash)
Откройте терминал в папке `C:\Ni_It` и введите команды:

```bash
# Инициализация гит
git init

# Добавление всех файлов (index.html, style.css, script.js, hero.png)
git add .

# Первый коммит
git commit -m "Initial commit: Ni-It landing page"

# Привязка к GitHub (вставьте свою ссылку вместо URL)
git remote add origin https://github.com/ваш-логин/ni-it-landing.git

# Переименование ветки в main
git branch -M main

# Загрузка файлов
git push -u origin main
```

### 3. Включение сайта
1. В вашем репозитории на GitHub перейдите во вкладку **Settings** (Настройки).
2. В левом меню выберите **Pages**.
3. В разделе **Build and deployment** выберите:
   - Source: **Deploy from a branch**
   - Branch: **main** / **(root)**
4. Нажмите **Save**.
5. Через 1-2 минуты сверху появится ссылка: *Your site is live at...*

Теперь ваш сайт доступен всему миру!
