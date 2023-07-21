
# DynamoDB Item
- An item is the core unit of data in DynamoDB
- It is composed of attributes, which are bits of data on the item. Attributes have types -- e.g., strings, numbers, 
  lists, sets, etc -- which must be provided when writing and querying Items
- A simple primary key uses a single attribute to identify an item
- A composite primary key uses a combination of two attributes to identify a particular item. The first attribute is a 
  partition key (also known as a "hash key") which is used to segment and distribute items across shards. The second 
  attribute is a sort key (also known as a "range key") which is used to order items with the same partition key. A 
  DynamoDB table with a composite primary key can use interesting query patterns beyond simple get / set operations
- An item is made up of attributes, which are different elements of data on a particular item. For example, an item in 
  the User table might have a Name attribute, an Age attribute, an Address attribute, and more