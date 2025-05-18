On a view level, with class-based views: we use mixins -  **LoginRequiredMixin** for only logged-in users content, **UserPassesTestMixin** with modified test_func() to for example only give access to the author of an article. Example in code:

`from django.contrib.auth.mixins import LoginRequiredMixin, UserPassesTestMixin`
`from django.views.generic.edit import UpdateView, DeleteView, CreateView`

`class ArticleUpdateView(LoginRequiredMixin, UserPassesTestMixin, UpdateView):`
    `model = Article`
    `fields = (`
        `"title",`
        `"body",`
    `)`
    `template_name = "article_edit.html"`

    def test_func(self):
        obj = self.get_object()
        return obj.author == self.request.user
[[Using mixins with class-based views in Django]]
[[Help with wrapping my head around Generic Class-Based Views in Django]]