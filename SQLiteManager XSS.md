# SQLiteManager XSS

So, upon visiting this page we can see it doesn't have any input fields or anything except that the page uses SQLiteManager and a hint that says: **CVE-2012-5105**: ![image](https://user-images.githubusercontent.com/111907811/228592673-0bee1556-0640-4938-ace4-83f7ddf9f041.png)

Let's search about this hint and see what we will find.

We can find here that we can inject XSS code in main.php file: ![image](https://user-images.githubusercontent.com/111907811/228599856-fd9b06b0-6601-4b90-875f-ec9ef0a14bea.png)

Let's click on "SQLiteManager" word, it will redirect us to this page: ![image](https://user-images.githubusercontent.com/111907811/228600060-97a84299-ad2b-4e25-8f74-6d20ba73ab38.png)

If we inspect element the page source, we can see a main.php file: ![image](https://user-images.githubusercontent.com/111907811/228600204-153e0bdc-4541-4e29-881f-f98af1ae4b3b.png)

By going into this file and injecting this payload:

`&#039;"</script><script>alert(document.cookie)</script>`

We can see that the XSS fully works: ![image](https://user-images.githubusercontent.com/111907811/228606020-4b79d674-7ae2-491b-9799-21353200be46.png)

Refrence links: 
https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2012-5105
https://www.exploit-db.com/exploits/36509

Stay tuned for more!
