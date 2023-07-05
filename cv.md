# My Curriculum Vitae
 Curriculum Vitae
> # Kseniya Ivanova
![Face Reveal](https://i.imgur.com/Bq4Y4AD.jpg)
> ## Age: 19

__
---
> ### Contacts
* [Telegram](https://t.me/kivaanka)
* [VK](https://vk.com/kivaanka)
* [GitHub](https://github.com/kivanka/CurriculumVitae)

__
---
> ## Something About Myself:
I am a student of Belarusian-Russian University, majoring in Software Engineering. I am from Belarus, Mogilev. I have experience in programming thanks to my university. I have made some course projects for two years studiyng. I am trying to study hard, because i want to work in IT-company

__
---
> ### My Skills:
1. C#
2. T-SQL (Microsoft SQL Server, Microsoft Access)
3. JavaScript
4. C++ (Basic skills)
5. Photoshop

__
---
> ### Language Skills:
1. English Level: B1 (According to EPAM English  Test), B1 (According to A1QA English Speaking and Grammar Test)
2. Russian Level: C2 (Native Speaker)
3. Belarussian Level: C2 (Native Speaker)

---
> ### Solved CodeWars Katas (Code Example)
* If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.
Finish the solution so that it returns the sum of all the multiples of 3 or 5 below the number passed in. Additionally, if the number is negative, return 0 (for languages that do have them).

* Note: If the number is a multiple of both 3 and 5, only count it once.
```js
function sumMultiples3And5(number) {
  if (number < 0) {
    return 0;
  }

  let sum = 0;
  for (let i = 1; i < number; i++) {
    if (i % 3 === 0 || i % 5 === 0) {
      sum += i;
    }
  }

  return sum;
}

```
* Write a function that takes an integer as input, and returns the number of bits that are equal to one in the binary representation of that number. You can guarantee that input is non-negative.

* Example: The binary representation of 1234 is 10011010010, so the function should return 5 in this case
```js
function countBits(num) {
  let count = 0;
  while (num > 0) {
    if (num & 1) {
      count++;
    }
    num >>= 1;
  }
  return count;
}

```
* Return the number (count) of vowels in the given string.
We will consider a, e, i, o, u as vowels for this Kata (but not y).
The input string will only consist of lower case letters and/or spaces.

```js
function countVowels(str) {
  const vowels = "aeiou";
  let count = 0;

  for (let char of str) {
    if (vowels.includes(char)) {
      count++;
    }
  }

  return count;
}
console.log(countVowels("hello"));      
console.log(countVowels("programming"));
console.log(countVowels("javascript")); 
console.log(countVowels("sky"));        

