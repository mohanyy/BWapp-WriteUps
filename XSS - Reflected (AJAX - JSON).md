# XSS - Reflected (AJAX/JSON)

Exactly like we did in  XSS - Reflected (JSON), there is one input field and a hint that says "our master really loves Marvel movies :)".

I tried to write "Iron Man", it said: ![image](https://user-images.githubusercontent.com/111907811/228381309-88567417-ec20-42e3-ba92-452d379b0ab2.png)

I tried to enter another movie, like "John Wick", the movie got returned as an output like this: ![image](https://user-images.githubusercontent.com/111907811/228381370-fb037888-504b-4ee2-8b04-c00853d37602.png)

So, I tried to inject a simple HTML payload: 

`<h1>Hello</h1>`

And the XSS worked like below: ![image](https://user-images.githubusercontent.com/111907811/228381445-db3b451c-9854-4d83-91c5-c68ec404b86e.png)

Stay tuned for more!
