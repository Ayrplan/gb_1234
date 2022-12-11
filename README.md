# gb_1234
# Инструкция для работы с Markdown и Git

## Синтаксис. (Часть 1)
### Заголовок - чтобы сделать заголовки в Markdown необходим символ #, он же решётка, он же хеш. Уровень заголовка определяется количеством решёток в нём, всего их может быть шесть.
### Выделение текста - чтобы выделить текст курсивом, необходимо обрамить его звездочками(*) или знаком нижнего подчеркивания(_). 
Напимер, *вот так* или _вот так_

Чтобы выделить текст полужирным, необходимо обрамить его двойными звездочками.(**) или двойным знаком нижнего подчеркивания(__) 
Например, **вот так** или __вот так__

Альтернативные способы выделения жирным или курсивом нужны для того чтобы мы могла совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом быть **полужирным**_.
### Цитаты
> Чтобы выделить какой то абзац как цитату, необходимо знак > проставлять перед каждой сторочкой цитаты. 
>
>Дед Мороз.

### Списки - чтобы добавить ненумерованные списки, необходимо пункты выделить звездочкой (*) или знаком (+).

Например, вот так:
* Элемент 1
* Элемент 2 
* Элемент 3 
+ Элемент 4

### Работа с изображением - чтобы вставить изображение в текст, достаточно написать следуюющее:
![Привет, это я](image159-18.jpg)

### Ссылки - для вставки ссылки необходимо написать следующее:
[yandex.ru/games](https://yandex.ru/games/?utm_source=dzen&utm_medium=icon&utm_campaign=mainpage)

### Чтобы добавить нумерованные списки, необходимо пункты просто пронумеровать.

1.
2.
3.

### Список дел - для обозначения списка дел используется:
- [ ] Невыполненная задача
- [ ] Невыполненная задача
- [X] Выполненная задача

## Синтаксис (Часть 2)

### Команды: 

* git init - Инициализирует новый репозиторий Git;
* git add - Переносит изменения из рабочего каталога в раздел проиндексированных файлов. В этом разделе можно подготовить снимок состояния, прежде чем сделать коммит изменений в официальную историю;
* git branch - С ее помощью можно создавать изолированные среды разработки в одном репозитории;
* git checkout - С командой git checkout можно не только получать старые коммиты и прежние версии файлов, но и осуществлять навигацию по существующим веткам. В сочетании с базовыми командами Git она позволяет сосредоточиться на определенном направлении разработки;
* git clean - Удаляет неотслеживаемые файлы из рабочего каталога. Это логический аналог команды git reset, которая (обычно) работает только с отслеживаемыми файлами;
* git clone - Создает копию существующего репозитория Git. Клонирование — самый распространенный способ, с помощью которого разработчики могут получить рабочую копию центрального репозитория;
* git commit - Получает проиндексированный снимок состояния и выполняет его коммит в историю проекта; Эта команда в сочетании с командой git add определяет классический рабочий процесс для всех пользователей Git;
* git commit --amend - Команда git commit с флагом --amend позволяет внести изменения в последний коммит. Она может оказаться полезной, если вы забыли проиндексировать файл или не указали важную информацию в комментарии к коммиту.
* git config - Удобный способ для настройки параметров конфигурации в инсталляции Git.
* git fetch - С помощью команды извлечения можно загрузить ветку из другого репозитория вместе со всеми связанными с ней коммитами и файлами, однако при этом изменения не будут интегрированы в локальный репозиторий. Благодаря этому вы сможете проверить изменения перед слиянием с проектом.
* git log - Позволяет изучить предыдущие версии проекта.
* git merge - способ интеграции изменений из разошедшихся веток. После разветвления истории проекта командой git branch можно использовать команду git merge, чтобы объединить отдельные ветки.
* git pull - Команда git pull — это автоматизированная версия команды git fetch. Она загружает ветку из удаленного репозитория и сразу же объединяет ее с текущей веткой. Эта команда представляет собой git-эквивалент команды svn update.
* git push - Команда git push противоположна команде извлечения (с некоторыми оговорками). С ее помощью можно перенести локальную ветку в другой репозиторий и без труда опубликовать поступивший код. Эта команда похожа на svn commit с тем исключением, что она отправляет не один набор изменений, а серию коммитов.
* git rebase - С помощью команды перебазирования можно переместить ветки и избежать ненужных коммитов слияния. Полученную линейную историю зачастую намного легче понять и изучить.
* git rebase -i - С помощью флага -i можно запустить перебазирование в интерактивном режиме. При этом сохраняются все преимущества обычного перебазирования и появляется возможность добавлять, редактировать или удалять коммиты по ходу операции.
* git reflog - Git отслеживает изменения в конце веток с помощью механизма журналов ссылок (reflog). Он позволяет вернуться к наборам изменений, даже если на них не ссылается никакая ветка или тег.
* git remote - С его помощью вместо полного URL-адреса в командах fetch, pull и push можно использовать более удобное сокращение.
* git reset - Отменяет изменения в файлах в рабочем каталоге. Эта команда сброса позволяет очистить или полностью удалить изменения, которые не были отправлены в публичный репозиторий.
* git revert - Отменяет коммит снимка состояния. Если вы обнаружили ошибочный коммит, его можно легко и безопасно удалить из базы кода с помощью команды git revert.
* git status - Показывает состояние рабочего каталога и проиндексированного снимка состояния. Эту команду можно выполнять в сочетании с git add и git commit, чтобы узнать, что именно будет включено в следующий снимок.
* git ignore - .gitignore используется для того, чтобы определить, какие файлы и папки не нужно добавлять в git репозиторий.

Работа на GitHub

1. Создать аккаунт на GitHub;
2. Cоздать локальный репозиторий;
3. Подружить локальный и удаленный репозитории(есть подсказка)
4. Отправить (push) со своего локального на удаленный репозиторий с возможной авторизацией;
5. Прровести изменения с другого компьютера;
6. Выкачать (pull) актуальное состояние из удалённого репозитория.