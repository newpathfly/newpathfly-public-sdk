# newpathfly-public-sdk

This is the SDK for any Java based project to interact with [`newpathfly` API](https://newpathfly.ticketcombine.com/). The SDK is generated by [OpenAPI Generator](https://openapi-generator.tech/docs/generators/java "OpenAPI Generator") for Java. It provides model classes as well as API client based on reactive [Spring WebClient](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/reactive/function/client/WebClient.html "Spring WebClient").

## Setup

To add this SDK to your project, include a dependecy `ewpathfly-public-sdk` from `com.newpathfly`.

For example, for Maven based project, add

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-webflux</artifactId>
</dependency>

<dependency>
    <groupId>com.newpathfly</groupId>
    <artifactId>newpathfly-public-sdk</artifactId>
    <version>${newpathfly-sdk-version}</version>
</dependency>
```

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
