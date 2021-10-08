# JSON-server-run

Использование и установка джэйсон сервера: 

1. Установить глобально: // npm install -g json-server 

2. Добавить db.json в корень проекта с некоторыми данными, например:  

{  

"posts": [ 
{ "id": 1, "title": "json-server", "author": "typicode" } 
], 
"comments": [ 
{ "id": 1, "body": "some comment", "postId": 1 } 
], 
"profile": { "name": "typicode" } 
} 

3. Запускаем JSON-server: 

	//json-server --watch db.json 

Если вы перейдете по ссылке: http://localhost:3000/posts/1 , то получите в ответ response(GET): { "id": 1, "title": "json-server", "author": "typicode" } 

4. В scripts файло package.json добавить: "server": "json-server --port 7777 --watch db.json", 
