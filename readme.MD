
# `filterPersons` Function

This repository contains a TypeScript function called `filterPersons` that filters an array of `Person` objects (`User` or `Admin`) based on their type and additional criteria. The function is type-safe and ensures that filtering is done correctly based on the provided arguments.

## `Usage.

### Function Signature.

```typescript
function filterPersons(persons: Person[], personType: 'user', criteria: Partial<Omit<User, 'type'>>): User[];
function filterPersons(persons: Person[], personType: 'admin', criteria: Partial<Omit<Admin, 'type'>>): Admin[];


`import { filterPersons, persons, logPerson } from './filterPersons';

// Filter users of age 23
const usersOfAge23 = filterPersons(persons, 'user', { age: 23 });
console.log('Users of age 23:');
usersOfAge23.forEach(logPerson);

// Filter admins of age 23
const adminsOfAge23 = filterPersons(persons, 'admin', { age: 23 });
console.log('Admins of age 23:');
adminsOfAge23.forEach(logPerson);.


Users of age 23:
 - Kate Müller, 23, Astronaut
 - Wilson, 23, Ball

Admins of age 23:
 - Agent Smith, 23, Anti-virus engineer


 git clone https://github.com/your-username/your-repo.git
cd your-repo

npm install

npm start


### `Key Features of the README

1. **Function Signature**: Clearly explains the overloaded `filterPersons` function.
2. **Usage Example**: Provides a practical example of how to use the function.
3. **Output**: Shows the expected output of the example.
4. **Code Structure**: Breaks down the code into interfaces, helper functions, and the main function.
5. **Installation**: Provides steps to clone and run the repository.
6. **Contributing**: Encourages contributions and provides guidelines.
7. **License**: Specifies the license for the project.`
