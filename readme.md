<h1 align="center" style="font-weight: bold;">TODO-LIST 💻</h1>

<p align="center">
 <a href="#tech">Technologies</a> • 
 <a href="#started">Getting Started</a> • 
  <a href="#routes">API Endpoints</a> •
 <a href="#license">License</a>
</p>

<p align="center">
    <b>Todo-list in java spring boot 🚀.</b>
</p>

<h2 id="technologies">💻 Technologies</h2>

- Java (Spring boot).

<h2 id="started">🚀 Getting started</h2>

Prerequisites necessary:

- [Java 17+](https://www.oracle.com/br/java/technologies/downloads/)

<h3>Cloning</h3>

```bash
git clone https://github.com/Marcos-Brhemem/todo-list-SPRING
```

<h3>Starting</h3>

```bash
mvn spring-boot:run or run using your preferred ide.
```

<h2 id="routes">📍 API Endpoints</h2>

​
| route               | description                                          
|----------------------|-----------------------------------------------------
| <kbd>GET /tasks/</kbd>     | retrieves information from all tasks see [response details](#get-tasks-detail)
| <kbd>POST /tasks</kbd>     | insert a new task see [response details](#post-insert-tasks-detail)
| <kbd>POST /users</kbd>     | register a new user see [request details](#post-users-detail)
| <kbd>PUT /tasks/{id}</kbd>     | edit the task see [response details](#put-edit-tasks-detail)




<h3 id="get-tasks-detail">GET /tasks</h3>

**RESPONSE**
```json
 {
        "id": "a85ca8f6-8f96-4dc8-bedb-4a6921e6e49d",
        "description": "Descrição teste",
        "title": "Title teste ",
        "startAt": "2025-03-05T12:30:00",
        "endAt": "2025-03-10T13:30:00",
        "priority": "ALTA",
        "idUser": "2272c555-5edf-4729-ae95-2667cbc7583b",
        "createdAt": "2025-03-04T14:13:25.086336"
    },
    {
        "id": "113be05c-44db-4423-a664-90a36eaa73d2",
        "description": "Descrição",
        "title": "Title",
        "startAt": "2025-03-05T12:30:00",
        "endAt": "2025-03-10T13:30:00",
        "priority": "ALTA",
        "idUser": "2272c555-5edf-4729-ae95-2667cbc7583b",
        "createdAt": "2025-03-04T14:13:40.695567"
    }
```

<h3 id="post-insert-tasks-detail">POST /tasks</h3>

**REQUEST**
```json
{
    "description": "Descrição",
    "title": "Title",
    "startAt": "2025-03-05T12:30:00",
    "endAt": "2025-03-10T13:30:00",
    "priority": "ALTA"
}
```

**RESPONSE**
```json
{
    "id": "113be05c-44db-4423-a664-90a36eaa73d2",
    "description": "Descrição",
    "title": "Title",
    "startAt": "2025-03-05T12:30:00",
    "endAt": "2025-03-10T13:30:00",
    "priority": "ALTA",
    "idUser": "2272c555-5edf-4729-ae95-2667cbc7583b",
    "createdAt": "2025-03-04T14:13:40.695567"
}
```

<h3 id="post-users-detail">POST /users</h3>

**REQUEST**
```json
{
  "name": "silva",
  "email": "silva@silva.com"
}
​
```

**RESPONSE**
```json
{
    "subscriptionNumber": 25,
    "designation": "http://codecraft.com/subscription/codecraft-summit-2030/11"
}
```


<h3 id="put-edit-tasks-detail">PUT /tasks/{id} </h3>

**REQUEST**
```json
{
  "title": "Modificando o title",
}
​
```

**RESPONSE**
```json
{
    "id": "a85ca8f6-8f96-4dc8-bedb-4a6921e6e49d",
    "description": "Descrição teste",
    "title": "Modificando o title",
    "startAt": "2025-03-05T12:30:00",
    "endAt": "2025-03-10T13:30:00",
    "priority": "ALTA",
    "idUser": "2272c555-5edf-4729-ae95-2667cbc7583b",
    "createdAt": "2025-03-04T14:13:25.086336"
}
```

<h2 id="license">📑 License</h2>

This project is under the MIT license.

---

Made with ♥ by Marcos Brhemem 👋