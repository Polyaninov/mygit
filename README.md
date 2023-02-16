Домашнее задание к занятию «8.1. Git»  Polyaninov Maksim

Инструкция по выполнению домашнего задания

    Сделайте fork репозитория c шаблоном решения к себе в GitHub и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw.
    Выполните клонирование этого репозитория к себе на ПК с помощью команды git clone.
    Выполните домашнее задание и заполните у себя локально этот файл README.md:
        впишите сверху название занятия, ваши фамилию и имя;
        в каждом задании добавьте решение в требуемом виде — текст, код, скриншоты, ссылка;
        для корректного добавления скриншотов используйте инструкцию «Как вставить скриншот в шаблон с решением»;
        при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в инструкции по MarkDown.
    После завершения работы над домашним заданием сделайте коммит git commit -m "comment" и отправьте его на GitHub git push origin.
    Для проверки домашнего задания в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем GitHub.
    Любые вопросы по выполнению заданий задавайте в чате учебной группы или в разделе «Вопросы по заданию» в личном кабинете.

Желаем успехов в выполнении домашнего задания!
   
   Задание 1

Что нужно сделать:

    1. Зарегистрируйте аккаунт на GitHub.
       Создайте публичный репозиторий. Обязательно поставьте галочку в поле «Initialize this repository with a README».
    
    Склонируйте репозиторий, используя https протокол git clone ....
    
![2667b1a8-25e1-4e06-b919-eab8c7474ad1](https://user-images.githubusercontent.com/75700701/219427462-1edd10a8-876a-4f80-94f3-6b8605f2b3f4.jpg)


   Перейдите в каталог с клоном репозитория.
   Произведите первоначальную настройку Git, указав своё настоящее имя и email: git config --global user.name и git config --global user.email johndoe@example.com. 
   
   ![75f9d4c8-9408-4c0f-8f4d-581dad49c37f](https://user-images.githubusercontent.com/75700701/219429549-f41638df-4b9b-4959-8516-5c9e0ca6459c.jpg)
   
   
 2.   Выполните команду git status и запомните результат.
      Отредактируйте файл README.md любым удобным способом, переведя файл в состояние Modified.
  

      ![ed9efb48-eb2e-42eb-ab2e-0ca1661fd3b6](https://user-images.githubusercontent.com/75700701/219430557-3b8ce932-5a2d-4d45-ad5d-5b967e471ec3.jpg)

3.   Ещё раз выполните git status и продолжайте проверять вывод этой команды после каждого следующего шага.
     Посмотрите изменения в файле README.md, выполнив команды git diff и git diff --staged.
     
     ![fdddf973-ccdc-47d0-88f7-0934825c9ae9](https://user-images.githubusercontent.com/75700701/219431425-aeb7ccdf-590b-47c1-a1b4-4dc03c7df48f.jpg)
     
     
  4.    Переведите файл в состояние staged или, как говорят, добавьте файл в коммит, командой git add README.md.
        Ещё раз выполните команды git diff и git diff --staged

        ![0b589b9c-560b-4ba3-a644-b4875816cf48](https://user-images.githubusercontent.com/75700701/219435211-b741f937-45cf-45c0-b45a-5de3b48bf052.jpg)
        
        
        
  5.   Теперь можно сделать коммит git commit -m 'First commit'.
        Сделайте git push origin master.
        
        ![9f33c373-ff27-4a04-ac14-7e4b484e80d1](https://user-images.githubusercontent.com/75700701/219435654-d3791ff0-87ee-4f5a-8e84-2a01069860f4.jpg)

        




     Задание 2
     Что нужно сделать:

     Создайте файл .gitignore (обратите внимание на точку в начале файла) и проверьте его статус сразу после создания.
     Добавьте файл .gitignore в следующий коммит git add....
       
  ![6918b477-4c14-4e2e-a556-ab024aeae5e6](https://user-images.githubusercontent.com/75700701/219464952-94c04906-b0cb-4fff-bea3-902f3c4129b3.jpg)
  
  
    Напишите правила в этом файле, чтобы игнорировать любые файлы .pyc, а также все файлы в директории cache.
    Сделайте коммит и пуш.
    
     
     
![9f33c373-ff27-4a04-ac14-7e4b484e80d1 (1)](https://user-images.githubusercontent.com/75700701/219465760-42daf011-7adb-4612-a24e-e0e007f3b98a.jpg)

    
    
  https://github.com/Polyaninov/mygit/blob/2f91e99e52ead81ecf7885b49bcac8d603c59705/.gitignore

    
    
Задание 3
Что нужно сделать:

Создайте новую ветку dev и переключитесь на неё.

![6bf95972-98c6-44b7-9ac3-2ec57e6af299](https://user-images.githubusercontent.com/75700701/219467239-e39f826d-ebad-4a3a-bf61-2b95479b85f2.jpg)


Создайте файл test.sh с произвольным содержимым.

![e66f048e-d38c-47e1-ac5b-2ba7e9943631](https://user-images.githubusercontent.com/75700701/219467367-e0358d16-34bd-4b92-908f-ba28529adcd6.jpg)


Сделайте несколько коммитов и пушей, имитируя активную работу над этим файлом.
Сделайте мердж этой ветки в основную. Сначала нужно переключиться на неё, а потом вызывать git merge.
Сделайте коммит и пуш.


![20c862c7-9b2d-4482-a797-be8512a37aff](https://user-images.githubusercontent.com/75700701/219467653-2df31320-cf0c-463a-9c03-5be668381485.jpg)



![4818ae0a-9ebc-4fd7-afa7-fb00d56bb12c](https://user-images.githubusercontent.com/75700701/219467702-387015c5-1859-4934-99c9-c554f842a36a.jpg)

  
https://github.com/Polyaninov/mygit/blob/323b5f2e29787c38af10791fb41744bc6e76ef79/test.sh
      
      




   
    
