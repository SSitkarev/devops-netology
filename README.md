# devops-netology

## Создание репозитория и первого коммита

Зарегистрируйте аккаунт на https://github.com/. Если предпочитаете другое хранилище для репозитория, можно использовать его.

Создайте публичный репозиторий, который будете использовать дальше на протяжении всего курса, желательное с названием devops-netology. Обязательно поставьте галочку Initialize this repository with a README.

Диалог создания репозитория

Создайте авторизационный токен для клонирования репозитория.

Склонируйте репозиторий, используя протокол HTTPS (git clone ...).

Клонирование репозитория

Перейдите в каталог с клоном репозитория (cd devops-netology).

Произведите первоначальную настройку Git, указав своё настоящее имя, чтобы нам было проще общаться, и email (git config --global user.name и git config --global user.email johndoe@example.com).

Выполните команду git status и запомните результат.

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/1_7.jpg)

Отредактируйте файл README.md любым удобным способом, тем самым переведя файл в состояние Modified.

Ещё раз выполните git status и продолжайте проверять вывод этой команды после каждого следующего шага.

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/1_9.jpg)

Теперь посмотрите изменения в файле README.md, выполнив команды git diff и git diff --staged.

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/1_10.jpg)

Переведите файл в состояние staged (или, как говорят, просто добавьте файл в коммит) командой git add README.md.

И ещё раз выполните команды git diff и git diff --staged. Поиграйте с изменениями и этими командами, чтобы чётко понять, что и когда они отображают.

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/1_12.jpg)

Теперь можно сделать коммит git commit -m 'First commit'.

И ещё раз посмотреть выводы команд git status, git diff и git diff --staged.

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/1_14.jpg)

## Создание файлов .gitignore и второго коммита

Создайте файл .gitignore (обратите внимание на точку в начале файла), проверьте его статус сразу после создания.

Добавьте файл .gitignore в следующий коммит (git add...).

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/2_2.jpg)

На одном из следующих блоков вы будете изучать Terraform, давайте сразу создадим соотвествующий каталог terraform и внутри этого каталога — файл .gitignore по примеру: https://github.com/github/gitignore/blob/master/Terraform.gitignore.

В файле README.md опишите своими словами, какие файлы будут проигнорированы в будущем благодаря добавленному .gitignore.

### Ответ: 

Будут проигнорированы 

- локальные директории .terraform,

- файлы, название которых заканчивающиется на *.tfstate

- файлы, которые содержат в названии *.tfstate.*

- файлы, с названими crash.log и crash.*.log (* заменяет любые символы)

- файлы, название которых заканчивается на *.tfvars и *.tfvars.json

- файлы с названиями override.tf и override.tf.json, а так же заканчивающиеся на *_override.tf и *_override.tf.json

- файлы с названиями .terraformrc и terraform.rc.

Закоммитьте все новые и изменённые файлы. Комментарий к коммиту должен быть Added gitignore.

## Эксперимент с удалением и перемещением файлов (третий и четвёртый коммит)

Создайте файлы will_be_deleted.txt (с текстом will_be_deleted) и will_be_moved.txt (с текстом will_be_moved) и закоммите их с комментарием Prepare to delete and move.

В случае необходимости обратитесь к официальной документации — здесь подробно описано, как выполнить следующие шаги.

Удалите файл will_be_deleted.txt с диска и из репозитория.

Переименуйте (переместите) файл will_be_moved.txt на диске и в репозитории, чтобы он стал называться has_been_moved.txt.

Закоммитьте результат работы с комментарием Moved and deleted.

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/3.jpg)

## Проверка изменения

В результате предыдущих шагов в репозитории должно быть как минимум пять коммитов (если вы сделали ещё промежуточные — нет проблем):
Initial Commit — созданный GitHub при инициализации репозитория.
First commit — созданный после изменения файла README.md.
Added gitignore — после добавления .gitignore.
Prepare to delete and move — после добавления двух временных файлов.
Moved and deleted — после удаления и перемещения временных файлов.
Проверьте это, используя комманду git log. Подробно о формате вывода этой команды мы поговорим на следующем занятии, но посмотреть, что она отображает, можно уже сейчас.

![Задание1](https://github.com/SSitkarev/devops-netology/blob/main/img/4.jpg)

Отправка изменений в репозиторий

Выполните команду git push, если Git запросит логин и пароль — введите ваши логин и пароль от GitHub.

В качестве результата отправьте ссылку на репозиторий.