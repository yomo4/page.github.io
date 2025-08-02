# 🚀 Развертывание сайта на GitHub Pages

## 📋 Пошаговая инструкция

### 1. Создание репозитория на GitHub

1. Идите на [github.com](https://github.com) и войдите в аккаунт
2. Нажмите **"New repository"** (зеленая кнопка)
3. Заполните данные:
   - **Repository name:** `w3w4lk0ncjiouds-links`
   - **Description:** `Personal links and donations hub for w3w4lk0ncjiouds`
   - **Visibility:** Public (обязательно для бесплатного GitHub Pages)
   - ❌ НЕ ставьте галочки на README, .gitignore, license
4. Нажмите **"Create repository"**

### 2. Загрузка файлов в репозиторий

#### Через Git (рекомендуется)
```bash
# В папке с файлами сайта
git init
git add .
git commit -m "Initial commit: w3w4lk0ncjiouds personal links site"
git branch -M main
git remote add origin https://github.com/ВАШ_ПОЛЬЗОВАТЕЛЬ/w3w4lk0ncjiouds-links.git
git push -u origin main
```

#### Через веб-интерфейс GitHub
1. На странице репозитория нажмите **"uploading an existing file"**
2. Перетащите все файлы проекта в область загрузки
3. Напишите commit message: `"Add personal links website"`
4. Нажмите **"Commit changes"**

### 3. Настройка GitHub Pages

1. В репозитории перейдите в **Settings** (последняя вкладка)
2. Прокрутите до раздела **"Pages"** (в левом меню)
3. В **"Source"** выберите **"Deploy from a branch"**
4. В **"Branch"** выберите **"main"** и **"/ (root)"**
5. Нажмите **"Save"**

### 4. Важные настройки

#### Обновить USDT адрес
В файле `index.html` найдите строку 474 и замените:
```html
<div class="wallet-address" id="usdtAddress">
    ВАШ_USDT_TRC20_АДРЕС_ЗДЕСЬ
```

#### Проверить ссылки
Убедитесь, что все ваши ссылки корректны:
- ✅ Discord: `https://discord.gg/AnkuZkbpfT`
- ✅ SoundCloud: `https://soundcloud.com/wwhclub`
- ✅ Telegram: `https://t.me/+qMUt63prwzs2ZDAy`
- ✅ FunPay: `https://funpay.com/users/3011202/`
- ✅ Donation Alerts: `https://www.donationalerts.com/r/22shalav`

### 5. Получение ссылки на сайт

После настройки GitHub Pages ваш сайт будет доступен по адресу:
```
https://ВАШ_ПОЛЬЗОВАТЕЛЬ.github.io/w3w4lk0ncjiouds-links/
```

**Время активации:** 5-10 минут после настройки

### 6. Проверка работы

1. Откройте ваш сайт в браузере
2. Проверьте все ссылки (должны открываться в новых вкладках)
3. Протестируйте кнопку копирования USDT адреса
4. Убедитесь, что сайт корректно отображается на мобильных

## 🔧 Дальнейшая настройка

### Пользовательский домен (опционально)

1. Купите домен (например, `w3w4lk0ncjiouds.com`)
2. В настройках домена добавьте CNAME запись:
   ```
   www.yourdomain.com -> ВАШ_ПОЛЬЗОВАТЕЛЬ.github.io
   ```
3. В файле `CNAME` замените содержимое на ваш домен:
   ```
   www.yourdomain.com
   ```
4. В настройках GitHub Pages укажите ваш домен

### SSL сертификат

GitHub Pages автоматически предоставляет SSL сертификат для:
- Стандартных доменов `*.github.io`
- Пользовательских доменов (после настройки)

### Аналитика (опционально)

Если хотите отслеживать посетителей, добавьте перед `</head>`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

## 🔄 Обновление сайта

### Через Git
```bash
# Внесите изменения в файлы
git add .
git commit -m "Update: описание изменений"
git push
```

### Через веб-интерфейс
1. Нажмите на файл, который хотите изменить
2. Нажмите иконку карандаша (Edit)
3. Внесите изменения
4. Commit changes

**Время обновления:** 1-5 минут после коммита

## 🛡️ Безопасность

### Что НЕ загружать в репозиторий:
- ❌ Приватные ключи кошельков
- ❌ Пароли или API ключи
- ❌ Личные данные
- ❌ Большие файлы (>100MB)

### Что безопасно:
- ✅ Публичные адреса кошельков
- ✅ Ссылки на социальные сети
- ✅ HTML/CSS/JS код
- ✅ Изображения и иконки

## 📊 Оптимизация SEO

Сайт уже оптимизирован для поиска:
- ✅ Meta описания
- ✅ Ключевые слова
- ✅ Структурированные данные
- ✅ Быстрая загрузка
- ✅ Мобильная адаптация

## 🚨 Решение проблем

### Сайт не открывается
- Проверьте настройки GitHub Pages
- Убедитесь, что репозиторий публичный
- Подождите 10-15 минут после настройки

### Ошибка 404
- Убедитесь, что файл называется `index.html`
- Проверьте ветку (должна быть `main`)
- Проверьте путь в настройках Pages

### Изменения не отображаются
- Очистите кеш браузера (Ctrl+F5)
- Проверьте, что изменения закоммичены
- Подождите 5 минут для обновления

## 📞 Поддержка

При возникновении проблем:
1. Проверьте статус GitHub на [githubstatus.com](https://githubstatus.com)
2. Посмотрите Actions в репозитории на предмет ошибок
3. Обратитесь в поддержку GitHub

---

**🎉 Готово!** Ваш персональный сайт теперь доступен в интернете!

*© 2024 w3w4lk0ncjiouds deployment guide*