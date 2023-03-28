# XSS - Reflected (JSON)

So, upon visiting this page, I found just one input field and a hint that says "our master really loves Marvel movies :)".

I tried to write "Iron Man", it said: ![image](https://user-images.githubusercontent.com/111907811/228380465-e8ac59f4-3d5a-4911-b2b4-dbafae024965.png)

I tried to enter another movie, like "John Wick", the movie got returned as an output like this: ![image](https://user-images.githubusercontent.com/111907811/228380611-86a0f013-d650-45eb-a937-ff8d5a28ed59.png)

So, I tried to inject a simple HTML payload: 
`<h1>Hello</h1>`

And the XSS worked like below: ![image](https://user-images.githubusercontent.com/111907811/228380705-f654e39f-234c-40e8-8200-3f01c5b89687.png)

Stay tuned for more!
