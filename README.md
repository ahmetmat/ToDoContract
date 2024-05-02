# Assistant Smart Contract

This is a simple to-do list smart contract implemented in the Motoko programming language for the Internet Computer blockchain. The contract allows users to add, complete, and clear to-do items.

## Getting Started

To use the Assistant smart contract, you will need to deploy it to the Internet Computer blockchain using the Internet Computer Software Development Kit (SDK). You can find more information on how to do this in the ICP Developer Documentation.

Once the contract is deployed, you can interact with it using the provided functions.

## Functions

- `getTodos() : [ToDo]`

  This function returns an array of all to-do items in the list.

- `addTodo(description: Text) : Nat`

  This function adds a new to-do item with the given description to the list and returns the unique ID of the new item.

- `completeTodo(id: Nat) : ()`

  This function marks the to-do item with the given ID as completed.

- `showTodos() : Text`

  This function returns a string representation of all to-do items in the list, with completed items marked with an exclamation point.

- `clearCompleted() : ()`

  This function removes all completed to-do items from the list.

## Data Structures

### `ToDo`

This struct represents a to-do item and has the following fields:

- `description`: The description of the to-do item as a string.
- `completed`: A boolean indicating whether the to-do item has been completed.

### `HashMap`

This is a built-in data structure provided by the Motoko standard library. It is a hash map that maps keys to values. In this contract, it is used to store the to-do items in the list.

### `Hash`

This is a built-in data structure provided by the Motoko standard library. It is a hash value that can be used to uniquely identify an object. In this contract, it is used to hash the keys of the to-do list hash map.

### `Nat`

This is a built-in data structure provided by the Motoko standard library. It is a natural number, which is an integer greater than or equal to zero. In this contract, it is used to represent the unique IDs of the to-do items.

### `Text`

This is a built-in data structure provided by the Motoko standard library. It is a string of characters. In this contract, it is used to represent the descriptions of the to-do items.

## Conclusion

The Assistant smart contract is a simple and easy-to-use to-do list application that can be deployed to the Internet Computer blockchain. It allows users to add, complete, and clear to-do items, and provides a string representation of the list for easy viewing.
