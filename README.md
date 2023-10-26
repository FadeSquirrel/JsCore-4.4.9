# JsCore-4.4.9

## Зарегал юзера через POST-запрос на `https://blog.kata.academy/api/users`

### Отправил
```
{
  "user": {
    "username": "MoiseevMihail",
    "email": "superbelochko@gmail.com",
    "password": "888"
  }
}
```

### Результат
```
{
    "user": {
        "username": "moiseevmihail",
        "email": "superbelochko@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1M2E4MTEzZmYzY2M4MWIwMGRhY2E5ZSIsInVzZXJuYW1lIjoibW9pc2Vldm1paGFpbCIsImV4cCI6MTcwMzUxNjk0NywiaWF0IjoxNjk4MzMyOTQ3fQ.cVHgY6JIukW1Fsn-9Bfk3OTYb0Y6qGPyV5WQqhFVfiQ"
    }
}
```

## Залогинился через POST-запрос на `https://blog.kata.academy/api/users/login`

### Отправил
```
{
  "user": {
    "email": "superbelochko@gmail.com",
    "password": "888"
  }
}
```

### Результат
```
{
    "user": {
        "username": "moiseevmihail",
        "email": "superbelochko@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1M2E4MTEzZmYzY2M4MWIwMGRhY2E5ZSIsInVzZXJuYW1lIjoibW9pc2Vldm1paGFpbCIsImV4cCI6MTcwMzUxNzE3NywiaWF0IjoxNjk4MzMzMTc3fQ.Art9uPSGPqN3xfdSZ6J03nBt46xsE6HB09iifdnx-mE"
    }
}
```

## Отправил GET-запрос на `https://blog.kata.academy/api/user` для получения данных об авторизованом юзере

### Токен
```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1M2E4MTEzZmYzY2M4MWIwMGRhY2E5ZSIsInVzZXJuYW1lIjoibW9pc2Vldm1paGFpbCIsImV4cCI6MTcwMzUxNzE3NywiaWF0IjoxNjk4MzMzMTc3fQ.Art9uPSGPqN3xfdSZ6J03nBt46xsE6HB09iifdnx-mE
```

### Результат
```
{
    "user": {
        "username": "moiseevmihail",
        "email": "superbelochko@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY1M2E4MTEzZmYzY2M4MWIwMGRhY2E5ZSIsInVzZXJuYW1lIjoibW9pc2Vldm1paGFpbCIsImV4cCI6MTcwMzUxNzUwNywiaWF0IjoxNjk4MzMzNTA3fQ.WtY4Nvr9ojNen678J8WrE3bbUj1w93CnlxVQdrr5ewg"
    }
}
```
