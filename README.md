# Домашнее задание к занятию «Системы контроля версий»

### Цель задания

В результате выполнения задания вы: 

* научитесь подготоваливать новый репозиторий к работе;
* сохранять, перемещать и удалять файлы в системе контроля версий.  


### Чеклист готовности к домашнему заданию

1. Установлена консольная утилита для работы с Git.


### Инструкция к заданию

1. Домашнее задание выполните в GitHub-репозитории. 
2. В личном кабинете отправьте на проверку ссылку на ваш репозиторий с домашним заданием.
3. Любые вопросы по решению задач задавайте в чате учебной группы.


------

## Задание 1. Создать и настроить репозиторий для дальнейшей работы на курсе

В рамках курса вы будете писать скрипты и создавать конфигурации для различных систем, которые необходимо сохранять для будущего использования. 
Сначала надо создать и настроить локальный репозиторий, после чего добавить удалённый репозиторий на GitHub.


### РЕШЕНИЕ
### Создание репозитория и первого коммита

1. Зарегистрирован аккаунт на [https://github.com/]. 
2. Создан публичный репозиторий с названием devops-netology. Галочка Initialize this repository with a README установлена.
[Repo](https://github.com/sash3939/VCS_Git/assets/156709540/7515afbf-3f26-4792-beeb-2d165aa24dc7)

2. Создан авторизационный токен для клонирования репозитория.
[Token](https://github.com/sash3939/VCS_Git/assets/156709540/d7c5344d-4584-4c4d-9214-51443a0e650a)

3. Репозиторий склонирован, перешли в каталог devops-netology
[Clone](https://github.com/sash3939/VCS_Git/assets/156709540/0d5748a5-a85c-4052-968b-fe09ee53d02f)

4. Произвели первоначальную настройку Git
[Git](https://github.com/sash3939/VCS_Git/assets/156709540/0c0567a9-773f-4545-b3d0-d8629eae0566)
 
5. Результат команды git status.
[git status](https://github.com/sash3939/VCS_Git/assets/156709540/e49c31ce-66ff-4a7c-a29d-ec787b590458)

6. Отредактирован README.md и выполнена git status. Состояние modified.
[git status+modified](https://github.com/sash3939/VCS_Git/assets/156709540/76ed5b1a-1d47-4aa7-b37c-8979d9a19681)

7. Посмотрели изменения в файле README.md, выполнив команды git diff и git diff --staged
[git diff+ git diff --staged](https://github.com/sash3939/VCS_Git/assets/156709540/3f97290b-9748-4d7b-b2af-e0386a8dc30c)

8. Перевели файл в состояние staged командой git add README.md. И ещё раз выполнили команды git diff и git diff --staged
-git diff покажет изменения в рабочем дереве, которые ещё не были добавлены в индекс. Мы увидим, что была добавлена новая строка
-Добавим изменения в индекс и посмотрим git diff и git diff --staged
-git diff теперь не покажет никаких изменений, потому что все изменения в рабочем дереве были добавлены в индекс.
-А git diff --staged покажет изменения, которые были добавлены в индекс. Мы увидим ту же новую строку, добавленную в файл README.md

git diff показывает изменения в рабочем дереве, которые ещё не были добавлены в индекс.
git diff --staged показывает изменения, которые были добавлены в индекс, но ещё не закоммичены.

[staged README and git diff](https://github.com/sash3939/VCS_Git/assets/156709540/f70998c4-6443-4d0d-9c61-c2f99b65a829)

9. Сделали коммит git commit -m 'First commit'.
И ещё раз посмотрели выводы команд git status, git diff и git diff --staged
[First Commit](https://github.com/sash3939/VCS_Git/assets/156709540/42005d3a-6dbf-49e1-a924-ea46eaf936ec)


### Создание файлов `.gitignore` и второго коммита

1. Создан файл .gitignore, проверен его статус сразу после создания.
2. Добавьте файл `.gitignore` в следующий коммит (`git add...`).
[.gitignore+add](https://github.com/sash3939/VCS_Git/assets/156709540/ab035f62-7433-48ae-8a8d-5a3ae9716be3)

3. Создали соотвествующий каталог terraform и внутри этого каталога — файл .gitignore по примеру: https://github.com/github/gitignore/blob/master/Terraform.gitignore.
[terraform](https://github.com/sash3939/VCS_Git/assets/156709540/80b56449-1b93-476b-ab81-ba1c4c8fbc04)
[.gitignore](https://github.com/sash3939/VCS_Git/assets/156709540/c65c92f8-048d-47d1-9d2b-d7e292daa5a6)

4. В файле README.md описали своими словами, какие файлы будут проигнорированы в будущем благодаря добавленному .gitignore.
[ignore files](https://github.com/sash3939/VCS_Git/assets/156709540/d5c672df-b328-453a-a567-53f78372f625)

5. Закоммитили все новые и изменённые файлы. Комментарий к коммиту Added gitignore.

[Added gitignore commit](https://github.com/sash3939/VCS_Git/assets/156709540/73a5c519-ab73-4df7-87e5-1df992ca5db9)


### Эксперимент с удалением и перемещением файлов (третий и четвёртый коммит)

1. Создали файлы will_be_deleted.txt (с текстом will_be_deleted) и will_be_moved.txt (с текстом will_be_moved) и закоммитили их с комментарием Prepare to delete and move.Create](https://github.com/sash3939/VCS_Git/assets/156709540/69ae7a33-de86-4387-8733-e40da7c43f2a)
[Create and commit](https://github.com/sash3939/VCS_Git/assets/156709540/86cf2c82-8888-4b8f-b3e7-5c352c4e7cf1)

2. Удалили файл will_be_deleted.txt с диска и из репозитория.
[rm file](https://github.com/sash3939/VCS_Git/assets/156709540/916f2ef6-b98f-4b06-a671-c2c7cfde93fe)

3. Переименовали (переместите) файл will_be_moved.txt на диске и в репозитории, чтобы он стал называться has_been_moved.txt.
4. Закоммитили результат работы с комментарием Moved and deleted.
[mv and commit](https://github.com/sash3939/VCS_Git/assets/156709540/774be07d-015b-40a7-a3e8-50b0390311b5)


### Проверка изменения

1. В результате предыдущих шагов в репозитории должно быть как минимум пять коммитов (если вы сделали ещё промежуточные — нет проблем):
- Initial Commit — созданный GitHub при инициализации репозитория.
- First commit — созданный после изменения файла README.md.
- Added gitignore — после добавления .gitignore.
- Prepare to delete and move — после добавления двух временных файлов.
- Moved and deleted — после удаления и перемещения временных файлов.
2. Проверили, используя комманду git log.

[git log](https://github.com/sash3939/VCS_Git/assets/156709540/e7d6b8cf-0c16-4bd4-b559-01e5339a414b)


### Отправка изменений в репозиторий

1. Выполните команду git push, если Git запросит логин и пароль — введите ваши логин и пароль от GitHub.
[git push](https://github.com/sash3939/VCS_Git/assets/156709540/68aeac30-3fe7-420e-8bbb-94cfa1a2d07c)


2. В качестве результата отправьте ссылку на репозиторий.
https://github.com/sash3939/devops-netology.git

----
