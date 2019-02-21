# RepositoryTimings
Benchmarks for the InfoQ Article Implementation Strategies for the Repository Pattern with Entity Framework, Dapper, and Chain

In modern enterprise development it is common to use a multi-layered approach to building one’s data access layer (DAL). 
When using C#, the lowest layer of the DAL is almost always ADO.NET. 

However, that can be a clumsy library at times so it is common to layer upon it an ORM. 
Then to enable mocking and hide the ORM’s details, the whole DAL is wrapped inside a repository.

we'll be looking at techniques for building a repository using three different styles of ORM:

- **Entity Framework:** A tradition “full feature” or “OOP” style ORM
- **Dapper:** A lightweight micro-ORM that focuses primarily on result set mapping.
- **Tortuga Chain:** A fluent ORM based on functional programming concepts.
