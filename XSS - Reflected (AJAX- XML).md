# XSS - Reflected (AJAX/XML)

So, upon visiting this page, I found just one input field and a hint that says "our master really loves Marvel movies :)".

I tried to write "Iron Man", it said: ![image](https://user-images.githubusercontent.com/111907811/228382486-92ab5d6e-3a26-4789-a411-ad2b0a86c9f1.png)

I tried to enter another movie, like "John Wick", the movie got returned as an output like this: ![image](https://user-images.githubusercontent.com/111907811/228382533-a87cf42f-dd6a-4620-b805-343a8a6912ce.png)

So, I tried to inject a simple HTML payload: 

`<h1>Hello</h1>`

But it did output "undefined" like below: ![image](https://user-images.githubusercontent.com/111907811/228382684-5efeaf96-aae5-4b5f-8dce-91902c339d45.png)

I tried to encode the payload with this website: http://htmlencode.net/

It did get me this code:

`&lt;h1&gt;Hello&lt;/h1&gt;`

I tried to use it this time and it did work like below:![image](https://user-images.githubusercontent.com/111907811/228382935-69bef680-e480-45ff-9e1c-1686e808ddfb.png)

Stay tuned for more!
