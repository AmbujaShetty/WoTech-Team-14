# WoTech-Team-14
A repository to add project files for WoTech Team 14, it will consist of java and python files.


Our team members are: Kaira, Lilian, Ambuja and Agy.

🙋‍♀️ Lilian is from Estonia and striving to become an expert in coding. 

🙋‍♀️ Agy is from Latvia, still on vacation mood and trying to catch-up 💻🔍

🙋‍♀️ Kaira is also from Estonia and learing coding so she could do a career change.

🙋‍♀️ Ambuja is from Latvia trying to be a techie.
## 11.07 JAVA TEAMWORK
```java
// Create an array in the endpoint, fill the array with data and access it from the URL
package com.datorium.Datorium.API;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.CrossOrigin;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestParam;
import org.springframework.web.bind.annotation.RestController;

import java.util.ArrayList;
import java.util.List;

@SpringBootApplication
@RestController
@CrossOrigin
public class DatoriumApiApplication {

    public static void main(String[] args) {
        System.out.println("asd");
        SpringApplication.run(DatoriumApiApplication.class, args);
    }


    @GetMapping("/list")
    public List<String> getList() {
        // Create an ArrayList
        ArrayList<String> list = new ArrayList<>();

        // Add some elements to the ArrayList
        list.add("Agy");
        list.add("Lilian");
        list.add("Ambuja");
        list.add("Kaira");

        // Return the ArrayList
        return list;
    }
}
```
