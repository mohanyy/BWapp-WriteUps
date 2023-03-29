# SQL Injection - Blind - Time-Based

So, upon visting this page, we can see a single input field and when we add anything in it, nothing happens as the result is being sent by email: ![image](https://user-images.githubusercontent.com/111907811/228589473-88cfa12b-a073-4e42-939d-dede4657d0c6.png)

Now let's try to inject this payload to see if it works:

`1' or sleep(5)#`

And as we can see it fully works and website is now delayed: ![image](https://user-images.githubusercontent.com/111907811/228590287-a1647441-8823-4a9b-a2de-cd519c286e6e.png)


Stay tuned for more!
