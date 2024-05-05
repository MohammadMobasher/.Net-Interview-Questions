# .Net-Interview-Questions

Let us understand more about Web API by delving into these Web API Interview Questions, which will help you during a job interview or enhance your overall knowledge and understanding of this subject.


<details>
  <summary >
    Basic    
  </summary>

## 1. What are the main return types supported in Web API?
It does not have any specific data type. It can return data of any type depending upon the business requirement. There are many HTTP methods like GET, POST, PUT, etc., which can return data in different formats depending upon the use case. 
* Void – It will return empty content
* HttpResponseMessage – It will convert the response to an HTTP message.
* IHttpActionResult – internally calls ExecuteAsync to create an HttpResponseMessage
* Other types – You can write the serialized return value into the response body


## 2. How do we limit access to methods with an HTTP verb in Web API?
An attribute has to be added/
* HttpGet
* HttpPost
* HttpDelete
* HttpPut


## 3. How can we register exception filter from the action?
We can register exception filter from action using following code:
```
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
</details>

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change. tanks.

## License

[MIT](https://choosealicense.com/licenses/mit/)

