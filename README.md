# ToDoDjango

A simple ToDoApp api, because why not
### Installation - Windows
```
mkdir todoapp
virtualenv env
cd env
./scripts/activate
git clone https://github.com/exactlyprateek/ToDoDjango.git
cd tododjango
pip install -r requirements.py
python manage.py runserver
```
### API Overview
[http://localhost:8000/api/](http://localhost:8000/api/)
>Output
```
{
    "List": "/task-list/",
    "Detail View": "/task-detail/<id>/",
    "Create": "/task-create/",
    "Update": "/task-update/<id>/",
    "Delete": "/task-delete/<id>/"
}
```
### Example 1- Task Detail (method: GET)
[http://localhost:8000/api/task-detail/19](http://localhost:8000/api/task-detail/19) will return task details
```json
{
    "id": 19,
    "title": "wooo hoo",
    "completed": false
}
```
### Example 2- Task Delete (method: DELETE)
[http://localhost:8000/api/task-delete/19](http://localhost:8000/api/task-detail/19) will delete the task

This app has it's own frontend and an interactive api testing environment of sorts, hope you'll find your way :)
