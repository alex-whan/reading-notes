# Reading 29: Hash Tables

## Reading, Research, and Discussion

- A data structure used to store information
- Data is stored as "hashes"
- Hashes map to a specific location within the table
- Use key/value pairs
- Method of implementing an `associative array`
- Very fast read/write access thanks to precise index location of hash/key
- Each index of the array can hold many types of values
- Each index contains `buckets` - which each hold one key/value pair
- Buckets all start `null` and are overwritten when a hashCode is given
- `Collision` = when more than one key hashes to the same index
- Can remedy a collision with linked lists
- Internal methods:
  - add()
  - find()
  - contains()
  - getHash()

### Other Sources

- [HashTables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
