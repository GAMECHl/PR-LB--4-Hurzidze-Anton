# PR-LB--4-Hurzidze-Anton
## Хурцидзе Антон IПЗ 3.02 Практична-Лабораторна робота № 4

## Тема: Реалізація нової сутності, створення CRUD-операцій та відповідного RESTful API
## Мета: Закріпити навички створення повноцінної серверної логіки для роботи з новою сутністю за допомогою TypeORM, Express та TypeDI. Ознайомитися з процедурою створення міграцій, перевірки змін у структурі бази даних та тестування REST API через Postman.

#### Використовуючи команду ```npm run migration:generate test``` генеруємо міграцію:
![1](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/1.png)
#### Після виконання команди в каталозі ```migrations``` з'явится файл:
![2](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/2.png)
#### Далі потрібно змінити зміст міграції і ми побачимо файл з наступним змістом:
![3](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/3.png)
#### Наступним кроком запускаємо міграцію:
![4](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/4.png)
#### Оновлюємо сторінку с базою данних та бачимо успішне виконанная міграції:
![5](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/5.png)
#### Створюємо каталог posts в каталозі controllers, і вже в цьому каталозі створюємо файл list.ts:
![6](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/6.png)
#### Та редактуємо зміст цього файла наступним чином:
![7](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/7.png)
#### Далі створюємо файл Post.ts в католозі src/orm/posts:
![8](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/8.png)
#### Використовуючи команду ```npm run migration:generate post``` стоврюємо міграцію:
![9](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/9.png)
#### Та запустимо її командою ```npm run migration:run```:
![10](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/10.png)
#### Після успішного виконання міграції, ми побачимо наступне в каталозі бази данних:
![11](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/11.png)
#### Для створення Post нам потрібно в каталозі /src/controllers/posts створити файл create.ts з наступним змістом:
![12](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/12.png)
#### Далі в каталозі /src/controllers/routes створюємо файл post.ts який визначе маршут:
![13](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/13.png)
#### В каталозі /src/controllers/posts створюємо файли - update.ts, delete.ts, show.ts, index.test.ts та index.ts:
![14](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/14.png)
#### Ці фвйли редактуємо наступним змістом:
#### Update.ts:
![15](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/15.png)
#### Delete.ts:
![16](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/16.png)
#### Show.ts:
![17](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/17.png)
#### Index.ts:
![18](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/18.png)
#### Index.test.ts:
![19](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/19.png)
![20](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/20.png)
#### У каталозі src/router/v1 створюємо файл post.ts з наступним змістом:
![21](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/21.png)
#### Наступним кроком змінюємо файл index.ts в каталозі src/routes щоб додати маршрут на пост:
![22](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/22.png)
#### Запускаємо сервер:
![22](https://github.com/GAMECHl/PR-LB--4-Hurzidze-Anton/blob/main/22.png)

