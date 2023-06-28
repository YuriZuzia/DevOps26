## Небольшая памятка по git
Справка по MarkDown [здесь](https://gist.github.com/fomvasss/8dd8cd7f88c67a4e3727f9d39224a84c), или [здесь](https://www.markdownguide.org/cheat-sheet/)
А по Git идём [сюда](https://githowto.com/ru), например.
## Начало работы
Инициализация Git в текущем каталоге:
```bash
git init
```
а "разгитить":  `rm -rf .git`, если передумали.
Не забываем указать имя и почту:
```bash
$ git config --global user.name "Ivan Petrov"
# имя или ник нужно написать латиницей и в кавычках

$ git config --global user.email username@pochta.ru
# здесь нужно указать свой настоящий email
```
Не забываем про любимые команды:
```bash
git status
git add .
git commit -m "комментарий коммита"
git log
```
да! правим .gitignore,чтобы не хранить tmp, bak, секреты
Также, пропишем удалённй репозиторий:
```bash
git remote add origin git@github.com:YuriZuzia/Git_testing.git #ссылка на этот репозиторий
```
да, ssh ключики же у наc сгенерёны и паблик ключ добавлен в гит?
```bash
$ ssh-keygen -t rsa -b 4096 -C "электронная почта, к которой привязан ваш аккаунт на GitHub"
```
и после этого можим заливать свой репо в Git:
```bash
git push origin master #текущая ветка - master
git push -u  origin master #можно привязать ветку к одноименной удалённой - ключ -u
# после "связывания" просто:
git push
```

памятка будет дополняться, возможно :smiley:
