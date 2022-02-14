## Welcome to Steven's GitHub Pages

I am a 4th year university student in Math & Computer Science. I have experiences in java, linux and web development and am looking for a position of java developer/full stack web developer/devop. You probably have my resume if you come here. :)

### Demo Application

I have made a Demo Web Application using Angular + Spring Boot.
<a href="https://chengfengzhai.github.io/sandbox">https://chengfengzhai.github.io/sandbox</a>

It is a Web application with Angular + Spring Boot. The user is authorized with JWT(Json Web Token). 
The front end angular application is hosted on github pages, the back end Rest Server is hosted on Oracle Cloud VM free tier, the free SSL certificate for the Rest Server was created with letsEncrypt (https://letsencrypt.org/)
</br>
There are 2 links ( login and register, of course we can add more content available to public) in the public home page. After a user signs up with simple username + password and logs in with the cretentials entered in signup page, the application will display other 2 links: logout and products list. The user can click the link of poducts list and get a view of list of products, these products are retrieved via Restful web service from a backend server, which was deployed in a Oracle Cloud VM. The user can click the logout link to logout and return to original public home pages with links of signup and login.

### Source Code
You can find the source code of the Demo Application at:
<a href="https://github.com/chengfengzhai/sandbox">https://github.com/chengfengzhai/sandbox</a> </br>
The backend Rest API Server is based on Spring Boot, Spring Data JPA, Spring Security, JJWT (https://github.com/jwtk/jjwt). </br>
I have used 2 databases: embedded H2 for development and oracle cloud autonomous database for production. </br>
In DAO (Data Access Object) layer, other than the normal convienent repositories which direclty extend from spring JpaRepository, I have added some classes to extend the basic repositories so that I can add customized repository methods for particular repository and/or all repositories.</br>
An optional DTO (Data Transfer Object) package was added so that I can get fine control the Json Objects between REST client and REST server, otherwise, entity beans have to be used for both purpose of persistence and transfer object (json format between server and client) and sometimes could makes things complicated.
