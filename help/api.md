# API

Third party APIs will be called after the second form submission.

___

### General Points:
- &rarr; **Type** : Refers to the type of request, i.e, GET, POST or REFRESH
- &rarr; **API URL** : Must be a valid URL with a protocol ( HTTP/HTTPS ).
```
  http://example.com/get 
```
or
```
  https://example.com/post
```
- &rarr; **Request Body** : Required for `POST` request type. Must be in the format of a query string, i.e, key-value pairs separated by `&`.
```
  key1=value1&key2=value2 
```
- &rarr; **Response Variable** : The variable name to compare value for success or failure of API. For example, for the below API response body, `status` will be the response variable to check the success or failure of API.
```
  {"id": "id_12345","status":"success"} 
```
- &rarr; **Message** : Message to compare for success or failure of API. For example, for the below API response body, `success` will be the message to check for success or failure of API.
```
  {"id": "id_12345","status":"success"} 
```
#### Only for `REFRESH` type:

- &rarr; **Token API URL** : Must be a valid URL with a protocol ( HTTP/HTTPS ). Similar to `API URL`.
- &rarr; **Token Post Body** : Must be in the format of a query string, i.e, key-value pairs separated by `&`. Similar to `Request Body`.
- &rarr; **Headers** : Headers to be sent with CRM APIs after getting token from `Token API`. Must be in the format of a query string, i.e, key-value pairs separated by `&`.
```
  key1=value1&key2=value2 
```
- &rarr; **Insert API** : Must be a valid URL with a protocol ( HTTP/HTTPS ). Similar to `API URL`.
- &rarr; **Insert Post Body** : Must be in the format of a query string, i.e, key-value pairs separated by `&`. Similar to `Request Body`.
- &rarr; **Update API** : Must be a valid URL with a protocol ( HTTP/HTTPS ). Similar to `API URL`.
- &rarr; **Update Post Body** : Must be in the format of a query string, i.e, key-value pairs separated by `&`. Similar to `Request Body`.

___

### Passing data:

- &rarr; **GET Requests** : Data can be passed as query string to GET requests as follows.
```
  http://example.com/get?key1=value1&key2=value2 
```
- &rarr; **POST Requests** : To add data to a POST request body, pass the key-value pairs as a query string into `Request body` form field. Data will automatically be converted to JSON object.
```
  http://example.com/get?key1=value1&key2=value2 
```
___

### Using Variable data:

- Replace the values with variables to pass dynamic values. Read more at [Variables Section](variables.md)

> example.com/get?key1={&#37;`variable1`&#37;}&key2={&#37;`variable2`&#37;}

or

> key1={&#37;`variable1`&#37;}&key2={&#37;`variable2`&#37;}`
  
___

### Using Pipes:

Use pipes to transform data.

- &rarr; **split:{index}** : pipe split the string with spaces and use the `index` to return the element at the particular index.


> example.com/get?key1={&#37;`name|split:0`&#37;}&key2={&#37;`name|split:1`&#37;} 


or

> key1={&#37;`name|split:0`&#37;}&key2={&#37;`name|split:1`&#37;} 






































