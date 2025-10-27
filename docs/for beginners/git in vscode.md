## Пора разобраться с гитом вэсэкодом и гитхабом

### Если вы используете github desktop - удалите его к чертям

скачиваем, если ещё не скачали https://code.visualstudio.com/ https://git-scm.com/


регаемся https://github.com сразу заходим в [настройки](https://github.com/settings/emails), чекаем свои email и username 

![git-geting-started-username-eamil](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-username-eamil.png){ align=left }


### открываем vscode, открываем терминал
![git-geting-started-username-eamil](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-terminal.png){ align=left }



вставляем туда по очереди эти две команды, предварительно меняем юзернаме и емаил на свои

`git config --global user.email "you@example.com"`

`git config --global user.name "Your Name"`

### Пока переходим в гитхабыч:

https://github.com/tsenturion/inueco делаем форк  

![git-geting-started-making-fork](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-making-fork.png){ align=left }


### Возвращаемся в vscode

Клонируем наш репозиторий, тыкаем сюда

![git-geting-started-clone-git-repo](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-git-repo.png){ align=left }


Выбираем нужный репозиторий, в нашем случае это будет что-то типа https://github.com/вашюзернейм/inueco.git вот его и выбираем

![git-geting-started-clone-git-repo-choose](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-git-repo-choose.png){ align=left }


Прежде чем продолжить устанавливаем:
https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github

Лучше делать это через вкладку extensions

![git-geting-started-clone-extensions-installing](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-extensions-installing.png){ align=left }



Вбиваем туда identifier: `github.vscode-pull-request-github`, бтв следующие дополнения будем устанавливать также, так шо привыкайте, тыкаем установить буквально единственная синяя кнопка, но на всякий случай:

![git-geting-started-clone-extensions-installing2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-extensions-installing2.png){ align=left }



Далее в терминал вбиваем `git pull --all` чтобы получить вообще все изменения, которые происходили. Если не сделаете ,не сможете через кнопку пулить изменения с апстрим репозитория. Кароч это нужно сделать, поверьте.


### git pull from upstream
Как получить изменения, когда он что-то сделал там у себя - тыкаем 

![git-geting-started-pull-from-upstream](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-from-upstream.png){ align=left }


### Далее ОБЯЗАТЕЛЬНО тыкаем main, HEAD ваще может на любую хуйню ссылаться, лучше не тыкайте его пока

![git-geting-started-pull-from-upstream2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-from-upstream2.png){ align=left }


### Это же мы выполняем, если преподаватель скажет, что что-то поправил. 

# Мы готовы к работе

дальше пришли такие на пару, нам дали задание, делаем в интервейсе vs code [git pull from upstream](#git-pull-from-upstream) как мы это делали на шаге раньше, вобщем привыкайте, будем делать это часто. 


## Следующее шо мы делаем - создаём ветку, или иными словами branch

это надо, шоб лишние файлы не влетали в ваш pull request, если не будете создавать ветки, то когда в следующий раз будете выполнять задание, то в пул реквест будут попадать файлы с предыдущих практик, нам такое не надо, шоб лишних вопросов к нам не было. 


кароч: Просто делайте новую ветку на каждую пару. 


![git-geting-started-create-branch](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch.png){ align=left }



сюда прописываем название, лучше по сегодняшней дате называйте, шоб потом мало ли его найти. 


![git-geting-started-create-branch2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch2.png){ align=left }



Публикуем, сообщение писать не надо, просто тыкаем синюю кнопку

![git-geting-started-create-branch3](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch3.png){ align=left }



Выбираем origin 

![git-geting-started-create-branch4](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch4.png){ align=left }




Проверка, что всё получилось - пишем в терминале git branch, если всё кайф, то * и зелёным цветом выделится ваша ветка. Если звёздочка возле main, и ваша ветка не отображается - вы что то сделали не так. 

![git-geting-started-create-branch5](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch5.png){ align=left }



### Можно выполнять задание

дальше делайте шо нужно, создавайте новые файлы, кароч питонируйте там по жоскому. 

![git-geting-started-creating-commit](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit.png){ align=left }



Дальше выбираем только те файлы, которые мы сами редактировали или создавали. Обязательно пишем сообщение и жмём большую синюю кнопку commit

![git-geting-started-creating-commit2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit2.png){ align=left }



не напишите сообщение в окно - откроется такое окно
просто напишите своё сообщение в нём, сохраните файл ctrl+s и закройте эту вкладочку

![git-geting-started-creating-commit3](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit3.png){ align=left }



Лишние файлы удаляем - или тыкаем discard changes - нам предложат удалить файл, либо удаляем ручками во вкладке проекта

![git-geting-started-creating-commit4](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit4.png){ align=left }



### Отправляем изменения в github

![git-geting-started-creating-commit5](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit5.png){ align=left }



Создаём пулл реквест, чтобы преподаватель увидел наши результаты:

![git-geting-started-pull-request](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-request.png){ align=left }



откроется окно, в title пишем фамилию, дату и группу, тыкаем create

![git-geting-started-pull-request2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-request2.png){ align=left }



# на этом всё! почти...

Возвращаемся обратно в main ветку, чтобы потом новые ветки создавались "чистыми". Кароч это нужно сделать, поверьте.

![git-geting-started-checkout](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-checkout.png){ align=left }



ОБЯЗАТЕЛЬНО выбираем origin/main

![git-geting-started-checkout2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-checkout2.png){ align=left }




Ну и вспоминаем как мы делали [git pull from upstream](#git-pull-from-upstream) через кнопки vscode или просто в консоль вбиваем `git pull upstream main`