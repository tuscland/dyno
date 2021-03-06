## Pending

- Fixed a bug that did not allow the CLI tool to function using EC2 IAM Role-based credentials
- Adds a function to estimate the number of bytes required to store an item

## v0.15.1

- Batch write requests now return any keys that went unprocessed

## v0.15.0

- Add support for [document types (List and Map)][1], [Boolean][2], and [Null][3]
- Native JavaScript arrays will now transform into lists instead of sets
- Add `Dyno.createSet()`, which constructs sets (of number, string, or binary
  type) that transform to the DynamoDB wire format correctly.
- Drop support for using a wire-formatted object as input.
- Add `Dyno.serialize()` and `Dyno.deserialize()` to convert items to/from strings

[1]:http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DataModel.html#DataModel.DataTypes.Document
[2]:http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DataModel.html#DataModel.DataTypes.Boolean
[3]:http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DataModel.html#DataModel.DataTypes.Null
