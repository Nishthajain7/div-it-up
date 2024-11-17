# Variables and data types
### Challenge
   1. **== and === are different** <br>
   
      == compares only the values of the two variables irrespective of the data type whereas <br>
      === compares both the data type and values of two variables.
      
       ```
        console.log(17 == '17') // true
        console.log( 17 === '17') // false
       ```
  2. **Automatic Semicolon Insertion (ASI)** automatically inserts semicolons at the end of statements when they're missing. But this could throw an       error sometimes. For example:
     ```
     function getNumber() {
       return
       5;
     }
     console.log(getNumber());
     ```
     You might expect `getNumber()` to return 5, but it actually returns undefined. This happens because ASI inserts a semicolon right after the return statement, like this:
    
     ```
     function getNumber() {
       return
       5;
     }
     console.log(getNumber());
     ```
