# XSS - Reflected (User-Agent)

So, upon visiting this page, I found no input fields or any button or anything, except this text, which is displaying my current User-Agent: ![image](https://user-images.githubusercontent.com/111907811/228398394-ee42d26d-d248-480a-9ce8-d08710960922.png)

I tried to view the page source but didn't find anything useful for me so I went to use the burpSuite to know the headers of the page and I found this: ![image](https://user-images.githubusercontent.com/111907811/228398450-7e8cfe6a-9a85-456e-a99f-bcdcbdc910bf.png)

As we can see, it displays my User-Agent in the user-agent header.

Let's try to change it and see what happens, after I my user-agent and added this text, we can see it displayed it: ![image](https://user-images.githubusercontent.com/111907811/228398561-5c225c20-b405-4eb8-a9e1-1bf85f90b0d7.png)

So, let's upload this simple payload and forward the request using burpSuite:

`<script>alert('Hello')</script>`

And finally the XSS works as below: ![image](https://user-images.githubusercontent.com/111907811/228398635-17543088-22bd-44c2-9b29-d90e5725f426.png)

Stay tuned for more!
