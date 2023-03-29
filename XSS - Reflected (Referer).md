# XSS - Reflected (Referer)

So, upon visiting this page, I found no input fields or any button or anything, except this text, which is displaying my current referer: ![image](https://user-images.githubusercontent.com/111907811/228397740-90b89da2-4cd9-4b8e-9d37-eaf6f318b7e2.png)

I tried to view the page source but didn't find anything useful for me so I went to use the burpSuite to know the headers of the page found this: ![image](https://user-images.githubusercontent.com/111907811/228397846-2f2dddbb-a555-4e9b-9a3a-5950c7c0e026.png)

As we can see, it displays the referer in the referer header.

Let's try to change it and see what happens, after I removed the link and added this text, we can see it displayed it: ![image](https://user-images.githubusercontent.com/111907811/228397955-dce2eb29-2ae5-447b-9038-543c74eabbc4.png)

So, let's upload this simple payload and forward the request using burpSuite: 

`<script>alert('Hello')</script>`

And finally the XSS works as below: ![image](https://user-images.githubusercontent.com/111907811/228398079-0688bacf-ed9f-4443-9b5b-e7115329724e.png)

Stay tuned for more!
