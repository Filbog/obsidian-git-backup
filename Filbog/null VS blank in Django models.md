- **null** is database-related. When a field has null=True, it can store a database entry as NULL, meaning no value.
- **blank** is validation-related. If blank=True, then a form will allow an empty value, whereas if blank=False then a value is required.
In practice, null and blank are commonly used together in this fashion so that a form allows an empty value, and the database stores that value as NULL. **BUT**, this depends on the field type. For example with string-types like TextField or CharField, we'd use ***""***, not *null*



#django #webdev #coding 