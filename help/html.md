# HTML

As per the requirements, HTML code is supported to structure and style the form.
___

### Points to note:

- &rarr; Format to enter HTML code form fields

```HTML
  <input id='name' type='text' name='demo-name' >
```

- &rarr; Only single quotes are allowed. Double quotes will be converted to single quotes during submission.

```HTML
  <input id="name" type="text" name="demo-name" > 
```
will become
```HTML
  <input id='name' type='text' name='demo-name' > 
```

-  &rarr; `<form>` tag is not allowed.
```HTML
  <form action="post.php" method="post" > 
```
Will not work.

- &rarr; For `Auto-fill`, `Auto-select`, `Auto-check` variables can be used. Variable is linked with the `name` attribute of the field. Read more at [Variables Section](help/variables.md)

> &lt;input id='name' type='text' name='demo-name' value='{&#37;demo-name&#37;}' &gt;




















