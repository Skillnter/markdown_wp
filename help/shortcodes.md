# Shortcodes

Shortcodes are small pieces of code in WordPress that allow you to achieve a variety of tasks with little effort.

```HTML
  [testt id="1" name="example"] 
```

### These are the following 4 shortcodes:

- &rarr; **testt** : Shortcode for the custom form and operations.
- &rarr; **aq_package** : Shortcode for the packages list and operations.
- &rarr; **aq_footer_link** : Shortcode for the footer link.
- &rarr; **aq_erase_data** : Shortcode for the GDPR page for validating user and deleting user data.

___

### testt:

Shortcode for the custom form and operations. It accept two attribute `id` and `name`.

- &rarr; **id** (required): The `id` of the form.
```HTML
  [testt id="1" name="example"]
```
- &rarr; **name** (optional): The `name` of the form.
```HTML
  [testt id="1" name="example"]
```
___

### aq_package:

Shortcode for the packages list and operations.
```HTML
  [aq_package]
```

- &rarr; **message** (required): The message to come after the package has been selected. Default is:
  - &ordm; *Single* : You have already applied to this package.
  - &ordm; *Combo* : You have already applied to {package_name list} package.
```HTML
  [aq_package message="custom message."]
```
___

### aq_footer_link:

Shortcode for the footer link. The link will only be seen by logged in user. It accept three attribute `name`, `link` and `class`.

- &rarr; **name** (required): The name or text for the link.
```HTML
  [aq_footer_link link="http://example.com" name="example"]
```
- &rarr; **link** (required): The anchor tag link.
```HTML
  [aq_footer_link link="http://example.com" name="example"]
```
- &rarr; **class** (optional): The style class or classes for the link.
```HTML
  [aq_footer_link link="http://example.com" name="example" class="class1 class2"]
```
___

### aq_erase_data:

Shortcode for the GDPR page for validating user and deleting user data. In case the session is not set for the user or user is not logged in, the page will redirect to home page.
```HTML
  [aq_erase_data]
```
- &rarr; **class** (optional): The style class or classes for the link.
```HTML
  [aq_erase_data form="1"]
```
- &rarr; **message** (optional): The message to come after the data has been deleted. Default is *"You data has been deleted"*.
```HTML
  [aq_erase_data form="1" message="Custom Message to show"]
```










