java-restful-practice
=====================
Creating a RESTful Web Service From Maven Archetype
http://docs.oracle.com/cd/E19226-01/820-7627/giqdq/index.html

Rest tutorial
http://www.vogella.com/articles/REST/article.html
A RESTFul webservices are based on the HTTP methods and the concept of REST. A RESTFul webservice typically defines the base URI for the services, the supported MIME-types (XML, Text, JSON, user-defined,..) and the set of operations (POST, GET, PUT, DELETE)

http://your_domain:port/display-name/url-pattern/path_from_rest_class
This name is derived from the "display-name" defined in the web.xml file, augmented with the servlet-mapping url-pattern and the "hello" @Path annotation from your class file.

JAX-RS supports the automatic creation of XML and JSON via JAXB

@Path
@Path("/users")

@PathParam
파라미터를 나타내고 싶을 때, {}로 표현. @PathParam으로 접근
@Path("{name}")
public Response getUserByName(@PathParam("name")String name)

정규식표현

@Path("{id : \\d+}")//support digit only

