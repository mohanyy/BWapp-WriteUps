# XSS - Reflected (Eval)

So, upon visiting this page, I found out that it displays my current date and time, I tried to check the page source and found nothing useful for me: ![image](https://user-images.githubusercontent.com/111907811/228388949-655b9776-3cb2-4ca5-a276-fad95ad2ce6c.png)

I checked the link of the page and tried to remove the "?date=Date()" and found out it displayed this: ![image](https://user-images.githubusercontent.com/111907811/228389052-f734760a-a22d-4bc0-8e10-3a0babfc0ded.png)

So I realized the displayed date and time has something to do with the "Date()" function.

I tried to inject a simple JavaScript payload in it like this:
`?date=Date(alert('Hello'))`

And finally the XSS worked:![image](https://user-images.githubusercontent.com/111907811/228390540-8d73bc46-52be-47c6-8517-58665ef5973e.png)


Stay tuned for more!
