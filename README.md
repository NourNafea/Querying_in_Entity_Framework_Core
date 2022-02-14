# Querying in Entity Framework Core  <img src="https://media.giphy.com/media/dYsB5F09z0fYvQLm9K/giphy.gif" width="60">
##### EF Core has a new feature in LINQ-to-Entities where we can include C# or VB.NET functions in the query. This was not possible in EF 6.

Entity Framework Core supports eager loading of related entities, same as EF 6, using the `Include()` extension method and projection query. In addition to this, it also provides the `ThenInclude()` extension method to load multiple levels of related entities.

🔴`First()`  Returns the "first" element in the collection, for an optional condition. If a condition is passed to the function as a predicate, the method returns the first element in the list which satisfies the predicate function. If no elements satisfy the condition, it throws an exception.

🔴`FirstOrDefault()`  Works in a similar fashion as the First() method for positive cases in a collection - it returns the first element in the collection which satisfy an optional condition. The difference is in the negative case where there are no elements that satisfy the condition or the collection is empty - the method returns the default value for that type: NULL for reference types and respective default value for value types.

🔴`Single()`  Returns the only element in the collection which satisfies a given condition. The rule is that there should be only a single element in the collection which satisfies the condition - for example a primary key in a table which is one and unique. If there are more than one elements which satisfy the condition for the Single() method, it throws an exception.
