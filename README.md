<div align="center">
  <a id="russian"></a>
  <h1>Добро пожаловать в Project-Euler-Blog</h1>

  <p>Данный проект - это сборник статей для моего блога</p>

  [![EN](https://img.shields.io/badge/English-🇬🇧-blue)](#english)
  [![RU](https://img.shields.io/badge/Русский-🇷🇺-red)](#russian)
  ![Version 0.4.1](https://img.shields.io/badge/Version-0.4.1-orange.svg)
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
  <h3>Навигация</h3>
</div>

* [Клонирование репозитория](#clone-repo-ru)
* [Обновление подмодуля до последней версии](#update-submodule-ru)
* [Для контрибьютеров](#contributing-ru)
* [Похожие проекты](#influences-ru)
* [Контакты](#contact-ru)
* [Список контрибьютеров](#list-of-contributors-ru)

---

<div align="center">
  <a id="clone-repo-ru"></a>
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
  <a id="update-submodule-ru"></a>
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

---

<div align="center">
  <a id="contributing-ru"></a>
  <h3>Для контрибьютеров</h3>
</div>

<div align="center">
  <h4>Инструкции по Установке</h4>
</div>

1. Сделайте "форк" этого репозитория нажатием 
  кнопки "Fork" в правом верхнем углу страницы.
  Это создаст копию репозитория на Вашем GitHub 
  аккаунте.

2. Клонируйте Ваш "форкнутый" репозиторий нажатием
  кнопки "Code":

Откроется маленькое окно: 

Скопируйте из него URL и выполните на своем 
компьютере команду:

```bash
git clone --recursive https://github.com/<your-username>/project-euler-blog.git
```

3. Перейдите в папку с проектом:

```bash
cd project-euler-blog
```

4. Добавьте ссылку на оригинальный репозиторий
  для будущих обновлений:

```bash
git remote add upstream https://github.com/AlexandrAnatoliev/project-euler-blog.git
```

(Напомню, здесь должен быть URL оригинального
репозитория, а не "форкнутого" Вами, так что
username в нем должно быть `AlexandrAnatoliev`,
а не Ваш собственный username.)

5. Проверьте ремоуты для своего репозитория:

```bash
git remote -v
```

Вы должны увидеть origin (создается автоматически
при клонировании) и upstream ремоуты: 

``` 
origin  https://github.com/<your-username>/project-euler-blog.git (fetch)
origin  https://github.com/<your-username>/project-euler-blog.git (push)
upstream        https://github.com/AlexandrAnatoliev/project-euler-blog.git (fetch)
upstream        https://github.com/AlexandrAnatoliev/project-euler-blog.git (push)
```

6. Выполните pull из upstream репозитория в Вашу
  master ветку, чтобы синхронизировать ее с основным
  проектом:

```bash
git pull upstream master
```

7. Создайте новую ветку командой:

```bash
git switch -c fix-issue
```

Сейчас вы готовы начать работать с issue!
Помните, каждый раз сначала делать pull
из upstream репозитория, чтобы держать содержимое
Вашего локального репозитория в соответствии
с главным проектом.

_Примечание: Рекомендую всегда создавать новую
ветвь для каждого issue, который вы выполняете!
Иначе pull request будут слишком большими и 
возможно возникнут конфликты слияния._

---

<div align="center">
  <a id="submitting-your-changes-ru"></a>
  <h4>Отправка Ваших изменений</h4>
</div>

После того как вы решили проблему, вы готовы отправить 
изменения! 

1. Добавьте Ваши изменения в отслеживание:

```bash
git add файлы-которые-вы-изменили
```

2. Сделайте коммит:

```bash
git commit -m "Fixed issue"
```

3. Отправить изменения в Ваш "форкнутый" репозиторий:

```bash
git push origin fix-issue
```

После того как вы отправили Ваши изменения на 
GitHub, вы готовы создать pull request.
Перейдите на Ваш "форк" репозитория на GitHub.

- Вы увидите надпись "fix-issue had recent pushes" 
(или как Ваша ветка называется) и кнопку 
"Compare & pull request" на ней.

- Нажмите кнопку "Compare & pull request" и перейдете
на страницу pull request оригинального репозитория
проекта project-euler-blog.

- Заполните поля title и description подробностями
о задаче и Вашем ее решении. Вы можете также добавить
иную информацию, такую как скриншоты, если хотите.

- В конце нажмите кнопку "Create pull request" 
чтобы закончить создание pull request.

Поздравляю, вы сделали свой вклад в open 
source на GitHub!

Можете расслабиться и подождать пока не сделают
ревью Вашего кода. Если все хорошо, Ваш pull request
вольют в основную ветку. Если нет, Вам будет 
предложено внести изменения в Ваш код.

Помните, что нужно подождать ревью Вашего pull 
request, не закрывайте его сами.
Если Вас просят сделать изменения, вы можете
коммитить их в ту же самую ветвь, не нужно
закрывать текущий pull request и открывать новый.

---

<div align="center">
  <a id="influences-ru"></a>
  <h3>Похожие проекты</h3>
</div>

Этот проект вдохновлялся несколькими хорошими
проектами, созданными с целью помочь новичкам
сделать свой первый вклад в open source.

- [Fork, Commit, Merge](https://github.com/fork-commit-merge/fork-commit-merge): 
Проект созданный чтобы помочь Вам познакомиться
с процессом вклада в open source на GitHub,
а также помочь освоить базы программирования на
различных языках, библиотеках и фреймворках.

- [Polyglot-Calculators](https://github.com/B3rou/Polyglot-Calculators): 
Polyglot-Calculators управляемый сообществом современный гибридный проект, 
который демонстрирует, как математические калькуляторы  и алгоритмы реализуются
на разных языках программирования.

Я очень рекомендую посмотреть эти проекты!

---

<div align="center">
  <a id="contact-ru"></a>
  <h3>Контакты</h3>
</div>

Столкнувшись с затруднениями, не стесняйтесь
открыть issue, написать в
[Discussions](https://github.com/AlexandrAnatoliev/project-euler-blog/discussions/14)
или мне на почту per-1986@list.ru.

---

<div align="center">
  <a id="list-of-contributors-ru"></a>
  <h3>Список Контрибьютеров</h3>
</div>

Огромное спасибо всем, кто внес вклад в этот проект!

<a href="https://github.com/AlexandrAnatoliev"><img src="https://images.weserv.nl/?url=https://avatars.githubusercontent.com/u/116306656?v=4&h=300&w=300&fit=cover&mask=circle&maxage=7d" width="80px"/></a>

