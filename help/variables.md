# Variables

Variables are containers for storing data (values).

> &lt;input id='name' type='text' name='demo-name' value='{&#37;demo-name&#37;}'&gt;

A variable is linked with the `name` attribute of the form field. For example, {&#37;`demo-name`&#37;} variable will store the value of the `name='demo-name'` form field.
___

### Points to note:
- &rarr; General structure of a variable

> {&#37;name&#37;}

- &rarr; For `Auto-fill`, `Auto-select`, `Auto-check` variables can be used.

For text box, use value attribute to auto-fill

> &lt;input id='name' type='text' name='demo-name' value='{&#37;demo-name&#37;}'&gt;

For textarea, directly use variable inside textarea tags

> &lt;textarea&gt;{&#37;demo-name&#37;}&lt;/textarea&gt;

For radio, check and select, use `autochecked` attribute to auto-select or auto-check

> &lt;select name='demo-name'  autochecked='{&#37;demo-name&#37;}'&gt;

> &lt;input type='radio' name='demo-name' autochecked='{&#37;demo-name&#37;}'&gt;

> &lt;input type='checkbox' name='demo-name' autochecked='{&#37;demo-name&#37;}'&gt;
