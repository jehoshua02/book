# Why Frontend and Backend?

Many places in this book we will be assuming a frontend/backend architecture. Back in the 2000s it was not uncommon for me to see an application whose html was generated 100% server side and javascript was sprinkled on just as an enhancing effect. This way of doing things is fine for websites not for web applications where data is being modified and displayed all over the place. Splitting the application into frontend and backend simplifies things greatly. The frontend and backend talk to eachother by sending data in json format.

This makes it easy to build highly interactive web applications and give the
user a good experience. It also means that the backend can be reused with
multiple frontends, such as a desktop application or a mobile application.

Reasons for splitting frontend and backend:

+ Separation of concerns, client worries about rendering. Server worries about
business logic and persistence. This simplifies maintenance.
+ Reuse of business logic in other frontends.
