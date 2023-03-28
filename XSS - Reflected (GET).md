# XSS - Reflected (GET)

So, to keep things short, I'm going to write about how did I exploit XSS - Reflected in bWapp.
I found two input fields, so I tried to write anything in them and found it got returned as an ouput like below:

![vmplayer_a30nW5LDVN](https://user-images.githubusercontent.com/111907811/228376147-d86d3120-6375-4e70-84c6-4afa0d800d26.png)

I tried to inject a simple JavaScript payload which is:

`<script>alert("Hello")</script>`

And it did work like below:

![image](https://user-images.githubusercontent.com/111907811/228376754-34143f76-ceee-4a63-a29b-dc617c5c9271.png)

Stay tuned for more!
