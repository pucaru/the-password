# The Password

## Difficulty: Easy | Catergory: Web
Write up for my challenge in LNC 2023!

>You stumble across a secret website that asks for your password...  
>http://thepassword.s.lagncra.sh/

Upon visiting the site, you will be prompted for a password.   

Solution: Key in `view-source:` in front of the URL.  

It allows you to view the HTML source file of the page you are viewing, and shows the following when viewed:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body> 
    <script src="password.js" defer></script>
</body>
</html>
```
