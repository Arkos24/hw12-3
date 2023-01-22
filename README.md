# Домашнее задание к занятию "Базы данных" - Мельников Семен


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

 Задание 1
 
 SELECT DISTINCT district FROM sakila.address WHERE district LIKE 'K%a' AND locate(' ', district) =0
 
 ![image](https://user-images.githubusercontent.com/114281054/213119915-0e263d81-bb1d-4b24-b043-b7802b2c45aa.png)


 Задание 2
 
 SELECT * FROM sakila.payment WHERE date(payment_date) BETWEEN '2005-06-15' AND '2005-06-18' AND amount > 10
 
 ![image](https://user-images.githubusercontent.com/114281054/213905760-91e84c93-5e5f-448a-af82-420e598ff41b.png)
 



 Задание 3
 
 SELECT * FROM sakila.rental ORDER BY rental_date DESC 
 
 ![image](https://user-images.githubusercontent.com/114281054/213121481-db702b83-d761-444e-bf62-a741f418c7b9.png)


 Задание 4
 
 SELECT replace(lower(first_name), 'll', 'pp'), lower(last_name) FROM sakila.customer WHERE active = '1' AND first_name IN ('Kelly') OR active = '1' AND first_name IN ('Willie')
 
 ![image](https://user-images.githubusercontent.com/114281054/213122710-ae586120-6e44-4387-bfb5-0b785d07e173.png)
