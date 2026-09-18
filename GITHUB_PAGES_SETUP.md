# 🚀 Посібник: Налаштування GitHub Pages для Git-гайда

## 📋 Зміст
1. [Створення репозиторію](#1-створення-репозиторію)
2. [Завантаження файлів](#2-завантаження-файлів)
3. [Активування GitHub Pages](#3-активування-github-pages)
4. [Налаштування користувацького домену](#4-налаштування-користувацького-домену)

---

## 1️⃣ Створення репозиторію

### Крок 1: Створіть новий репозиторій на GitHub

1. Перейдіть на https://github.com/new
2. Заповніть поля:
   - **Repository name:** `git-guide` (або будь-яка інша назва)
   - **Description:** "Практичний посібник з Git | Educational guide to Git version control"
   - **Visibility:** Публічний (Public)
   - ☑️ Виберіть "Add a README file"
   - ☑️ Виберіть ліцензію: MIT License

3. Натисніть **Create repository**

### Крок 2: Клонуйте репозиторій на ваш ПК

```bash
git clone https://github.com/YOUR_USERNAME/git-guide.git
cd git-guide
```

---

## 2️⃣ Завантаження файлів

### Крок 1: Скопіюйте файли до папки

Скопіюйте наступні файли у папку `git-guide`:
- `index.html` - основна веб-сторінка
- `README.md` - описання проекту

Папка повинна мати таку структуру:
```
git-guide/
├── index.html
├── README.md
└── .git/
```

### Крок 2: Закомітьте та завантажте файли

```bash
# Додайте всі файли до git
git add .

# Зробіть commit
git commit -m "Initial commit: Add Git guide webpage and documentation"

# Завантажте на GitHub
git push origin main
```

> Якщо використовується гілка `master` замість `main`:
> ```bash
> git push origin master
> ```

---

## 3️⃣ Активування GitHub Pages

### Крок 1: Перейдіть до налаштувань репозиторію

1. На GitHub перейдіть до вашого репозиторію
2. Натисніть **Settings** (⚙️)
3. Виберіть **Pages** у лівому меню (розділ "Code and automation")

### Крок 2: Налаштуйте GitHub Pages

1. Розділ **Source:**
   - **Deploy from a branch** (обраний за замовчуванням)
   
2. Виберіть гілку та папку:
   - **Branch:** `main` (або `master`, залежно від вашої конфігурації)
   - **Folder:** `/ (root)`
   
3. Натисніть **Save**

### Крок 3: Чекайте активування

- GitHub почне будувати вашу сторінку
- Зачекайте 1-2 хвилини
- Ви бачитимете зеленого значка ✅ коли готово
- Посилання на вашу сторінку буде видно в розділі Pages:
  - `https://YOUR_USERNAME.github.io/git-guide/`

---

## 4️⃣ Налаштування користувацького домену

Це **опціональний** крок для тих, хто хоче використовувати власний домен вместо `github.io`

### Метод 1: Використання Freenom (Безплатні домени)

#### На Freenom (freenom.com)

1. Перейдіть на https://www.freenom.com
2. Пошукайте безплатний домен (.tk, .ml, .ga, .cf)
3. Виберіть домен на 12 місяців (безплатно)
4. Зареєструйтеся або ввійдіть
5. Дотримуйтесь інструкцій реєстрації

#### DNS налаштування на Freenom

1. Перейдіть в **My Domains** > **Manage Domain**
2. Виберіть **Nameservers**
3. Виберіть **Use custom nameservers**
4. Введіть GitHub nameservers:
   - `ns1.github.io`
   - `ns2.github.io`
   - `ns3.github.io`
   - `ns4.github.io`

> GitHub для свідомих користувачів також пропонує використовувати їхні IP-адреси замість nameservers

### Метод 2: Платні домени (Namecheap, Google Domains)

#### На Namecheap

1. Придбайте домен
2. Перейдіть до **Dashboard** > **Domain List**
3. Натисніть **Manage** біля доменом
4. Перейдіть у **Advanced DNS**
5. Додайте наступні записи:

**Для поддержки `www.yourdomain.com`:**

| Type | Host | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOUR_USERNAME.github.io |

### Метод 3: Крок на GitHub

1. Повертайтесь до GitHub репозиторію
2. Перейдіть **Settings** > **Pages**
3. У розділі **Custom domain** введіть ваш домен:
   - `yourdomain.com`
4. Натисніть **Save**
5. Виберіть ☑️ **Enforce HTTPS** (рекомендується)

### Крок 4: CNAME файл

GitHub автоматично створює файл `CNAME` на вашому репозиторію. Якщо ні, створіть його вручну:

1. Натисніть **Add file** > **Create new file** на GitHub
2. Назвіть файл: `CNAME`
3. Введіть вміст:
   ```
   yourdomain.com
   ```
4. Зробіть **Commit**

### Крок 5: Тестування

- Чекайте 24-48 годин для повного поширення DNS записів
- Протестуйте за адресою: `https://yourdomain.com`
- Та `https://www.yourdomain.com`

---

## ✅ Контрольний список

- [ ] Репозиторій створений на GitHub
- [ ] Файли скопійовані (index.html, README.md)
- [ ] Файли закомічені та завантажені (git push)
- [ ] GitHub Pages активований
- [ ] Сторінка доступна за адресою `https://YOUR_USERNAME.github.io/git-guide/`
- [ ] (Опціонально) Користувацький домен налаштований
- [ ] (Опціонально) HTTPS активований

---

## 🐛 Розв'язання проблем

### Сторінка не завантажується

1. Перевірте, чи файл **index.html** знаходиться в корені репозиторію
2. Переглядіть логи в розділі **Settings** > **Pages**
3. Очистіть кеш браузера (Ctrl+Shift+Delete або Cmd+Shift+Delete)

### GitHub Pages показує помилку 404

1. Перевірте ім'я репозиторію в URL
2. Правильна адреса: `https://USERNAME.github.io/REPO_NAME/`
3. Переконайтеся, що репозиторій **публічний**

### Користувацький домен не працює

1. Перевірте DNS записи: https://mxtoolbox.com (для перевірки A записів)
2. Дайте DNS записам час на поширення (до 48 годин)
3. Переконайтеся, що файл CNAME присутній у репозиторії
4. Спробуйте відключити та включити HTTPS знову

---

## 📚 Додаткові ресурси

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Custom Domain Setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [Freenom Free Domain Registration](https://www.freenom.com)
- [Namecheap Domain Registration](https://www.namecheap.com)

---

## 🎓 Готово!

Після виконання цих кроків ваш Git-гайд буде доступний в інтернеті! 🎉

- **GitHub Pages URL:** `https://YOUR_USERNAME.github.io/git-guide/`
- **Користувацький домен:** `https://yourdomain.com` (якщо налаштований)

Успіхів! 🚀