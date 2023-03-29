# SQL Injection (CAPTCHA)

So, upon visiting this page, we can see a CAPTCHA that we have to bypass by writing it: ![image](https://user-images.githubusercontent.com/111907811/228613846-aef20242-e467-4bf0-9e99-475d2e1933d7.png)

It then redirects us to this page so we can enter a movie name and it outputs the following: ![image](https://user-images.githubusercontent.com/111907811/228614052-44c9f373-e9af-40fb-9a25-9d0fb97b3476.png)

Let's try and see if this page is vulnerable to SQL injection with this error:

`1'` and we can see it already displayed an error: ![image](https://user-images.githubusercontent.com/111907811/228614896-9da77e81-3e11-4a7c-aa03-d4dead3bd395.png)

As we can see the table is full of columns so we will use union based type, so let's try and inject this payload and see what happens:

`1' union select null,null,null,null,null,null,null#`

And finally the SQL injection works: ![image](https://user-images.githubusercontent.com/111907811/228615080-decc0f3f-5e10-4256-8b61-f451f312766d.png)

Stay tuned for more!
