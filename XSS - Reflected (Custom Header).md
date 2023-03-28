# XSS - Reflected (Custom Header)

So, upon visiting this page, I found no input fields or any button or anything, except this text, which is talking about custom headers: ![image](https://user-images.githubusercontent.com/111907811/228386003-96370717-24cc-4bae-834a-f25484337bc8.png)

I tried to view the page source but didn't find anything useful for me so I went to use the burpSuite to know the headers of this page since it is talking about headers and found this: ![image](https://user-images.githubusercontent.com/111907811/228386167-247625e4-dd44-4422-8e85-b06429922668.png)

I tried to add a custom header called bWAPP like it says in the page and found out it does output stuff on the page when I forward the request like below: ![image](https://user-images.githubusercontent.com/111907811/228386482-c4558a01-f9d1-4ec8-aa06-de8cb43e92bd.png)

By also trying to inject a JavaScript payload to confirm more, we find out it does work like this by forwarding this request: ![image](https://user-images.githubusercontent.com/111907811/228386600-a28a5352-7ea2-4ea7-a3e7-5b18f02ae5df.png)

And finally the XSS works fine: ![image](https://user-images.githubusercontent.com/111907811/228386633-6afe4674-f28d-43af-8727-51a836011e80.png)

Stay tuned for more!
