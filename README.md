# Querying in Entity Framework Core  <img src="https://media.giphy.com/media/dYsB5F09z0fYvQLm9K/giphy.gif" width="60">
##### EF Core has a new feature in LINQ-to-Entities where we can include C# or VB.NET functions in the query. This was not possible in EF 6.

### 🔴 Eager Loading

Entity Framework Core supports eager loading of related entities, same as EF 6, using the `Include()` extension method and projection query. In addition to this, it also provides the `ThenInclude()` extension method to load multiple levels of related entities.


`FirstOrDefault()`  Returns first element of a sequence, or a default value if no element is found. It throws an error Only if the source is null.
