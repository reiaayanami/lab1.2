# 📋 Посібник для Виконання Завдання з Git

## 📌 Вимоги Завдання

```
1. Підготувати веб-сторінку опрацювання теми Git
2. Посилання прикріпити у завдання

3б. Посилання на новий репозиторій GitHub
4б. Посилання на сторінку репозиторію (Markdown README)
5б. Посилання на веб-сторінку на GitHub Pages
5б+5б. Посилання на веб-сторінку з налаштованим стороннім доменом
```

---

## ✅ Чек-лист виконання

### 1️⃣ **Основна вимога: Веб-сторінка про Git**

Файл: **`index.html`** ✓ ГОТОВО

**Містить:**
- ✅ Короткі відомості про системи контролю версій та Git
- ✅ Основні можливості та переваги Git (6 преваг в карточках)
- ✅ 10 базових команд Git з коментарями:
  1. `git init`
  2. `git clone`
  3. `git add`
  4. `git commit`
  5. `git push`
  6. `git pull`
  7. `git branch`
  8. `git checkout`
  9. `git merge`
  10. `git status`
- ✅ Интерактивний сертифікат курсу
- ✅ Джерела інформації (6 посилань на офіційні ресурси)
- ✅ Адаптивний дизайн (мобільні пристрої підтримуються)
- ✅ Плавна навігація та приємний визуальний стиль

---

## 🚀 Крок 1: Створення GitHub репозиторію (3б)

### На GitHub:

1. Перейдіть на https://github.com/new
2. Заповніть:
   - **Repository name:** `git-guide`
   - **Description:** "Практичний посібник з Git | Educational guide to Git version control"
   - **Public:** ☑️
   - **Add README:** ☑️ (виберіть MIT License)

3. **Create repository**

### Локально:

```bash
# Клонуйте репозиторій
git clone https://github.com/YOUR_USERNAME/git-guide.git
cd git-guide

# Завантажте файли
# Скопіюйте: index.html, README.md, LICENSE, .gitignore

# Закомітьте
git add .
git commit -m "Initial commit: Add Git guide"
git push origin main
```

**Посилання для завдання (3б):**
```
https://github.com/YOUR_USERNAME/git-guide
```

---

## 📄 Крок 2: Markdown README (4б)

### Файл: **`README.md`** ✓ ГОТОВО

**Містить:**
- ✅ Заголовок та опис проекту
- ✅ Таблиця змісту
- ✅ Інформацію про проект
- ✅ Функціональність сторінки
- ✅ Структуру репозиторію
- ✅ Інструкції встановлення
- ✅ 10 команд Git у форматі таблиці
- ✅ Посилання на джерела
- ✅ Інформацію про ліцензію та автора

**Посилання для завдання (4б):**
```
https://github.com/YOUR_USERNAME/git-guide/blob/main/README.md
```

---

## 🌐 Крок 3: GitHub Pages (5б)

### На GitHub:

1. Перейдіть до репозиторію
2. **Settings** (⚙️) > **Pages**
3. **Source:**
   - Branch: `main`
   - Folder: `/ (root)`
4. **Save**
5. Чекайте активування (1-2 хвилини)

### Перевірка:

Ваша сторінка буде доступна за адресою:
```
https://YOUR_USERNAME.github.io/git-guide/
```

**Посилання для завдання (5б):**
```
https://YOUR_USERNAME.github.io/git-guide/
```

---

## 🌍 Крок 4: Користувацький домен (5б+5б)

### Варіант А: Безплатний домен (Freenom)

**Крок 1: Реєстрація домену**

1. Перейдіть https://www.freenom.com
2. Пошукайте домен (наприклад: `gitguide.tk`)
3. Виберіть 12 місяців (безплатно)
4. Реєструйтесь та активуйте

**Крок 2: DNS Nameservers**

1. **My Domains** > **Manage Domain**
2. **Management Tools** > **Nameservers**
3. **Use custom nameservers:**
   ```
   ns1.github.io
   ns2.github.io
   ns3.github.io
   ns4.github.io
   ```

**Крок 3: GitHub налаштування**

1. GitHub Settings > Pages
2. **Custom domain:** `gitguide.tk`
3. **Save**
4. Виберіть ☑️ **Enforce HTTPS**
5. Система автоматично створить CNAME

### Варіант Б: Платний домен (Namecheap, Google Domains)

**Крок 1: DNS записи на Namecheap**

| Type | Host | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOUR_USERNAME.github.io |

**Крок 2: GitHub налаштування**

1. GitHub Settings > Pages
2. **Custom domain:** `yourdomain.com`
3. **Save** і ☑️ **Enforce HTTPS**

**Крок 3: CNAME файл**

GitHub створить автоматично, або створіть вручну:

```bash
echo "yourdomain.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

### Тестування

```bash
# Чекайте 24-48 годин
# Потім тестуйте:
# https://yourdomain.com
# https://www.yourdomain.com
```

**Посилання для завдання (5б+5б):**
```
https://yourdomain.com
```

---

## 📊 Структура файлів для репозиторію

```
git-guide/
├── index.html                    # Основна сторінка (задача)
├── README.md                     # Markdown документація (4б)
├── LICENSE                       # MIT License
├── .gitignore                    # Git ignore файл
└── GITHUB_PAGES_SETUP.md        # Детальна інструкція GitHub Pages
```

---

## 📝 Шаблон відповіді для завдання

Скопіюйте та заповніть:

```markdown
## Завдання: Git - Веб-сторінка та GitHub Pages

### Основна вимога:
Веб-сторінка про Git: **[посилання на ваш GitHub Pages]**

---

### 3 бали: Репозиторій GitHub
- Посилання: https://github.com/YOUR_USERNAME/git-guide
- Статус: ✅ Готово
- Вміст: index.html, README.md, LICENSE

---

### 4 бали: Markdown README
- Посилання: https://github.com/YOUR_USERNAME/git-guide/blob/main/README.md
- Статус: ✅ Готово
- Містить: Описання, 10 команд, посилання, інформацію про автора

---

### 5 балів: GitHub Pages
- Посилання: https://YOUR_USERNAME.github.io/git-guide/
- Статус: ✅ Активовано
- Содержит: Інтерактивна веб-сторінка

---

### 5б+5б: Користувацький домен (ОПЦІОНАЛЬНО)
- Домен: yourdomain.com
- Посилання: https://yourdomain.com
- Статус: ✅ Налаштовано
- DNS провідер: Freenom / Namecheap / тощо
```

---

## 🎯 Резюме кроків

1. ✅ Скопіюйте файли (index.html, README.md, LICENSE, .gitignore)
2. ✅ Створіть репозиторій на GitHub
3. ✅ Завантажте файли (`git push`)
4. ✅ Активуйте GitHub Pages
5. ✅ (Опціонально) Налаштуйте користувацький домен
6. ✅ Приєднайте посилання до завдання

---

## 🆘 Швидка допомога

### Проблема: Сторінка не завантажується

```bash
# Перевірте структуру репозиторію
git status

# Переконайтеся що index.html в корені
ls -la

# Перепушьте файли
git add .
git commit -m "Fix: Ensure files are at root"
git push origin main
```

### Проблема: GitHub Pages не активується

1. Перевірте репозиторій - повинен бути **публічним**
2. Перейдіть Settings > Pages і переконайтеся в налаштуваннях
3. Очистіть кеш браузера та перезавантажте

### Проблема: Користувацький домен не працює

1. Перевірте DNS записи: https://mxtoolbox.com
2. Дайте часу на поширення (до 48 годин)
3. Переконайтеся що файл CNAME є в репозиторії

---

## 📞 Контакти для допомоги

- 📚 GitHub Docs: https://docs.github.com/en/pages
- 🎓 Git Book: https://git-scm.com/book/uk/v2
- 💬 Telegram: [@makoto699](https://t.me/makoto699)

---

**Успіхів з завданням!** 🚀

Всі файли готові до використання. Просто скопіюйте їх та підставте ваше ім'я користувача GitHub!
