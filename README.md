# ToDoApp
Installation
   
        pip install pycopg2
        pip install django
 
  Usage
   
        https://www.enterprisedb.com/postgres-tutorials/how-use-postgresql-django
        https://www.youtube.com/watch?v=llbtoQTt4qw&t=4249s
        python3.8 manage.py runserver
        
 
 Examples
        
  
 
      https://github.com/divanov11/Django-To-Do-list-with-user-authentication
      
      urlpatterns = [
    path('login/', CustomLoginView.as_view(), name='login'),
    path('logout/', LogoutView.as_view(next_page='login'), name='logout'),
    path('register/', RegisterPage.as_view(), name='register'),
    path('', TaskList.as_view(), name='tasks'),
    path('task/<int:pk>/', TaskDetail.as_view(), name='task'),
    path('task-create/', TaskCreate.as_view(), name='task-create'),
    path('task-update/<int:pk>/', TaskUpdate.as_view(), name='task-update'),
    path('task-delete/<int:pk>/', DeleteView.as_view(), name='task-delete'),
]
