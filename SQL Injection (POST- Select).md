# SQL Injection (POST/Select)

So, upon visiting this page, we can see a Select input where we can select a movie and it displays it's data: ![image](https://user-images.githubusercontent.com/111907811/228638958-999bb108-7647-44da-8dce-8433538770e9.png)

Since there is nothing useful for us, let's try to intercept the request using BurpSuite: ![image](https://user-images.githubusercontent.com/111907811/228639085-2f7ccc8f-f8e7-4449-ba1a-c6f69e460d98.png)

We can see that the movie field in the request field, let's try to change it to `1'` and forward the request to see what happens: ![image](https://user-images.githubusercontent.com/111907811/228639364-41999703-734d-4816-91d6-89a046c35d41.png)

We can see that a MySQL error is displayed so, this page is vulnerable to SQL injection.

As we can see the table is full of columns so we will use union based type, so let's try and inject this payload and see what happens:

`15 union select null,null,null,null,null,null,null; --`

And finally the SQL injection works: ![image](https://user-images.githubusercontent.com/111907811/228641899-a2cacea7-6973-4441-9b76-e29df3077959.png)

Stay tuned for more!
