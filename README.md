# Project-3  Dog Kennel

# Project Instructions: Dog and DogKennel Classes

## Overview
This project involves creating two classes: `Dog` and `DogKennel`. The `Dog` class represents individual dogs with specific attributes, while the `DogKennel` class manages a collection of `Dog` objects. Follow the instructions below to complete the project, ensuring that you include detailed documentation for each method, including descriptions, preconditions, and postconditions.

## Class 1: Dog

### Attributes
Each `Dog` object should have the following attributes:
- `name` (type `String`): The dog's name.
- `breed` (type `String`): The dog's breed.
- `weight` (type `double`): The dog's weight. Ensure this value is greater than or equal to zero.
- `medals` (type `int`): The number of medals the dog has won. Ensure this value is greater than or equal to zero.

### Methods
Create the following methods for the `Dog` class:

#### Constructor
```java
public Dog(String name, String breed, double weight, int medals)
```
**Description**: Initializes a new `Dog` object with the specified attributes.
- **Preconditions**: `weight` ≥ 0, `medals` ≥ 0.
- **Postconditions**: A `Dog` object is created with the specified attributes.

#### Getters
```java
public String getName()
public String getBreed()
public double getWeight()
public int getMedals()
```
**Description**: Return the respective attributes of the `Dog` object.
- **Preconditions**: None.
- **Postconditions**: Returns the value of the requested attribute.

#### Setters
```java
public void setName(String name)
public void setWeight(double weight)
public void setMedals(int medals)
```
**Description**: Set the respective attributes of the `Dog` object.
- **Preconditions**: `weight` > 0 for `setWeight`, `medals` ≥ 0 for `setMedals`.
- **Postconditions**: The attribute is updated with the new value.

#### Display Method
```java
public void displayDog()
```
**Description**: Displays the `Dog` object's name, breed, weight, and medal count in a readable format.
- **Preconditions**: None.
- **Postconditions**: Outputs the dog's details to the console.

## Class 2: DogKennel

### Attributes
- `kennel` (type `ArrayList<Dog>`): Stores the dogs currently in the kennel.

### Methods

#### Constructor
```java
public DogKennel()
```
**Description**: Initializes an empty `ArrayList` to hold `Dog` objects.
- **Preconditions**: None.
- **Postconditions**: A `DogKennel` object with an empty list of dogs is created.

#### Display Method
```java
public void displayKennel()
```
**Description**: Prints the index, name, breed, weight, and medal count of each dog in the kennel.
- **Preconditions**: None.
- **Postconditions**: Outputs the details of all dogs in the kennel.

#### Add Dog Method
```java
public void addDog(Dog d)
```
**Description**: Adds a new `Dog` to the kennel. Ensure the `Dog` object is not null before adding.
- **Preconditions**: `d` is not null.
- **Postconditions**: The `Dog` object is added to the `kennel` list.

#### Find Name Method
```java
public boolean findName(String dogName)
```
**Description**: Returns true if a dog with the specified name exists in the kennel.
- **Preconditions**: None.
- **Postconditions**: Returns true if the name is found, false otherwise.

#### Find Breed Method
```java
public int findBreed(String dogBreed)
```
**Description**: Returns the number of dogs of the specified breed in the kennel.
- **Preconditions**: None.
- **Postconditions**: Returns the count of dogs matching the breed.

#### Remove Method
```java
public boolean remove(String dogName)
```
**Description**: Removes all dogs with the specified name from the kennel and returns true if at least one dog was removed.
- **Preconditions**: None.
- **Postconditions**: The specified dogs are removed from the kennel.

#### Find Champions Method
```java
public ArrayList<Dog> findChampions(int medals)
```
**Description**: Returns a list of `Dog` objects with at least the specified number of medals.
- **Preconditions**: None.
- **Postconditions**: Returns a list of qualifying dogs or an empty list if none are found.

#### Find Light Method
```java
public ArrayList<Dog> findLight(double weight)
```
**Description**: Returns a list of `Dog` objects with a weight less than or equal to the specified weight.
- **Preconditions**: None.
- **Postconditions**: Returns a list of qualifying dogs or an empty list if none are found.

## Bonus Methods
These methods are optional.  You will not be given extra class time to do these methods.  

### Alpha Sorted Method
```java
public boolean alphaSorted()
```
**Description**: Checks if the dogs are sorted alphabetically by name.
- **Preconditions**: None.
- **Postconditions**: Returns true if the dogs are alphabetically sorted, false otherwise.

### Sort by Weight Method
```java
public void sortByWeight()
```
**Description**: Sorts the `dogs` list by weight from lightest to heaviest.
- **Preconditions**: None.
- **Postconditions**: The `dogs` list is sorted by weight.

### Champ Sort Method
```java
public boolean champSort()
```
**Description**: Checks if the dogs are sorted by the number of medals in descending order.
- **Preconditions**: None.
- **Postconditions**: Returns true if sorted by medals, false otherwise.

## Documentation Requirements
- **Description**: Provide a clear description of each method's purpose.
- **Preconditions**: Specify any conditions that must be true before the method is called.
- **Postconditions**: Describe the state of the program after the method has executed.
- **Comments**: Include logical comments to explain complex sections of code.

Ensure your code is well-documented and follows good coding practices. Happy coding!

