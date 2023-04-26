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

Clicking on the `password.js` link will direct you to:

```js
function promptPassword( )
{

var pwd = prompt ("Enter your Password: ");

while (pwd != 's0m3t1me$_1t_i5_pr377y_s1aY'){
alert("Login is incorrect");
pwd = prompt ("Enter your Password: ");
}

alert("Password is correct, the flag is LNC2023{s0m3t1me$_1t_i5_pr377y_s1aY}");

}
promptPassword();
```

where the password and the flag is located at.

Flag: `LNC2023{s0m3t1me$_1t_i5_pr377y_s1aY}`
