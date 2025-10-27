# Как юзать git и github в vscode

!!! tip "Важно"

    Если вы используете github desktop - удалите его к чертям


скачиваем, если ещё не скачали https://code.visualstudio.com/ https://git-scm.com/
<br><br>
<figure markdown="span">
![git-geting-started-username-eamil](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-username-eamil.png){ align=right width="500"}

регаемся https://github.com сразу заходим в [настройки](https://github.com/settings/emails), **чекаем свои email и username**
</figure>

## Базовые настройки
<figure markdown="span">

открываем vscode, открываем терминал<br><br>
![git-geting-started-username-eamil](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-terminal.png){ align=left width="500"}



вставляем туда по очереди эти две команды, предварительно меняем юзернаме и емаил на свои
<br><br>

```git config --global user.email "you@example.com"```

<br>

`git config --global user.name "Your Name"`

</figure>

## Делаем fork

<figure markdown="span">

Пока переходим в гитхабыч:<br><br>
![git-geting-started-making-fork](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-making-fork.png){ align=left width="500"}



https://github.com/tsenturion/inueco делаем форк 
</figure>

<figure markdown="span">
Возвращаемся в vscode



![git-geting-started-clone-git-repo](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-git-repo.png){ width="500"}
<figcaption>Клонируем наш репозиторий, тыкаем сюда</figcaption>
</figure>

<figure markdown="span">


![git-geting-started-clone-git-repo-choose](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-git-repo-choose.png){ align=left width="500"}


Выбираем нужный репозиторий, в нашем случае это будет что-то типа https://github.com/вашюзернейм/inueco.git вот его и выбираем
</figure>

## Установка расширения для гитхаба

Прежде чем продолжить устанавливаем:
https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github

<figure markdown="span">
Лучше делать это через вкладку extensions

![git-geting-started-clone-extensions-installing](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-extensions-installing.png){ align=left width="500"}



Вбиваем туда identifier: `github.vscode-pull-request-github`, бтв следующие дополнения будем устанавливать также, так шо привыкайте

</figure>
<figure markdown="span">
тыкаем установить буквально единственная синяя кнопка, но на всякий случай:
![git-geting-started-clone-extensions-installing2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-clone-extensions-installing2.png){ width="500"}
<figcaption></figcaption>
</figure>


Далее в терминал вбиваем `git pull --all` чтобы получить вообще все изменения, которые происходили. Если не сделаете ,не сможете через кнопку пулить изменения с апстрим репозитория. Кароч это нужно сделать, поверьте.


## git pull from upstream
Как получить изменения, когда преподаватель что-то сделал там у себя, грит обновитесь - тыкаем 
<figure markdown="span">
![git-geting-started-pull-from-upstream](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-from-upstream.png){ width="500"}
<figcaption></figcaption>
</figure>

<figure markdown="span">
**Далее ОБЯЗАТЕЛЬНО тыкаем main**, HEAD ваще может на любую хуйню ссылаться, лучше не тыкайте его пока

![git-geting-started-pull-from-upstream2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-from-upstream2.png){ width="500"}
<figcaption></figcaption>
</figure>

Всё тоже самое мы выполняем, если преподаватель скажет, что что-то поправил. 

## Мы готовы к работе

дальше пришли такие на пару, нам дали задание, делаем в интерфейсе vs code [git pull from upstream](#git-pull-from-upstream) как мы это делали на шаге раньше, вобщем привыкайте, будем делать это часто. 


## Следующее шо мы делаем - создаём ветку, или иными словами branch


это надо, шоб лишние файлы не влетали в ваш pull request, если не будете создавать ветки, то когда в следующий раз будете выполнять задание, то в пул реквест будут попадать файлы с предыдущих практик, нам такое не надо, шоб лишних вопросов к нам не было. 


кароч: Просто делайте новую ветку на каждую пару. 

<figure markdown="span">
![git-geting-started-create-branch](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch.png){  width="500"}
<figcaption></figcaption>
</figure>

<figure markdown="span">


![git-geting-started-create-branch2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch2.png){ align=left width="500"}
сюда прописываем название, лучше по сегодняшней дате называйте, шоб потом мало ли его найти. 

</figure>



<figure markdown="span">
![git-geting-started-create-branch3](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch3.png){ align=right width="500"}
Публикуем, сообщение писать не надо, просто тыкаем синюю кнопку

</figure>

<figure markdown="span">

![git-geting-started-create-branch4](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch4.png){  width="500"}

Выбираем origin 

</figure>


<figure markdown="span">

![git-geting-started-create-branch5](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-create-branch5.png){ align=left width="500"}

Проверка, что всё получилось - пишем в терминале git branch, если всё кайф, то * и зелёным цветом выделится ваша ветка. Если звёздочка возле main, и ваша ветка не отображается - вы что то сделали не так. 

</figure>

## Можно выполнять задание

!!! tip "Работайте братья"

    дальше делайте шо нужно, создавайте новые файлы, кароч питонируйте там по жоскому. 




<figure markdown="span">

![git-geting-started-creating-commit2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit2.png){ align=left width="500"}

Дальше выбираем только те файлы, которые мы сами редактировали или создавали. Обязательно пишем сообщение и жмём большую синюю кнопку commit
</figure>

<figure markdown="span">



![git-geting-started-creating-commit3](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit3.png){ align=right width="500"}
Если не напишите сообщение в окно это не страшно - откроется такое окно, паниковать не надо, ничего не сломалось
просто напишите своё сообщение в нём, сохраните файл ctrl+s и закройте эту вкладочку
</figure>

<figure markdown="span">


![git-geting-started-creating-commit4](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit4.png){ align=left width="500"}
Если в процессе появились лишние файлы, ну например вы тест запустили или ещё какую нибудь новую весёлую фигню, то л ишние файлы удаляем - или тыкаем discard changes - нам предложат удалить файл, либо удаляем ручками во вкладке проекта

</figure>

## Отправляем изменения в github

<figure markdown="span">

![git-geting-started-creating-commit5](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-creating-commit5.png){ align=left width="500"}

</figure>

<figure markdown="span">


![git-geting-started-pull-request](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-request.png){ align=left width="500"}
Создаём пулл реквест, чтобы преподаватель увидел наши результаты:

</figure>

<figure markdown="span">


![git-geting-started-pull-request2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-pull-request2.png){ align=right width="500"}
откроется окно, в title пишем фамилию, дату и группу, тыкаем create

</figure>

## на этом всё! почти...

Возвращаемся обратно в main ветку, чтобы потом новые ветки создавались "чистыми". Кароч это нужно сделать, поверьте.
<figure markdown="span">

![git-geting-started-checkout](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-checkout.png){ align=left width="500"}
</figure>


<figure markdown="span">

ОБЯЗАТЕЛЬНО выбираем origin/main

![git-geting-started-checkout2](https://raw.githubusercontent.com/Egoryich/Based-Department/refs/heads/main/images/get_started_inueco_git/git-geting-started-checkout2.png){ align=left width="500"}
</figure>



Ну и вспоминаем как мы делали [git pull from upstream](#git-pull-from-upstream) через кнопки vscode или просто в консоль вбиваем `git pull upstream main`