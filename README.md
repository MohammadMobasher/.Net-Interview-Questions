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
</details>

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change. tanks.

## License

[MIT](https://choosealicense.com/licenses/mit/)

