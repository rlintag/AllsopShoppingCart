# AllsopShoppingCart

Used .net core framework 2.1.4 (just because it is the only framework readily available on my machine)
Used xunit and moq for testing

The application is partitioned in the following sequence
1. ShoppingCart.Domain - Initially, I was supposed to create this with EF Core so I put in a domain layer for the use of DDD
2. ShoppingCart.Data - should do all the database connection. Although along the development I was careless to put in business logic on some of the code because of time constraint.
3. ShoppingCart.Application - should contain all business logic
4. ShoppingCart.Api - should be the interface of the application. most of the logic should be in the ShoppingCart.Application because it should be easily be transportable to another framework if needed be.
5. ShoppingCart.Application.Tests - I can only do the tests on the business logic 

I refrained from using third party libraries so that it would be easy to to just open the application, build, and run.
