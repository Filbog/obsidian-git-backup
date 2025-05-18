2024-08-17

Via chatGPT with an example:
### First Example

```
from django.contrib import admin

from .models import Book, Review

class ReviewInline(admin.TabularInline):
    model = Review

class BookAdmin(admin.ModelAdmin):
    inlines = [
        ReviewInline
    ]
    list_display = ("title", "author", "price")

admin.site.register(Book, BookAdmin)

```
In this version, `ReviewInline` is defined before it's used in `BookAdmin`. Python reads the file from top to bottom, so by the time `ReviewInline` is referenced in `BookAdmin`, Python already knows what `ReviewInline` is.
### Your Second Example

```
from django.contrib import admin

from .models import Book, Review


class BookAdmin(admin.ModelAdmin):
    inlines = [ReviewInline]
    list_display = ("title", "author", "price")


class ReviewInline(admin.TabularInline):
    model = Review


admin.site.register(Book, BookAdmin)

```
In this version, `ReviewInline` is referenced inside `BookAdmin` before it is defined. This will result in an error because Python has not yet encountered the `ReviewInline` class when it is referenced inside `BookAdmin`.

### Why the Order Matters

In Python, the interpreter needs to know what an object (like a function or class) is before it can be used. If you reference something before it is defined, Python will raise a `NameError` because it doesn't know what you're referring to.

### The Error You Would See

If you ran the second example, you would get a `NameError` like this:

`NameError: name 'ReviewInline' is not defined`

### Summary

- **First Example:** Works perfectly because everything is defined before it's used.
- **Second Example:** Fails because `ReviewInline` is used before it is defined.

In conclusion, in Python, the order of definitions does matter. Classes or functions must be defined before they are referenced in the code.

### Hashtags:
#python #codingfundamentals

### References (source material, similar notes):
