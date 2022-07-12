## Задача

**Project**: gradle

**Language**: Java

**Spring Boot**: 2.7.0 (последний стабильный на данный момент)



**Project Metadata:**

**Group**: SkillBox.com (домен, которому принадлежит ваша компания)

**Artifact**: users (сервис, отвечающий за пользователей)

**Name**: users

**Description**: описание функций сервиса

**Package name**: место, где будут ваши классы с логикой



**Packaging**: jar

**Java**: 11



В поле **Dependencies** добавьте **Spring Web, Spring Data JPA**. После этого скачайте проект.

Чтобы убедиться, что всё работает, создайте класс:

```
package com.example.springboot;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;
@RestController
public class HelloController {
    @GetMapping("/")
    public String index() {
        return "Hello world from users service!";
    }
}
```

После этого запустите проект и выполните в консоли:

curl localhost:8080



Этапы работы над задачей
Настройте проект с помощью веб-конфигуратора.
Создайте дополнительный класс, который позволит общаться с приложением из вне.
Запустите сервис и проверьте его работу.


Критерии оценки
Сервис создан с нужными конфигурациями.
Запущенный сервис отвечает на запрос из консоли curl localhost:8080.
