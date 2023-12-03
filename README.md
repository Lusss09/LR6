# LR6
Лабораторная работа №6
Цель лабораторной работы:
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием. 
Ход работы:
1) В начале создается аккаунт на GitHub
2) Создаём копию в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork).
3) Устанавливаем Git
4) Настраиваем клиент Git, вводим (Группа Фамилия И.О.) и email.  
  для этого вводим команды:  
  git config user.name "<имя>"  
  git config user.email "<почта>"  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%B8%D0%BC%D1%8F%20%D0%B8%20%D0%BF%D0%BE%D1%87%D1%82%D0%B0.png) 
5) Клонируем свой личный удалённый репозиторий на компьютер.  
   для этого вводим команду (перед этим перейдя в католог, где будет репозиторий):  
   git clone <ссылкаНаРепозиторий>  
   ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/clone.png)  
6) Добавляем файл через интерфейс GitHub. Подтягиваем изменения в локальный репозиторий.  
  Для подтягивания изменений в локальный репозиторий вводим команду:  
  git pull  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%B4%D0%BE%D0%B1%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BD%D0%BE%D0%B2%D0%BE%D0%B3%D0%BE%20%D1%84%D0%B0%D0%B9%D0%BB%D0%B0.png)  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%BD%D0%BE%D0%B2%D1%8B%D0%B9%20%D1%84%D0%B0%D0%B9%D0%BB.png)  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%BD%D0%BE%D0%B2%D1%8B%D0%B9%20%D1%84%D0%B0%D0%B9%D0%BB%20%D0%B4%D0%BE%D0%B1%D0%B0%D0%B2%D0%B8%D0%BB%D1%81%D1%8F.png)   
7) Получаем историю операций для каждой из веток.  
  Для этого вводим команду:  
  git log  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/git%20log.png)  
  Для смены ветки вводим команду:  
  git checkout branch1  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%BF%D0%B5%D1%80%D0%B5%D1%85%D0%BE%D0%B4%20%D0%BD%D0%B0%20%D0%B2%D0%B5%D1%82%D0%BA%D1%83%20%D0%B1%D1%80%D0%B0%D0%BD%D1%871.png)  
8) Просматриваем последние изменения.  
  Для этого вводим команду:  
  git log  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/git%20log...png)  
9) Выполняем слияние в ветку master, разрешив конфликт.  
  Для этого сначала переходим в ветку master:  
  вводим команду git checkout master  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%B2%D0%B5%D1%82%D0%BA%D0%B8%20%D0%BD%D0%B0%20%D0%BC%D0%B0%D1%81%D1%82%D0%B5%D1%80.png)  
  Для слияния вводим команду git merge branch1  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/merge%20branch%201.png)  
  Для разрешения конфликта редактируем файл  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/merge%D1%82%D0%B5%D0%BA%D1%81%D1%82.png)  
  Для сохранения изменений вводим: git add .  
  проверяем изменения с помощью git status  
  и применняем git commit -m "<Massage>"  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/merge.png)  
10) Удаляем побочную ветку после успешного слияния. 
  Для этого вводим команду git branch --delete branch1  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D1%83%D0%B4%D0%B0%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%B2%D0%B5%D1%82%D0%BA%D0%B8.png) 
11) Сохраняем изменения с помощью команд git add . и git commit -m "<Massage>"  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%B4%D0%BE%D0%B1%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B9.png)  
12) Делаем откат коммита  
  Для этого вводим git reset --soft HEAD~  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%BE%D1%82%D0%BA%D0%B0%D1%82%20%D0%BA%D0%BE%D0%BC%D0%B8%D1%82%D0%B0.png)  
13) Создаём ветку для отчета  
  Для этого вводим git checkout -b "<название>"  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D1%81%D0%BE%D0%B7%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%B2%D0%B5%D1%82%D0%BA%D0%B8%20%D0%BE%D1%82%D1%87%D0%B5%D1%82%D0%B0.png)  
14) Оформляем отчет  
15) Получаем историю операций в форматированном виде и сохраняем изменения  
  Для этого вводим команду git log --pretty=format: "%h - %ad | %an | %s"  
  ![](https://github.com/Lusss09/LR6/blob/Report/Screenshots/%D0%B8%D1%81%D1%82%D0%BE%D1%80%D0%B8%D1%8F%20%D0%BE%D0%BF%D0%B5%D1%80%D0%B0%D1%86%D0%B8%D0%B9.png)  
16) Отправляем локальные изменения в сетевое хранилище GitHub  
  Для этого вводим команду git push  
17) Лог команд:
  git config - настройки
  git clone - клонирование репозитория
  git pull - используется для извлечения и загрузки содержимого из удаленного репозитория
  git log - используется для просмотра истории коммитов
  git checkout - для перехода на другую ветку
  git merge - объединяет ветки
  git commit -m - для создания коммита
  git branch --delete - для удаления ветки
  git push - передаёт в удалённый репозиторий изменения, сделанные в локальном репозитории
  git status - показывает состояния файлов в рабочем каталоге
  git reset --soft HARD - для отката коммита
  git log --pretty=format: "%h - %ad | %an | %s" - для получения истории операций в форматированном виде
## Вывод:  
Мы изучили базовые возможности системы управления версиями, получили опыт работы с Git Api, опыт работы с локальным и удаленным репозиториями.