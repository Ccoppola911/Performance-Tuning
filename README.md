# Performance-Tuning
Performance Tuning in MongoDB for Keeping Track of Products
MongoDB provides several tools and techniques for performance tuning. Some of the key ones are:

Indexes: Indexes can significantly improve query performance. Ensure that you have appropriate indexes on the fields that are frequently used in queries.

Query optimization: MongoDB provides several query optimization techniques such as query plan caching, index intersection, and covered queries. Use these techniques to optimize your queries.

Sharding: Sharding is a technique for distributing data across multiple servers. Sharding can improve query performance and increase the amount of data that can be stored in a MongoDB cluster.

Profiling: MongoDB provides a profiling feature that allows you to log the performance of database operations. Use this feature to identify slow queries and optimize them.

Replica sets: Replica sets provide high availability and fault tolerance. Use replica sets to ensure that your database is always available.
Here's an example of how to create an index on a collection in MongoDB:

Copy
db.collection.createIndex({ field: 1 })
This will create an ascending index on the field field of the collection collection.

Here's an example of how to enable profiling in MongoDB:

Copy
db.setProfilingLevel(1)
This will enable profiling at level 1, which logs all operations.

Here's an example of how to create a sharded collection in MongoDB:

Copy
sh.enableSharding("mydb")
sh.shardCollection("mydb.mycollection", { "shardkey": 1 })
