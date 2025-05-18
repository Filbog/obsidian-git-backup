https://docs.djangoproject.com/en/4.2/ref/contrib/admin/#django.contrib.admin.ModelAdmin.list_display - docs

For example, I have an Article model and I want its three properties displayed in my list view. It'd look like this in the app's admin.py:



`from django.contrib import admin`
`from .models import Article`
`class ArticleAdmin(admin.ModelAdmin):`  
    `list_display = ["title", "body", "author",]`  
  
  
`admin.site.register(Article, ArticleAdmin)`

#django #coding #webdev #djangoforprofessionals 