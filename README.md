# newpathfly-public-sdk

This is the SDK for any Java based project to interact with [`newpathfly` API](https://newpathfly.ticketcombine.com/). The SDK is generated by [OpenAPI Generator](https://openapi-generator.tech/docs/generators/java "OpenAPI Generator") for Java. It provides model classes as well as API client based on reactive [Spring WebClient](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/reactive/function/client/WebClient.html "Spring WebClient").

## Sample Code

```java
SearchRequest request = new SearchRequest();

// populate properties of search request here

ShoppingApi shoppingClient = new ShoppingApi();
shoppingClient.createSearch(request).subscribe(
  response -> {
  	// do something with the response here
  },
  exception -> {
  	// do something with the exception here
  }
)
```
