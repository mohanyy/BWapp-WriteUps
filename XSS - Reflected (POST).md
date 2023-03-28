# XSS - Reflected (POST)

Exactly like we did in Reflected (GET), there is a two input fields here, I tried to write anything in them and found it got returned as an ouput like below: ![image](https://user-images.githubusercontent.com/111907811/228378661-b8292302-3f5c-485c-a99f-4da447c8907e.png)

I tried to inject a simple JavaScript payload which is:

`<script>alert("Hello")</script>`

And it did work like below:

![image](https://user-images.githubusercontent.com/111907811/228379197-79901267-faea-4945-9a55-b29211161aee.png)

Stay tuned for more!
