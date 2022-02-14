# Querying in Entity Framework Core  <img src="https://media.giphy.com/media/dYsB5F09z0fYvQLm9K/giphy.gif" width="60">
##### EF Core has a new feature in LINQ-to-Entities where we can include C# or VB.NET functions in the query. This was not possible in EF 6.

Entity Framework Core supports eager loading of related entities, same as EF 6, using the `Include()` extension method and projection query. In addition to this, it also provides the `ThenInclude()` extension method to load multiple levels of related entities.

🔴`First()` returns the "first" element in the collection, for an optional condition. If a condition is passed to the function as a predicate, the method returns the first element in the list which satisfies the predicate function. If no elements satisfy the condition, it throws an exception.

🔴`FirstOrDefault()`  Returns first element of a sequence, or a default value if no element is found. It throws an error Only if the source is null.
