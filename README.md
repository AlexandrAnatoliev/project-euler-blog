<div align="center">
  <a id="russian"></a>
  <h1>Добро пожаловать в Project-Euler-Blog</h1>

  <p>Данный проект - это сборник статей для моего блога</p>

  [![EN](https://img.shields.io/badge/English-🇬🇧-blue)](#english)
  [![RU](https://img.shields.io/badge/Русский-🇷🇺-red)](#russian)
  ![Version 0.3.6](https://img.shields.io/badge/Version-0.3.6-orange.svg)
  ![Stars](https://img.shields.io/github/stars/AlexandrAnatoliev/project-euler-blog.svg?style=flat)
  ![Forks](https://img.shields.io/github/forks/AlexandrAnatoliev/project-euler-blog.svg?style=flat)
  [![PRs Welcome](https://img.shields.io/badge/PR:s-welcome-brightgreen.svg)](https://github.com/AlexandrAnatoliev/project-euler-blog/pulls)
  [![First Contributors](https://img.shields.io/badge/first-contributors-brightgreen.svg)](https://github.com/AlexandrAnatoliev/project-euler-blog/pulls)
  ![GitHub repo size](https://img.shields.io/github/repo-size/AlexandrAnatoliev/project-euler-blog)
</div>

  > **Author:** Alexandr Anatoliev

  > **GitHub:** [AlexandrAnatoliev](https://github.com/AlexandrAnatoliev)

---

<div align="center">
  <h3>Клонирование репозитория</h3>
</div>

CSS-настройки для блога выделены в отдельный репозиторий, что позволяет
использовать их повторно в разных проектах и избавляет от необходимости
вносить одни и те же изменения в каждый проект.

* Поэтому при клонировании репозитория использовать флаг --recursive
```
git clone --recursive https://github.com/AlexandrAnatoliev/project-euler-blog.git
```

* Или так
```
# Обычное клонирование — папка src/styles будет пустой!
git clone https://github.com/AlexandrAnatoliev/project-euler-blog.git
cd project-euler-blog
ls src/styles/  # пусто или не существует

# Нужно инициализировать и обновить подмодули
git submodule init    # инициализирует подмодули из .gitmodules
git submodule update  # загружает актуальные файлы
```

<div align="center">
  <h3>Обновление подмодуля до последней версии</h3>
</div>

```
# Перейти в папку подмодуля
cd src/styles

# Обновиться до последнего коммита в ветке main
git checkout main
git pull

# Вернуться в основной репозиторий
cd ../..

# Зафиксировать изменение (новую ссылку на коммит)
git add src/styles
git commit -m "Update project-euler-css to latest version"
```

