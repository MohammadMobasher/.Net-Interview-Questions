# .Net-Interview-Questions

Let us understand more about Web API by delving into these Web API Interview Questions, which will help you during a job interview or enhance your overall knowledge and understanding of this subject.

<details>
  <summary >
    Basic    
  </summary>

## 1. What are the main return types supported in Web API?

It does not have any specific data type. It can return data of any type depending upon the business requirement. There are many HTTP methods like GET, POST, PUT, etc., which can return data in different formats depending upon the use case.

- Void – It will return empty content
- HttpResponseMessage – It will convert the response to an HTTP message.
- IHttpActionResult – internally calls ExecuteAsync to create an HttpResponseMessage
- Other types – You can write the serialized return value into the response body

## 2. How do we limit access to methods with an HTTP verb in Web API?

An attribute has to be added/

- HttpGet
- HttpPost
- HttpDelete
- HttpPut

## 3. How can we register exception filter from the action?

We can register exception filter from action using following code:

```C#
[NotImplExceptionFilter]
public TestCustomer GetMyTestCustomer(int custid)
{
}
```

Or you can register exception filter globally using following code:

```
GlobalConfiguration.Configuration.Filters.Add (new MyTestCustomerStore.NotImplExceptionFilterAttribute());
```

[More Info.](https://learn.microsoft.com/en-us/aspnet/web-api/overview/error-handling/exception-handling)

## 4. How Can assign alias name for ASP.NET Web API Action?

We can give alias name for Web API action same as in case of ASP.NET MVC by using “ActionName” attribute as follows:

```C#
[ActionName("SaveStudentInfo")]
public void UpdateStudent(Student aStudent)
{
}
```

[More Info.](https://learn.microsoft.com/en-us/dotnet/api/system.web.mvc.actionnameattribute?view=aspnet-mvc-5.2)

## 5. What is CORS in Web API?

CORS (Cross-Origin Resource Sharing) is basically a mechanism that allows one to make requests from one website to another website in a browser that is normally not allowed by another policy called SOP (Same Origin Policy). It supports secure cross-origin requests and data transfers among clients or browsers and servers. Here, cross-origin request means requests coming from different origins. CORS simply resolves the same-origin restriction for JavaScript. One can enable CORS for web API using the respective web API package or OWIN middleware.

## 6. What are the differences between HTTP Get and HTTP Post?

A: GET and POST are two important verbs of HTTP.

- Parameters of GET are included in the URL; while parameters of POST are included in the body
- GET requests do not make any changes to the server; while POST does make changes to the server
- A GET request is idempotent; while a POST request is non-idempotent
- In a GET request, data is sent in plain text; binary and text data are sent

</details>

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change. tanks.

## License

[MIT](https://choosealicense.com/licenses/mit/)
