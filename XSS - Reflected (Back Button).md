# XSS - Reflected (Back Button)

So, upon visiting this page, I found out it doesn't have any input fields, it only has a button that says "Go Back" like below: ![image](https://user-images.githubusercontent.com/111907811/228383664-14e02c74-a33b-487f-a737-974c60a707b1.png)

When I tested it, it only returned me to the last the page I visited.

So, I tried to inspect element the button and found out this code: ![image](https://user-images.githubusercontent.com/111907811/228383753-41eab357-b97e-4e1d-8d6b-e24cb30a3736.png)

I tried to replace this code:

`onclick="document.location.href='http://192.168.5.129/bWAPP/xss_ajax_1-1.php'"`

With this: 

`onclick="alert('Hello there')"`

And finally the XSS code works like below: ![image](https://user-images.githubusercontent.com/111907811/228383931-ab14c640-3cc8-4c7a-9232-b3db01980905.png)

Stay tuned for more!
