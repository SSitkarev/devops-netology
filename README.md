# devops-netology

### Создание репозитория и первого коммита

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

### Создание файлов .gitignore и второго коммита

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

