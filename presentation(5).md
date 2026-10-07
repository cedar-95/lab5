---
marp: true
theme: default
paginate: true
footer: 'Лабораторная работа №5 · НПИбд-03-25, Чжу Ино'
style: |
  section {
    font-family: "Times New Roman", serif;
    font-size: 24px;
    padding: 50px 70px;
    line-height: 1.5;
    color: #1a1a1a;
  }
  h1 {
    font-size: 38px;
    color: #003366;
    border-bottom: 3px solid #003366;
    padding-bottom: 10px;
    margin-bottom: 20px;
  }
  h2 {
    font-size: 30px;
    color: #003366;
    margin-bottom: 15px;
  }
  ul {
    margin-top: 10px;
  }
  li {
    margin-bottom: 8px;
  }
  section.lead {
    text-align: center;
    justify-content: center;
  }
  section.lead h1 {
    border: none;
    font-size: 46px;
    margin-bottom: 40px;
  }
  section.lead p {
    font-size: 26px;
    margin: 6px 0;
  }
  section.chapter {
    text-align: center;
    justify-content: center;
    background: #f4f7fb;
  }
  section.chapter h1 {
    border: none;
    font-size: 44px;
  }
  footer {
    font-size: 14px;
    color: #666;
  }
---

<!-- _class: lead -->

# Лабораторная работа №5. Управление конфигурационными файлами с помощью chezmoi

НПИбд-03-25, Чжу Ино

---

# Содержание

1. Титульный слайд
2. Введение
3. Инициализация Git-репозитория для dotfiles
4. Создание удалённого репозитория на GitHub
5. Восстановление конфигурации
6. Заключение
7. Список литературы

---

<!-- _class: chapter -->

# 1. Титульный слайд

---

- Лабораторная работа №5
- Управление конфигурационными файлами с помощью chezmoi
- НПИбд-03-25
- Чжу Ино

---

<!-- _class: chapter -->

# 2. Введение

---

- Изучение инструмента chezmoi
- Управление dotfiles
- Синхронизация через GitHub

---

<!-- _class: chapter -->

# 3. Инициализация Git-репозитория для dotfiles

---

- Переход в каталог chezmoi: `chezmoi cd`
- Инициализация: `git init`
- Добавление файлов: `git add .`
- Первый коммит: `git commit -m "Initial commit of dotfiles"`

---

<!-- _class: chapter -->

# 4. Создание удалённого репозитория на GitHub

---

- Создание репозитория `dotfiles` на GitHub
- Подключение: `git remote add origin <URL>`
- Отправка: `git push -u origin main`

---

<!-- _class: chapter -->

# 5. Восстановление конфигурации

---

- Команда: `chezmoi init --apply cedar-95`
- Проверка: `cat ~/.test_alias`
- Результат: `alias ll='ls -la'`, `alias gs='git status'`

---

<!-- _class: chapter -->

# 6. Заключение

---

- Освоены команды `chezmoi init`, `chezmoi add`, `chezmoi apply`, `chezmoi diff`
- Создан репозиторий dotfiles на GitHub
- Протестировано восстановление конфигурации

---

<!-- _class: chapter -->

# 7. Список литературы

---

1. Neil N. J. Learning CentOS: A Beginners Guide to Learning Linux. — CreateSpace Independent Publishing Platform, 2016.
2. Vugt S. van. Red Hat RHCSA/RHCE 7 cert guide. — Pearson IT Certification, 2016.
3. Unix и Linux: руководство системного администратора / Э. Немет и др. — 5-е изд. — СПб. : ООО «Диалектика», 2020.