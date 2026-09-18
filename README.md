# 🔀 Git - Практичний Посібник

[![Статус: Завершено](https://img.shields.io/badge/Статус-Завершено-brightgreen)](https://github.com)
[![Ліцензія: MIT](https://img.shields.io/badge/Ліцензія-MIT-blue)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Active-success)](https://github.com)

Комплексний посібник з вивчення системи контролю версій **Git**. Проект містить детальну веб-сторінку з інформацією про Git, його переваги та 10 базових команд для початківців.

## 📚 Зміст

- [Про проект](#про-проект)
- [Функціональність](#функціональність)
- [Структура репозиторію](#структура-репозиторію)
- [Встановлення](#встановлення)
- [Використання](#використання)
- [GitHub Pages](#github-pages)
- [Команди Git](#команди-git)
- [Джерела](#джерела)
- [Автор](#автор)

## 🎯 Про проект

Це освітній проект, розроблений для вивчення та розуміння основ системи контролю версій **Git**. Проект включає:

✅ Вступ до систем контролю версій  
✅ Історію та розвиток Git  
✅ 10 базових команд Git з прикладами  
✅ Переваги використання Git  
✅ Інтерактивний сертифікат  
✅ Посилання на перевірені джерела  
✅ Адаптивний дизайн для мобільних пристроїв

## 🚀 Функціональність

### Веб-сторінка включає:

- **Інформація про VCS** - поняття систем контролю версій
- **Про Git** - історія створення та основні характеристики
- **Переваги Git** - 6 ключових переваг з карточками
- **10 Базових Команд** - детальний опис кожної команди:
  - `git init`
  - `git clone`
  - `git add`
  - `git commit`
  - `git push`
  - `git pull`
  - `git branch`
  - `git checkout`
  - `git merge`
  - `git status`

- **Навіщики** - корисні команди (log, diff, reset, tag)
- **Сертифікат** - інтерактивний сертифікат з поточною датою
- **Джерела** - посилання на офіційні та перевірені ресурси

## 📁 Структура репозиторію

```
git-guide/
├── index.html          # Основна веб-сторінка
├── README.md          # Цей файл
├── LICENSE            # Ліцензія MIT
└── assets/            # Папка для медіа-файлів (якщо потрібно)
```

## 💻 Встановлення

### Локально

1. **Клонуйте репозиторій:**
```bash
git clone https://github.com/ВАШ-USERNAME/git-guide.git
cd git-guide
```

2. **Відкрийте сторінку в браузері:**
```bash
# На Windows
start index.html

# На macOS
open index.html

# На Linux
xdg-open index.html
```

Або скористайтеся локальним сервером:
```bash
# Python 3
python -m http.server 8000

# Node.js (http-server)
npx http-server
```

Потім відкрийте `http://localhost:8000` у браузері.

## 🌐 Використання

Веб-сторінка містить:
- **Навігаційне меню** для швидкого переходу до секцій
- **Інтерактивні посилання** на джерела
- **Адаптивний дизайн** для всіх розмірів екранів
- **Стильована консоль** для команд Git
- **Темні теми** для зручного читання

Просто відкрийте `index.html` у будь-якому сучасному браузері.

## 🚀 GitHub Pages

### Активування GitHub Pages:

1. Перейдіть до **Settings** вашого репозиторію
2. Прокрутіть до **Pages** (в лівому меню)
3. У **Source** виберіть:
   - Branch: `main` (або `master`)
   - Folder: `/ (root)`
4. Натисніть **Save**
5. Ваша сторінка буде доступна за адресою:
   - `https://ВАШ-USERNAME.github.io/git-guide/`

### Налаштування користувацького домену (опціонально):

1. Придбайте домен у реєстратора (наприклад, Namecheap, Google Domains)
2. У **GitHub Pages** налаштуваннях введіть домен
3. Налаштуйте DNS записи у реєстраторі домену
4. Додайте CNAME файл у репозиторій:

```bash
echo "your-domain.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

## 📝 10 Команд Git

| Команда | Опис |
|---------|------|
| `git init` | Ініціалізувати новий репозиторій |
| `git clone <url>` | Клонувати існуючий репозиторій |
| `git add <файл>` | Додати файл до staging area |
| `git commit -m "msg"` | Зберегти снімок з повідомленням |
| `git push origin <гілка>` | Завантажити на сервер |
| `git pull origin <гілка>` | Завантажити з сервера |
| `git branch` | Показати список гілок |
| `git checkout <гілка>` | Переключитися на гілку |
| `git merge <гілка>` | Об'єднати гілку |
| `git status` | Показати поточний стан |

## 📚 Джерела

Проект використовує інформацію з наступних джерел:

- 📖 [Офіційна документація Git](https://git-scm.com/doc)
- 📕 [Git Book (укр.)](https://git-scm.com/book/uk/v2)
- 🎓 [GitHub Learning Lab](https://github.com/skills)
- 🏫 [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)
- 🎮 [Interactive Git Learning](https://learngitbranching.js.org/)
- 📚 [GitHub Guides](https://guides.github.com/)

## 🎓 Освітня цінність

Цей посібник розроблений для:
- ✅ Студентів, що починають вивчати Git
- ✅ Новичків у веб-розробці
- ✅ Людей, які хочуть зрозуміти основи контролю версій
- ✅ Професіоналів, що повторюють базові концепції

## 📄 Ліцензія

Цей проект ліцензований під [MIT License](LICENSE) - дивіться файл LICENSE для більш детальної інформації.

## 👤 Автор

**Rei (Yulia Gorbach)**
- 🎓 Студент Novovolynsk Electromechanical Professional College
- 💻 Frontend Developer & Designer
- 📍 Ukraine

## 🤝 Внесок

Рекомендації та поправки вітаються! Будь ласка:

1. **Fork** цей репозиторій
2. Створіть **feature гілку** (`git checkout -b feature/amazing-feature`)
3. Зробіть **commit** своїх змін (`git commit -m 'Add amazing feature'`)
4. **Push** на гілку (`git push origin feature/amazing-feature`)
5. Відкрийте **Pull Request**

## 📞 Контакти

- 📧 Email: [ваш-email@example.com]
- 💬 Telegram: [@makoto699](https://t.me/makoto699)
- 🐙 GitHub: [github.com/ваш-username](https://github.com)

---

<div align="center">

**⭐ Якщо вам сподобався цей проект, дайте йому зірку!**

Розроблено з ❤️ як освітній матеріал

</div>