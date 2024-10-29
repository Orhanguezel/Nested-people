

```markdown
# Nested People Tasks

This repository contains tasks related to JavaScript objects and nested structures. Below are the details of each task and the solutions.

## Task 1

Given the following `person` object:

```javascript
let person = {
  name: "Petra Morin",
  address: {
    delivery: {
      street: "371-7636 Nulla Road",
      zip: "83-315",
      country: "Germany",
    },
    billing: {
      street: "123-999 Fake Street",
      zip: "12345",
      country: "Germany",
    },
  },
  hobbies: ["drums", "skating", "comics"],
  languages: [
    { name: "German", level: 5 },
    { name: "English", level: 4 },
    { name: "Spanish", level: 2 },
  ],
};
```

### Task 1.1
Print the zip code of the billing address.

**Solution:**
```javascript
console.log(`Zip: ${person.address.billing.zip}`);
```

**Expected Output:**
```
12345
```

### Task 1.2
Print the last hobby.

**Solution:**
```javascript
console.log(person.hobbies[person.hobbies.length - 1]);
```

**Expected Output:**
```
comics
```

### Task 1.3
Print the name and level of the second spoken language.

**Solution:**
```javascript
console.log(`${person.languages[1].name}: ${person.languages[1].level}`);
```

**Expected Output:**
```
English: 4
```

### Task 1.4
Print all information related to the delivery address.

**Solution:**
```javascript
console.log(`Street: ${person.address.delivery.street}
Zip: ${person.address.delivery.zip}
Country: ${person.address.delivery.country}`);
```

**Expected Output:**
```
Street: 371-7636 Nulla Road
Zip: 83-315
Country: Germany
```

### Task 1.5
Using a loop, print all the hobbies.

**Solution:**
```javascript
console.log(`Hobbies: \n-${person.hobbies.join("\n-")}`);
```

**Expected Output:**
```
Hobbies: 
- drums
- skating
- comics
```

### Task 1.6
Using a loop, list all known languages with a level less than 5.

**Solution:**
```javascript
for(let i = 0; i < person.languages.length; i++) {
  if(person.languages[i].level < 5) {
    console.log(`${person.languages[i].name}: ${person.languages[i].level}`);
  }
}
```

**Expected Output:**
```
English: 4
Spanish: 2
```

---

## Task 2

Given the following `users` array:

```javascript
const users = [
  {
    name: "Petra Morin",
    ...
  },
  {
    name: "Abel Ashley",
    ...
  },
  ...
];
```

### Task 2.1
Print the name and hobbies (separated by commas) from the last person on the list.

**Solution:**
```javascript
console.log(`${users[users.length-1].name}
Hobbies: ${users[users.length-1].hobbies.join(", ")}`);
```

**Expected Output:**
```
Skyler May
Hobbies: cycling, soccer, bouldering
```

### Task 2.2
Print the name and billing address of the second person.

**Solution:**
```javascript
console.log(`${users[1].name}
Billing address:
Street: ${users[1].address.billing.street}
Zip: ${users[1].address.billing.zip}
Country: ${users[1].address.billing.country}`);
```

**Expected Output:**
```
Abel Ashley
Billing address:
Street: 123 Lorem Square
Zip: 912098
Country: Mexico
```

### Task 2.3
Using loops, print all names with an index starting from 1.

**Solution:**
```javascript
for (let i = 0; i < users.length; i++) {
  console.log(`${i + 1}. ${users[i].name}`);
}
```

**Expected Output:**
```
1. Petra Morin
2. Abel Ashley
3. Aaron Cardenas
4. Felix Moreno
5. Skyler May
```

### Task 2.4
Print a message showing the name, delivery country, and first hobby for each person.

**Solution:**
```javascript
for (let i = 0; i < users.length; i++) {
  console.log(`${users[i].name} lives in ${users[i].address.delivery.country} and their favourite hobby is: ${users[i].hobbies[0]}.`);
}
```

**Expected Output:**
```
Petra Morin lives in Germany and their favourite hobby is: drums.
Abel Ashley lives in Mexico and their favourite hobby is: reading books.
Aaron Cardenas lives in France and their favourite hobby is: painting.
Felix Moreno lives in New Zealand and their favourite hobby is: jogging.
Skyler May lives in Singapore and their favourite hobby is: cycling.
```

### Task 2.5
Print each name and every language they know with a level greater than or equal to 4.

**Solution:**
```javascript
for (let i = 0; i < users.length; i++) {
  console.log(`${users[i].name} speaks fluently:`);
  for (let j = 0; j < users[i].languages.length; j++) {
    if (users[i].languages[j].level >= 4) {
      console.log(`- ${users[i].languages[j].name}`);
    }
  }
}
```

**Expected Output:**
```
Petra Morin speaks fluently:
- German
- English

Abel Ashley speaks fluently:
- Spanish
- English

Aaron Cardenas speaks fluently:
- French
- Spanish

Felix Moreno speaks fluently:
- English

Skyler May speaks fluently:
- Malay
- English
- Mandarin
```
```