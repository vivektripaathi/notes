# Web Application
It is an application program that is stored on a remote server delivered over the internet through a browser interface.
- It is a type of application that usually runs on a browser and uses various technologies to perform various tasks.
- For a web app to operate, it needs a web server, application server and database. Web servers manage the requests that come from a client, while the application server completes the requested task. A database stores any necessary information.
- Web applications typically have short development cycles and small development teams. Developers write most web apps in JavaScript, HTML5 or CSS. Client-side programming typically utilizes these languages, which help build an application's front-end. Server-side programming creates the scripts a web app will use. Languages such as Python, Java and Ruby are commonly used in server-side programming.

# Java Tomcat Server
- It is an open-source Java servlet container that implements many Java Enterprise Specs such as the Websites API, Java-Server Pages and last but not least, the Java Servlet.
- Full name Apache tomcat server.
- First implemented in 1998.
- Began with the reference implementation of java server page and java Servlet API.
- We use the HTTP server if we want to send simple data. If we want to send dynamic data or to make our website dynamic, we need to use the servlet. Hence, we need an HTTP server and what else we need is a container where we will run or servlet, so ==when we combine the HTTP server and the servlet (or we can say servlet container), they both combine to become a single server know as tomcat server==.

### Advantages of Tomcat Server
1. **Open Source**.
2. **Highly flexible.**
3. **Well Documented.
4. **Widely used application server.**
5. **Light Weight** : It is actually a very light application, even with the JavaEE's certification. However, it provides all necessary and standard functionalities required to operate a server, which means it gives very fast load and redeploys as compared to its various alternatives. 
### Disadvantages of Tomcat Server
1. It is not as fast as Apache server.
2. Memory Leak issue.
3. Issue with SSL Installation.
4. Basic User Interface.

# J2EE 
- It stands for Java 2 Platform, Enterprise Edition.
- It is a platform-independent, Java-centric environment used for building, deploying, and managing enterprise-level applications.
- J2EE provides a comprehensive set of APIs (Application Programming Interfaces), protocols, and services for developing multitiered, scalable, and secure applications.
**The main components of J2EE include:**
1. **Java Servlet:** Java language class used to process client request and generate dynamic web pages. Building block of web application and lies in the Web Layer.
2. **Java Service Pack (JSP):** Allows embedding of java code within HTML pages, enabling the creation of dynamic web contents. Lies in Web Layer.
3. **Enterprise JavaBeans (EJB):** Server-side components used for implementing the business logic of the application. Lies in Business Logic Layer.
4. **Java Message Services (JMS):** API that enables application to exchange messages asynchronously.  Lies in BLL.
5. **Java Transaction API (JTA):** It provides various interfaces to manages transaction among resources. Lies in Persistence Layer.
[Digram](https://www.educative.io/answers/what-is-j2ee)
**Here are some of the benefits of using J2EE:**
- **Portability:** J2EE applications are portable across different platforms and vendors.
- **Security:** J2EE applications are secure by design. They support a number of security features, such as authentication, authorization, and encryption.
- **Scalability:** J2EE applications are scalable. They can be easily scaled up or down to meet the needs of your business.
- **Reliability:** J2EE applications are reliable. They are designed to handle failures gracefully.