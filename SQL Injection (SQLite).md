# SQL Injection (SQLite)

So, upon visiting this page, we can see an input field that lets us enter a movie name and it outputs the following: ![image](https://user-images.githubusercontent.com/111907811/228619799-f2767978-86ab-488f-8314-7f78b786481e.png)

Let's try and see if this page is vulnerable to SQL injection with this error:

`1'` and we can see it already displayed an error: ![image](https://user-images.githubusercontent.com/111907811/228619901-da9e434c-3968-4345-bd25-ec3ccefbe6d3.png)

As we can see the table is full of columns so we will use union based type, so let's try and inject this payload and see what happens:

`1' union select null,null,null,null,null,null; --`

And finally the SQL injection works: ![image](https://user-images.githubusercontent.com/111907811/228621709-63103757-059c-4ca2-9a17-d5b658f702fd.png)

Stay tuned for more!
