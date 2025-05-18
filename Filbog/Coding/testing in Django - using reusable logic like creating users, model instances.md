 31-12-2024

To keep our test code DRY and make our lives easier, can define BaseTestClass with a setUp method containing users and model instances. Then we just inherit the BaseTestClass for all our EditView, CreateView etc tests. No need to repeat creating users and other stuff. Example in aerial-calendar repo
https://github.com/Filbog/aerial-calendar

### Hashtags:
#coding #webdev #django #testing

### References (source material, similar notes):
