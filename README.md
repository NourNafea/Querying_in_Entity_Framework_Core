# Querying in Entity Framework Core  <img src="https://media.giphy.com/media/dYsB5F09z0fYvQLm9K/giphy.gif" width="60">
##### EF Core has a new feature in LINQ-to-Entities where we can include C# or VB.NET functions in the query. This was not possible in EF 6.

## Here are the top 10 LINQ methods we use in our everyday C# Development

1️⃣ `First()`  Returns the "first" element in the collection, for an optional condition. If a condition is passed to the function as a predicate, the method returns the first element in the list which satisfies the predicate function. If no elements satisfy the condition, it throws an exception.

2️⃣ `FirstOrDefault()`  Works in a similar fashion as the First() method for positive cases in a collection - it returns the first element in the collection which satisfy an optional condition. The difference is in the negative case where there are no elements that satisfy the condition or the collection is empty - the method returns the default value for that type: NULL for reference types and respective default value for value types.

3️⃣ `Single()`  Returns the only element in the collection which satisfies a given condition. The rule is that there should be only a single element in the collection which satisfies the condition - for example a primary key in a table which is one and unique. If there are more than one elements which satisfy the condition for the Single() method, it throws an exception.

4️⃣ `SingleOrDefault()` Works similar to Single() method in the positive case - returns the only element which satisfies a given condition. But when this condition returns more than one element or the collection is empty, the method returns a default value - NULL for a reference type and respective default value for a value type.

5️⃣ `Any()` Returns a boolen value. The method just returns if there exists any element in the collection, which satisfies an optional condition. If no condition is provided, the method just returns if the collection is empty or not.

6️⃣ `Select()` Helps in projecting or mapping each element of the collection into a new sequence. If the elements of the collection are complex types (such as classes) consisting of properties, the method can be used to project one or more specific properties of each element in the collection into a new collection of elements.

7️⃣ `Where()` Returns all the elements from the collection which satisfy a given condition. One major difference between Where(), First() and Single() is that while Single() and First() methods return a single element from the collection, the Where() method returns all the elements in the collection for that condition that is passed for all these three methods.

8️⃣ `OrderBy()` Sorts the elements in a given collection in ascending order based on a given condition and returns the sorted collection. If we have to sort a collection of complex types based on more than one property of the elements, we can do so by chaining another function to OrderBy() called ThenBy().

9️⃣ `OrderByDescending()` Similar to OrderBy() method, except that the collection is sorted in a descending order.

🔟 `ToList()` Takes in an IEnumerable type and converts it to a List type. This conversion is important in cases where we would want to use a concrete type "List" in place of an abstract "IEnumerable" or when we want to use the methods available in a "List" type over a collection of an abstract type.
