JSON
 4. Создать внешний репозиторий c названием JSON.
	https://github.com/Tellim235/JSON.git
 5. Клонировать репозиторий JSON на локальный компьютер.
	git clone https://github.com/Tellim235/JSON.git
 6. Внутри локального JSON создать файл “new.json”.
	touch JSON/new.json
 7. Добавить файл под гит.
	cd JSON 
	git add new.json
 8. Закоммитить файл.
	git commit -m "new"
 9. Отправить файл на внешний GitHub репозиторий.
	git push
 10. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
	vim new.json
	i
{
	"name": "Kseniya",
	"age": 35,
	"pets": 1,
	"salary": 300000
}
	Esc
	:wq
 11. Отправить изменения на внешний репозиторий.
	git add new.json
	git commit -m "new2"
	git push
 12. Создать файл preferences.json
	touch preferences.json
 13. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
	vim new.json
	i
{
	"film": "Spider man",
	"series": "Friends",
	"food": "Meat",
	"season": "Summer",
	"counrty": "Korea"
}
	Esc
	:wq	
 14. Создать файл skils.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
	touch skils.json
	vim skils.json
	i
{
	"Base theory": "1. Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC.", 
	"Client-Server": "2. Что такое клиент-серверная архитектура.",  
	"HTTP methods": "3. HTTP Методы запросов на сервер.",  
	"HTTP codes":"4. Коды ответов HTTP сервера.",  
	"HTTP Structures": "5. Структуры HTTP запросов и ответов.",  
	"JSON": "6. Что такое JSON, XML. Их структура.", 
	"API": "7. Тестирование API через Postman (JS, автотесты API).",
	"Other_skills": "и другие навыки"
}
	Esc
	:wq
 15. Отправить сразу 2 файла на внешний репозиторий.
	git add preferences.json skils.json
	git commit -m "add preferences.json and skils.json"
	git push
 16. На веб интерфейсе создать файл bug_report.json.
	Нажать Add file => Create new file , указываем имя файла bug_report.json
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
	В нижней части страницы нажимаем Commit new file
 18. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
	Выбрать файл bug_report.json и нажать "Edit this file"
{
	"ID": "A1",
	"Title": "Нажатие кнопки 'Поиск' на главной странице не предоставляет результат поиска",
	"Steps": [
		"1. Зайти на главную страницу сайта (ссылка на сайт)",
		"2. Ввести текст поиска",
		"3. Нажать кнопку Поиск"
	],
	"Enviroment":
	  {
		"OS": "Windows 10 x64",
		"Browser": "Google Chrome v 100.0.4896.127"
  	},
	"Expected result": "Нажатие кнопки Поиск выдает результат поиска",
	"Actual result": "При нажатии кнопки Поиск ничего не происходит",
	"Severity": "Critical",
	"Priority": "High",
	"Status": "Open",
	"Attachments": "ссылка на картинку или видео"
}
 19. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 20. Синхронизировать внешний и локальный репозиторий JSON
	git pull
