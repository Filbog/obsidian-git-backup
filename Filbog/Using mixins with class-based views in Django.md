#coding #django #webdev 

**Order is critical**. For example here:

`from django.contrib.auth.mixins import (`
    `LoginRequiredMixin,`
    `UserPassesTestMixin # new`
`)`
`from django.views.generic.edit import UpdateView`

`class ArticleUpdateView(`
  `LoginRequiredMixin, UserPassesTestMixin, UpdateView):  # new`
    `model = Article`
    `fields = (`
        `"title",`
        `"body",`
    `)`
    `template_name = "article_edit.html"`

    def test_func(self):
        obj = self.get_object()
        return obj.author == self.request.user
**LoginRequiredMixin must come first to force login, then UserPassesTestMixin to authorize, and only then the view.**
