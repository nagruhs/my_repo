
[![icon](logo.png)](https://git-scm.com "перейти на сайт")

# Инструкция для работы с Git и удалёнными репозиториями 

## Краткий список основных команд git:
-----------------
* `git config --global user.name` - ввод имени пользователя
* `git config --global user.email` - ввод e-mail адреса пользователя
* `git --version` - просмотр установленной версии git
* `git config --list` - показать текущие настройки git
* `git init` - инициализация нового репозитория  git
* `git status` - выводит на экран текущий статус  git
* `git add <имя файла>` - переносит ожидающие изменения из рабочего каталога в раздел проиндексированных файлов
   * `git add .` -  то же для всех файлов в каталоге
   *  `git rm --cached ＜имя файла＞` - удалить файл из отслеживаемых
* `git commit -m <сообщение к коммиту>` -mфиксирует и сохраняет состояние файла с нашим комментарием
   * `git commit -am <сообщение к коммиту>` - выполняет *git add* и *git commit* для отслеживаемых файлов
   * `git commit --amend -m <сообщение к коммиту>` - редактирование последнего сообщения к коммиту
* `git log` -  просмотр истории коммитов
   * `git log --help` - справка по *git log*
   * `git log --graph` - представление лога в графическом виде
   * `git log -p` - лог с подробными изменениями
* `git checkout <номер коммита>`- позволяет переключаться между коммитами
* `git diff` - выводит список изменений между текущим состоянием и последним коммитом
* `git branch` - показать существующие ветки
  * `git branch <имя ветки>` - создание ветки
  * `git branch -d <имя ветки>` - удаление ветки
* `git checkout ＜имя ветки＞` - переход на ветку
  * `git checkout -b ＜имя ветки＞` - создание ветки и переключение на нее
  * `git checkout --<имя файла>` - возвращает файл к состоянию предыдущего сохранения
* `git merge ＜имя ветки＞` - слияние ветки с текущей
  * `git merge --abort` - отменяет процесс слияния

#### Для подключения удаленного репозитория см. подсказку на github [https://github.com/](https://github.com/ "Ссылка на github").

* `git clone <адрес>` - клонировать удаленный репозиторий
* `git push` - отправить изменения в удаленный репозиторий
* `git pull` - скачать изменения из удаленного репозитория (также эта команда мерджит ветки)

#### Для работы с чужим репозиторием на github:
1. Делаем **fork** интересующего репозитория.
2. Выполняем `git clone`.
3. Создаем новую ветку.
4. Производим изменения в этой ветке и делаем коммит.
5. Выполняем `git push`.
6. В окне на github отправляем **pull request**.
------------