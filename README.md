# Домашнее задание к занятию 7 «Жизненный цикл ПО»  

## Подготовка к выполнению  

1. Получить бесплатную версию [Jira](https://www.atlassian.com/ru/software/jira/free).  
2. Настроить её для своей команды разработки.  
3. Создать доски Kanban и Scrum.  
![create_project1](/screenshots/1.png)  
![create_project2](/screenshots/2.png)  

5. [Дополнительные инструкции от разработчика Jira](https://support.atlassian.com/jira-cloud-administration/docs/import-and-export-issue-workflows/).  

## Основная часть  

Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:  

1. Open -> On reproduce.
2. On reproduce -> Open, Done reproduce.  
3. Done reproduce -> On fix.  
4. On fix -> On reproduce, Done fix.  
5. Done fix -> On test.  
6. On test -> On fix, Done.  
7. Done -> Closed, Open.  
![create_project3](/screenshots/3.png)  
![create_project4](/screenshots/4.png)  

Остальные задачи должны проходить по упрощённому workflow:  

1. Open -> On develop.  
2. On develop -> Open, Done develop.  
3. Done develop -> On test.  
4. On test -> On develop, Done.  
5. Done -> Closed, Open.  
![create_project5](/screenshots/5.png)  
![create_project6](/screenshots/6.png)  

**Что нужно сделать**  

1. Создайте задачу с типом bug, попытайтесь провести его по всему workflow до Done.  
![create_project7](/screenshots/7.png)  

2. Создайте задачу с типом epic, к ней привяжите несколько задач с типом task, проведите их по всему workflow до Done.  
![create_project8](/screenshots/8.png)  
![create_project9](/screenshots/9.png)  

3. При проведении обеих задач по статусам используйте kanban.  
Есть  

4. Верните задачи в статус Open.  
Есть  
![create_project10](/screenshots/10.png)  

5. Перейдите в Scrum, запланируйте новый спринт, состоящий из задач эпика и одного бага, стартуйте спринт, проведите задачи до состояния Closed. Закройте спринт.  
![create_project11](/screenshots/11.png)  
![create_project12](/screenshots/12.png)  
![create_project13](/screenshots/13.png)  

7. Если всё отработалось в рамках ожидания — выгрузите схемы workflow для импорта в XML. Файлы с workflow и скриншоты workflow приложите к решению задания.  
Все прошло в рамках ожидания:  
[workflow_bug](/workflows/workflow_bug.xml)  
[workflow_simplified](/workflows/workflow_simplified.xml)  

---
