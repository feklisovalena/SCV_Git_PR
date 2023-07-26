![Logo] (headergit.png)
# Работа с Git и GitHub
Скачать [Установка VSCode](https://code.visualstudio.com)
## 1. Проверка наличия установленного Git
В терминале выполнить команду 
```
git version
```
Если Git установлен появится сообщение о версии программы, иначе будет сообщение об ошибке. 
## 2. Установка Git
Загружаем последнюю версию Git с сайта [Установка Git](https://git-scm.com/downloads.)
Устанавливаем с настройками по умолчанию.
## 3. Настройка Git
При первом использовании Git необходимо представиться.
Для этого нужно ввести в терминале 2 команды:
```
git config --global user.name "Ваше имя английскими буквами"
git config --global user.email "Ваша почта@example.com"
```
## 4. Инициализация репозитория
В терминале переходим к папке, в которой хотим создать репозиторий. Выполняем команду:
```
git init
```
## 5. Запись изминений в репозиторий
Для того, чтобы сохранить запись изминений в репозитроий, необходимо выполнить команду:
```
git commit
```
## 6. Просмотр истории коммитов
Для того, чтобы просмотреть историю коммитов, необходимо выполнить команду:
```
git log
```
## 7. Перемещение между сохранениями 
Для перемещения между сохранениями, необходимо выполнить команду:
```
git checkout
```
## 8. Игнорирование файлов
Для того, чтобы исключить из отслеживания в репозитории определенные файлы или папки, необходимо создать файл ***.gitignore*** и записать в него их названия или шаблоны, соответствующие таким файлам или папкам.
## 9. Создание веток в Git
По умолчанию имя основной ветки в Git - *master*.
Создать ветку можно командой:
```
git branch <название для новой ветки>
```
Список веток в репозитории можно посмотреть с помощью команды:
```
git branch
```
Текущая ветка будет отмечена звездочкой: **\* master**
## 10. Слияние веток и разрешение конфликтов
Для слияния выбранной ветки с текущей нужно выполнить команду:
```
git merge <название выбранной ветки>
```
Если былв изменена одна и та же часть файла в обеих ветках, то может возникнуть конфликт, который потребует участия пользователя.
VSCode предлагает варианты разрешения.
Чтобы разрешить конфликт, нужно выбрать один из вариантов, либо объединить содержимое по-своему. 
После разрешения конфликта нужно выполнить коммит слияния.
## 11. Удаление веток
Чтобы удалить ветку необходимо выполнить команду:
```
git branch -d <название необходимой ветки>
``` 
Нельзя удалить ветку, если вы находитесь в этой ветке в данный момент.
Если после сохраненых изменений не было слияния веток,то при удалении будет предлагаться? либо слияние? либо команда принудительного удаления:
```
git branch -D
```

# **Работа с удаленными репозиториями**
## 1.Создать аккаунт GitHub 
## 2.Cоздать локальный репозиторий 
## 3.Создать удаленный репозиторий 
## 4.Связать удаленный репозиторий с локальным 
Добавить удаленный репозиторий к проекту:

git remote add <имя для репозитория><url-адрес репозитория в сети>

Для получения и слияния изменений из удаленного репозитория используется команда:
```
git pull
```
``` C# 
while(count <0)
{
count++;
}
```
Для того, чтобы можно было работать с чужими репозиториями,нужно воспользоваться командой:
```
Fork
```
Затем с помощью кнопки: *Code* в разделе *Local* создается копия чужого удаленного репозитория
Затем заходим в локальный репозиторий и в терминале используем команду с помощью которой перейдем к корневую папку:
```
cd ..
``` 
И затем нужно ввести команду:
```
git clone <копия чужого удаленного репозитория>
```
Создать новую ветку 
После открыть чужой репозиторий в терминале 
 Внести изминения в репозиторий 
 Сохранить изминения 
Использовать команду 
```
git push --set-upstream origin new
```
Зайти в удаленный репозиторий, выбрать новую ветку 
Использовать команду ***Pull request*** - ***new pull request*** выбираем нужную нам ветку и нажимаем ***create pul request***
