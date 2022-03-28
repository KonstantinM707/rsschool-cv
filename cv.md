## Konstantin Missyurkeyev
---
### Contacts
* Location: Nur-Sultan(Astana), Kazakhstan
* Phone number: +7 705 8743775
* E-mail: KonstantinM707@yandex.ru
* Discord: Achileus#4519 (@KonstantinM707)
---
### About Me

I am an electrical technician by education.
My hobby is developing the electronic devices.
At my first job, I worked with complex equipment that was controlled by software. I have not been able to access the source code to diagnose this equipment. I was very interested in how complex equipment works from the inside. So I started learning to program. 
In my next job, I was allowed to develop complex equipment myself and write code for it. It was the animatronics theater "Jungle" in Astana, where it was installed and operates to this day.
Also, I was interested in 3d modeling. So I started learning 3d modeling and visualization. I made some learning animations for the project called Mechanicum3D. In order to consolidate the studied material, I decided to combine the experience of modeling and programming and began to develop video games using the Unity engine. Now I want to learn how to make applications and games using web technologies.

---
### Skills
* C#, Pascal(Delphi), STL
* HTML5, CSS3
* JavaScript Basics
* PhotoShop, 3DSMax, Corel
---
### Code Example

**Find The Parity Outlier:** *You are given an array (which will have a length of at least 3, but could be very large) containing integers. The array is either entirely comprised of odd integers or entirely comprised of even integers except for a single integer N. Write a method that takes the array as an argument and returns this "outlier" N.*
```
using System.Collections.Generic;
using System.Linq;
using System;

public class Kata
{
  public static int Find(int[] integers)
  {
    IEnumerable<int> evens = from i in integers where i % 2 == 0 select i;
    IEnumerable<int> odds = from i in integers where i % 2 > 0 select i;

    if (evens.Count() > 1) return odds.First();
    if (odds.Count() > 1) return evens.First();

    return -1;
  }
}
```

**Find the odd int:** *Given an array of integers, find the one that appears an odd number of times.*
*There will always be only one integer that appears an odd number of times.*
*Examples*
*[7] should return 7, because it occurs 1 time (which is odd).*
*[0] should return 0, because it occurs 1 time (which is odd).*
*[1,1,2] should return 2, because it occurs 1 time (which is odd).*
*[0,1,0,1,0] should return 0, because it occurs 3 times (which is odd).*
*[1,2,2,3,3,3,4,3,3,3,2,2,1] should return 4, because it appears 1 time (which is odd).*
```
function findOdd(array) {
    let obj = {};
    for (let i = 0; i < array.length; i++) {
        if(obj[array[i]]) obj[array[i]]++;
        else obj[array[i]] = 1;
    }
    for(let num in obj){
        if(obj[num]%2 == 1) return Number(num);
    }
    return 0;
}
```
---
### Courses
* **Self-Learning**
---
### Languages
* English - Intermediate/Upper-intermediate
* Russian - Native
---