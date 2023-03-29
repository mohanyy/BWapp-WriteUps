# XSS - Stored (Blog)

So, upon visiting this page, I found out an input field and a submit button, after trying to write anything in it, it displays as an output like this: ![image](https://user-images.githubusercontent.com/111907811/228399212-61551a43-a785-4a60-9168-3058b99407b7.png)

So, I tried to inject this simple payload:

`<script>alert("Hello")</script>`

and finally the XSS works: ![image](https://user-images.githubusercontent.com/111907811/228399338-c40b9ab9-60e8-4509-80fc-b970aa52eb33.png)

Stay tuned for more.
