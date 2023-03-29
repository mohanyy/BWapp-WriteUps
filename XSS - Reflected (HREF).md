# XSS - Reflected (HREF)

So, upon visiting this page, I found just one input field which asks me to enter my name like below: ![image](https://user-images.githubusercontent.com/111907811/228394907-1f2f478c-30af-49af-9db7-fff6bcf6393f.png)

When I entered my name, It got returned as an output in the next page like this: ![image](https://user-images.githubusercontent.com/111907811/228394952-f59f8374-9ff9-4209-abf6-1e98cfcdbad7.png)

So, I tried to inject a XSS payload which is: 

`<IMG """><SCRIPT>alert("XSS")</SCRIPT>"\>`

and finally the XSS worked: ![image](https://user-images.githubusercontent.com/111907811/228395081-6d4387bc-0090-44de-a7fb-ed1c190440bf.png)

Stay tuned for more!
