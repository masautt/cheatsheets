### Default Boilerplate

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Your title</title>
  </head>
  <body>
  
  </body>
</html>
```

### w/ Meta Tags

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
  <meta name="author" content="Your name">
  <meta name="description" content="Your description">
  <meta name="keywords" content="your,keywords">
  </head>
  <body>
  
  </body>
</html>
```

### w/ Favicon

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
  <link rel="shortcut icon" href="favicon.ico" type="image/vnd.microsoft.icon">
  </head>
  <body>
  
  </body>
</html>
```

### w/ Google Web Fonts

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
    <link rel="stylesheet" href="//fonts.googleapis.com/css?family=font1" type="text/css">
  </head>
  <body>
  
  </body>
</html>
```

### w/ Linked CSS Stylesheet

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
    <link rel="stylesheet" href="stylesheet.css" type="text/css">
  </head>
  <body>
  
  </body>
</html>
```

### w/ Embedded CSS Stylesheet

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
    <style type="text/css">
   

    </style>
  </head>
  <body>
  
  </body>
</html>
```

### w/ Google Analytics

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
  <script type="text/javascript">
   var _gaq = _gaq || [];
   _gaq.push(['_setAccount', '{ACCOUNT_NAME_HERE}']);
   _gaq.push(['_trackPageview']);
   (function()
   {
    var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
    ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
   })();
  </script>
  </head>
  <body>
  
  </body>
</html>
```


### w/ jQuery

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
  </head>
  <body>
  
  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js" type="text/javascript"></script>
  </body>
</html>
```

### w/ JavaScript that runs on DOM Ready

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
  </head>
  <body>
  
  <script type="text/javascript">
   function autorun()
   {
    
   }
   if (document.addEventListener) document.addEventListener("DOMContentLoaded", autorun, false);
   else if (document.attachEvent) document.attachEvent("onreadystatechange", autorun);
   else window.onload = autorun;
  </script>
  </body>
</html>
```

### w/ JavaScript that runs on Page Load

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
   <title>Your title</title>>
  </head>
  <body>
  
  <script type="text/javascript">
   function autorun()
   {
    
   }
   if (window.addEventListener) window.addEventListener("load", autorun, false);
   else if (window.attachEvent) window.attachEvent("onload", autorun);
   else window.onload = autorun;
  </script>
  </body>
</html>
```