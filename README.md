# Learn JavaScript

- the 1ne Week
    
    ![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled.png)
    
    - Introduction and What Is JavaScript ?
    - How To Study The Course ?
    - Setting Up Environment And Tools
    - Work With Chrome Developer Tools
    - Where To Put The Code
    - Comments And Bad Practice
    - Output To Screen
    - Console Methods And Styling And Web API
    - What Is ECMAScript ?
    - 1. Introduction and What Is JavaScript ?
        - **What Is New ?**
            - Merge All Old Courses + New Content
            - New Quality
            - What About Old Content
        - **What Is JavaScript ?**
            - Scripting Or Programming Language
            - Working On Client Side And Server Side
            - Implement Complex Features On A Web Page By Making It Interactive
        - **What JavaScript Can Do ?**
            - Dynamically Update Content
            - Manipulating HTML And CSS
            - Animate Images And Content And Create Image Gallery
            - Manipulate And Validate Data
            - Control Multimedia [Audio, Video, Etc…]
            - Web Browser Games
            - Mobile Apps
        - **Content**
            - Core Language
            - DOM
            - BOM
            - OOP
            - ES6, ES7
            - Practice
        - **What I Need To Learn ?**
            - Learn HTML Language
            - Learn CSS Language
            - Finish Practice
            - Text Editor [ Visual Studio Code, Atom ]
            - Internet Browser [ Google Chrome, Firefox Developer Edition ]
            - Windows And Internet Knowledge
    - **2. How To Study The Course ?**
        - Focus
        - Always Search
        - Ask How To Fix Not Fix
        - Start Idea
        - Check Lessons Code [ [https://elzero.org/category/courses/js-course](https://elzero.org/category/courses/js-course) ]
        - Do The Assignments [ [https://elzero.org/category/assignments/js-assignments/](https://elzero.org/category/assignments/js-assignments/) ]
        - Submit On Group [ [https://www.facebook.com/groups/ElzeroStudy](https://www.facebook.com/groups/ElzeroStudy) ]
    - **3.  Setting Up Environment And Tools**
        
        **The most important additions to the Visual Studio code editor**
        
        - Bracket Pair Colorizer 2
        - Editor Config
        - EsLint
        - GitLens
        - Indent Rainbow
        - Live Server
        - Material Icon Theme
        - Path Intellisense
        - Prettier
        - VS Code Icons
        
        **You can develop your skills in Visual Studio Code by watching the clip in the link** 
        
        [https://www.youtube.com/watch?v=UuBRd7GeARg](https://www.youtube.com/watch?v=UuBRd7GeARg)
        
    - **4. Work With Chrome Developer Tools**
        
        **You can develop your skills and information in everything related to the Developer Tools from the following sources**
        
        - Chrome Dev Tools Official Website
            
            [https://developer.chrome.com/docs/devtools/](https://developer.chrome.com/docs/devtools/)
            
        - Chrome DevTools 20+ Tips and Tricks
            
            [https://www.keycdn.com/blog/chrome-devtools](https://www.keycdn.com/blog/chrome-devtools)
            
        - Chrome Developer Tools Main Concepts and Principles Explained
            
            [https://www.bitdegree.org/learn/chrome-developer-tools](https://www.bitdegree.org/learn/chrome-developer-tools)
            
        
        **You can develop your skills and get some information about Chrome Dev Tools from this clip** 
        
        [https://www.youtube.com/watch?v=_IKTGQosYMo&list=PLDoPjvoNmBAz30MJ4-4lxhmu668bFTcoj&index=20](https://www.youtube.com/watch?v=_IKTGQosYMo&list=PLDoPjvoNmBAz30MJ4-4lxhmu668bFTcoj&index=20)
        
    - **5. Where To Put The Code**
        
        Cannot read properties of null because arrangement 
        Because the language translator translates in order, when it comes to the <script tag> it doesn't see the element
        
        ```html
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta http-equiv="X-UA-Compatible" content="IE=edge">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Document</title>
            <script src="main.js"></script>
        </head>
        <body>
            <h1>Page Title</h1>
        </body>
        </html>
        ```
        
        ```jsx
        document.querySelector("h1").style.color = 'Blue';
        ```
        
        ![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%201.png)
        
        **It is better to write it this way**
        
        ```html
        <body>
            <h1>Page Title</h1>
            <script src="main.js"></script>
        </body>
        ```
        
        ```jsx
        document.querySelector("h1").style.color = 'Blue';
        ```
        
        ![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%202.png)
        
        **I can write before the element in HTML but I need to modify in JavaScript like this**
        
        ```jsx
        window.onload = function () {
          document.querySelector("h1").style.color = 'Blue';
        };
        ```
        
        <aside>
        ⚠️ All the codes that were written for testing only, 
        and you will learn them in the upcoming lessons,
        which is to test the location of the code for the JavaScript language
        
        </aside>
        
    - **6. Comments And Bad Practice**
        
        ```jsx
        // Wait The Window To Load
        window.onload = function () {
          // Single Line Comment
          document.querySelector("h1").style.color = "Blue"; // Single Line Comment
        };
        
        // Single Line Comment
        // Single Line Comment
        // Single Line Comment
        
        /* Single Line Comment */
        
        /* multiLine Comment
          1
          2
          3
          4
          5
        */
        
        //Press ("Ctrl" + "/") To Commend line
        ```
        
    - **7. Output To Screen**
        
        **Output To Screen**
          - window.alert()
          - document.write()
          - console.log()
        
        ```jsx
        window.alert("Hello From JS File");
        
        document.write("<h1>Hello <span>Page</span></h1>");
        
        console.log("Hello From JS File");
        ```
        
    - **8. Console Methods And Styling And Web API**
        
        **Console Methods**
          - log
          - error
          - table
        
          Web API
        
        **Styling Console**
          - Directive %c
        
        ```jsx
        console.log("Log");
        console.error("Error");
        console.table(["Osama", "Ahmed", "Sayed"]);
        console.log("Hello From %cJS %cFile", "color: red; font-size: 40px", "color: blue; font-size: 40px");
        ```
        
    - **9. What Is ECMAScript ?**
        
        ***ECMA Script***
        
        <aside>
        💡 ECMA SCript is a JavaScript standard meant to ensure the interoperability of web pages across different web browsers. 
        It is standardised by Ecma International according to the document ECMA-262. 
        ECMAScript is commonly used for client-side scripting on the World Wide Web, 
        and it is increasingly being used for writing server applications and services using Node.js.
        
        </aside>
        
        ```jsx
        var myName = "Osama";
        let myName = "Osama"; //ES6
        
        console.log("Hello " + myName);
        console.log(`Hello ${myName}`);  //ES6
        ```
        
        ***Important links for understanding ES***
        
        - **ECMA International (**[https://www.ecma-international.org/](https://www.ecma-international.org/)**).**
        - **ES6 Features (**[http://es6-features.org/](http://es6-features.org/)**).**
        - **Babel (**[https://babeljs.io/repl/](https://babeljs.io/repl/)**).**
        - **Wikipedia (**[https://en.wikipedia.org/wiki/ECMAScript](https://en.wikipedia.org/wiki/ECMAScript)**).**
    - ***Assignments***
        - Q1 You have more than one code, they all do the same job, 
        write a comment Multiple Lines explaining in English 
        what is the code that will not work with the reason
        
        ```html
        <!DOCTYPE html>
        <html lang="en">
        <head>
          <meta charset="UTF-8" />
          <meta http-equiv="X-UA-Compatible" content="IE=edge" />
          <title>assignment 1</title>
          <script>
        
            // Code One
            /*
            this code is to change the <h1> element color to red
            but it will not run because <script> tag is in the top of the page and the browser have not seen it 
            result: style = null
            */
        
            document.getElementById('el').style.color = 'red';
          </script>
          <script>
        
            // Code Two
        			/* same thing for the previous code
              but this one will run and change the text to red 
              becuase we use the function onload which is inside window object
              this function is useful to run our code after all the element are alredy in the page
              result: Page Title in red color
              */
        
            window.onload = function() {
        			document.getElementById('el').style.color = 'red';
            }
          </script>
        </head>
        
        <body>
          <h1 id="el">Page Title</h1>
          <script>
        
            // Code Three
            /*
            becurse the best place to put our js code are inside the <body> tag
            so this will replace the previous codes 
            result: Page Title in red color
            */
        
            document.getElementById('el').style.color = 'red';
          </script>
        </body>
        
        </html>
        ```
        
        - Q2 Create the element in the image inside the page by JavaScript language
            
            ![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%203.png)
            
        

![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%204.png)

![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%205.png)

# **the 6th week**

1.  **Array Big Introduction**
2. **Using Length With Array**
3. **Add And Remove From Array**
4. **Searching Array**
5. **Sorting Array**
6. **Slicing Array**
7. **Joining Arrays**
8. **Array Challenge**
9. Assignments
10. Search words

### 1. Array Big Introduction:

**Arrays**

- Create Arrays [Two Methods] new Array() + []
- Access Arrays Elements
- Nested Arrays
- Change Arrays Elements
- Check For Array Array.isArray(arr);

```jsx
let myFriends = ["Ahmed", "Mohamed", "Sayed", ["Marwan", "Ali"]];
console.log(`Hello ${myFriends[0]}`); // result {Hello Ahmed}
console.log(`Hello ${myFriends[2]}`); // result {Hello Sayed}
console.log(`${myFriends[1][2]}`);    // result {h}
console.log(`Hello ${myFriends[3]}`); // result {Hello Marwan, Ali}
console.log(`Hello ${myFriends[3][1]}`); // result {Hello Ali}
console.log(`${myFriends[3][1][2]}`); // result {i}
console.log(myFriends); // result {['Ahmed', 'Mohamed', 'Sayed', Array(2)]}
myFriends[1] = "Gamal";
console.log(myFriends); // result {['Ahmed', 'Gamal', 'Sayed', Array(2)}
myFriends[3] = "Sameh";
console.log(myFriends); // result {['Ahmed', 'Gamal', 'Sayed', 'Sameh'}
myFriends[3] = ["Omar", "Osama", "Ibrahim"];
console.log(myFriends); // result {['Ahmed', 'Gamal', 'Sayed', Array(3)}
```

### 2. **Using Length With Array:**

- **Array Methods**
  - Length

```jsx
// Index Start From 0 [ 0, 1, 2, 3 ]
let myFriends = ["Ahmed", "Mohamed", "Sayed", "Alaa"];
let myBest = ["Osama", "Islam", "Kareem", "Ibrahim", "Essam"];
console.log(myFriends.length); // result  4 
myFriends[6] = "Gamal";
console.log(myFriends); // result ["Ahmed", "Mohamed", "Sayed", "Alaa", empty x 2, "Gamal"]
myFriends[4] = "Omar";
// {myFriends[myFriends.length] = "Omar"}==={myFriends[4] = "Omar";}
console.log(myFriends); // result ["Ahmed", "Mohamed", "Sayed", "Alaa", "Omar"]
myBest[myBest.length] = "Omar";
console.log(myByst); // result ["Osama", "Islam", "Kareem", "Ibrahim", "Essam", "Omar"]
myBest[myBest.length - 1] = "Bakr";
console.log(myByst); // result ["Osama", "Islam", "Kareem", "Ibrahim", "Bakr", "Omar"]
myFriends.length = 2;
console.log(myFriends); // result ["Ahmed", "Mohamed"]
```

### 3. **Add And Remove From Array:**

- **Arrays Methods [Adding And Removing]**
  - unshift("", "") Add Element To The First
  - push("", "") Add Element To The End
  - shift() Remove First Element From Array
  - pop() Remove Last Element From Array

```jsx
let myFriends = ["Ahmed", "Mohamed", "Sayed", "Alaa"];
console.log(myFriends);                // result ["Ahmed", "Mohamed", "Sayed", "Alaa"]

myFriends.unshift("Osama", "Nabil");   //unshift Add Element To The First
console.log(myFriends);                // result ["Osama", "Nabil", "Ahmed", "Mohamed", "Sayed", "Alaa"]

myFriends.push("Samah", "Eman");       // push Add Element To The End
console.log(myFriends);                // result ["Osama", "Nabil", "Ahmed", "Mohamed", "Sayed", "Alaa", "Samah", "Eman"]

let first = myFriends.shift();        //shift() Remove First Element From Array
console.log(myFriends);                //result ["Nabil", "Ahmed", "Mohamed", "Sayed", "Alaa", "Samah", "Eman"]
console.log("First Name Is ${first}"); // result {First Name Is Osama}

let last = myFriends.pop();           //shift() Remove last Element From Array
console.log(myFriends);               //result ["Nabil", "Ahmed", "Mohamed", "Sayed", "Alaa", "Samah"]
console.log("First Name Is ${last}"); // result {First Name Is Eman}
```

### 4. **Searching Array:**

- **Arrays Methods [Search]**
  - indexOf(Search Element, From Index [Opt])
  - lastIndexOf(Search Element, From Index [Opt])
  - includes(valueToFind, fromIndex [Opt]) [ES7]

```jsx
let myFriends = ["Ahmed", "Mohamed", "Sayed", "Alaa", "Ahmed"];
console.log(myFriends);                          //result ["Ahmed", "Mohamed", "Sayed", "Alaa", "Ahmed"]

console.log(myFriends.indexOf("Ahmed"));         // result "0"
// indexOf >> ["0", "1", "2", "3", "4"] >> Searching from first to last
console.log(myFriends.indexOf("Ahmed", 2));      // result "4"

console.log(myFriends.lastIndexOf("Ahmed"));     // result "4"
// LastIndexOf >> ["0", "1", "2", "3", "4"] >> Searching from last to first
console.log(myFriends.lastIndexOf("Ahmed", -2)); // result "0"

console.log(myFriends.includes("Ahmed"));        // result "true"
console.log(myFriends.includes("Ahmed", 2));     // result "true"

if (myFriends.lastIndexOf("Osama") === -1) {
  console.log("Not Found");                      // result "Not Found"
}
console.log(myFriends.indexOf("Osama"));         // result "-1"
console.log(myFriends.lastIndexOf("Osama"));     // result "-1"
```

### 5. **Sorting Array:**

- **Arrays Methods [Sort]**
  - sort(Function [Opt])
  - reverse

```jsx
let myFriends = [10, "Sayed", "Mohamed", "90", 9000, 100, 20, "10", -20, -10];
console.log(myFriends);                   // result [10, "Sayed", "Mohamed", "90", 9000, 100, 20, "10", -20, -10]

console.log(myFriends.sort());            // result [-10, -20, 10, '10', 100, 20, '90', 9000, 'Mohamed', 'Sayed']
// sort() >> The order here is alphabetical, not from smallest to largest

console.log(myFriends.reverse());         // result ['Sayed', 'Mohamed', 9000, '90', 20, 100, '10', 10, -20, -10]
// reverse() >> It reverses the order

console.log(myFriends.sort().reverse());  // result ['Sayed', 'Mohamed', 9000, '90', 20, 100, '10', 10, -20, -10]
//sort().reverse() >> It arranges alphabetically and then reverses the order
```

### **6. Slicing Array:**

- **Arrays Methods [Slicing]**
  - slice(Start [Opt], End [Opt] Not Including End)
  --- slice() => All Array
  --- If Start Is Undefined => 0
  --- Negative Count From End
  --- If End Is Undefined || > Indexes => Slice To The End Array.length
  --- Return New Array
  - splice(Start [Mand], DeleteCount [Opt] [0 No Remove], The Items To Add [Opt])
  --- If Negative => Start From The End

```jsx
let myFriends = ["Ahmed", "Sayed", "Ali", "Osama", "Gamal", "Ameer"];
console.log(myFriends);                // result ['Ahmed', 'Sayed', 'Ali', 'Osama', 'Gamal', 'Ameer']

console.log(myFriends.slice());        // result ['Ahmed', 'Sayed', 'Ali', 'Osama', 'Gamal', 'Ameer']

console.log(myFriends.slice(1));       // result ['Sayed', 'Ali', 'Osama', 'Gamal', 'Ameer']
// slice() >> not included end >> ["0", "1", "2", "3", "4", "5"]
console.log(myFriends.slice(1, 3));    // result ['Sayed', 'Ali']

console.log(myFriends.slice(-3));      // result ['Osama', 'Gamal', 'Ameer']
// slice(-1) >> ["-6", "-5", "-4", "-3", "-2", "-1"]
console.log(myFriends.slice(1, -2));   // result ['Sayed', 'Ali', 'Osama']
console.log(myFriends.slice(-4, -2));  // result ['Ali', 'Osama']

console.log(myFriends);                // result ['Ahmed', 'Sayed', 'Ali', 'Osama', 'Gamal', 'Ameer']

// splice(Start[Mand], DeleteCount[Opt][0 No Remove], TheIteamsToAdd [Opt]);
myFriends.splice(0, 0, "Sameer", "Samara");
console.log(myFriends); // result ['Sameer', 'Samara', 'Ahmed', 'Sayed', 'Ali', 'Osama', 'Gamal', 'Ameer']

myFriends.splice(0, 1, "Sameer", "Samara");
console.log(myFriends); // result ['Sameer', 'Samara', 'Sayed', 'Ali', 'Osama', 'Gamal', 'Ameer']

myFriends.splice(1, 2, "Sameer", "Samara");
console.log(myFriends); // result ['Ahmed', 'Sameer', 'Samara', 'Osama', 'Gamal', 'Ameer']

```

### **7. Joining Arrays:**

- **Arrays Methods [Joining]**
  - concat(array, array) => Return A New Array
  - join(Separator)

```jsx
let myFriends = ["Osama", "Gamal", "Ameer"];
let myNewFriends = ["Samar", "Sameh"];
let schoolFriends = ["Haytham", "Shady"];
console.log(myFriends); // result ["Osama", "Gamal", "Ameer"]

let allFriends = myFriends.concat(myNewFriends, schoolFriends); 
console.log(allFriends);// result ["Osama", "Gamal", "Ameer", "Samar", "Sameh", "Haytham", "Shady"]

let allFriends = myFriends.concat(myNewFriends, schoolFriends, "Gamel"); 
console.log(allFriends);// result ["Osama", "Gamal", "Ameer", "Samar", "Sameh", "Haytham", "Shady", "Gamel"]

let allFriends = myFriends.concat(myNewFriends, schoolFriends, "Gamel", ["A", "B"]); 
console.log(allFriends);// result ["Osama", "Gamal", "Ameer", "Samar", "Sameh", "Haytham", "Shady", "Gamel", "A", "B"]

console.log(allFriends.join()); 
// result { Ahmed,Sayed,Ali,Osama,Gamal,Ameer,Samar,Sameh,Haytham,Shady,Gameel,A,B }

console.log(allFriends.join("")); 
// result { AhmedSayedAliOsamaGamalAmeerSamarSamehHaythamShadyGameelAB }

console.log(allFriends.join(" @ ")); 
// result { Ahmed @ Sayed @ Ali @ Osama @ Gamal @ Ameer @ Samar @ Sameh @ Haytham @ Shady @ Gameel @ A @ B }

console.log(allFriends.join("|")); 
// result {Ahmed|Sayed|Ali|Osama|Gamal|Ameer|Samar|Sameh|Haytham|Shady|Gameel|A|B}

console.log(allFriends.join("|").toUpperCase()); 
// result {AHMED|SAYED|ALI|OSAMA|GAMAL|AMEER|SAMAR|SAMEH|HAYTHAM|SHADY|GAMEEL|A|B}
```

### **8. Array Challenge:**

```jsx
let zero = 0;
let counter = 3;
let my = ["Ahmed", "Mazero", "Elham", "Osama", "Gamal", "Ameer"];

// Write Code Here
console.log(my); // ["Osama", "Elham", "Mazero", "Ahmed"];

console.log(my.slice("????")); // ["Elham", "Mazero"]

console.log(); // "Elzero"

console.log(); // "rO"
```

```jsx
let zero = 0;
let counter = 3;
let my = ["Ahmed", "Mazero", "Elham", "Osama", "Gamal", "Ameer"];
// Variables zero and counter They change every time
console.log(my.slice(zero, ++counter).reverse()); // result ['Osama', 'Elham', 'Mazero', 'Ahmed']
console.log(my.slice(++zero, --counter).sort());  // result ['Elham', 'Mazero']
console.log(my[--counter].slice(--zero, counter).concat(my[++zero].slice(counter))); // result {Elzero}
console.log(my[zero][++counter + zero].concat(my[counter][--zero].toUpperCase()));   // result {rO}
```

```jsx
*let* zero = 0;
let zero = 0;
let counter = 3;
let my = ["Ahmed", "Mazero", "Elham", "Osama", "Gamal", "Ameer"];
let n2 = my.length / counter; 
let n1 = counter - n2;
my.length = my.length - n2; my.reverse();
console.log(my);                                         // result ['Osama', 'Elham', 'Mazero', 'Ahmed']
console.log(my.slice(n1, counter));                      // result ['Elham', 'Mazero']
console.log(my[n1].slice(zero, n2) + my[n2].slice(n2));  // result {Elzero}
console.log(my[n2][n2+n2] + my[zero][zero]);             // result {rO}
```

```jsx
*let* zero = 0;
let counter = 3;
let my = ["Ahmed", "Mazero", "Elham", "Osama", "Gamal", "Ameer"];
let four = my.reverse().splice(zero, --counter);            // ["Osama", "Elham", "Mazero", "Ahmed"];
let sec = my.slice(Number(true), ++counter);                // ["Elham", "Mazero"]
let $num1 = Number(true); // 1 
let third = sec[Number(true)].slice(++$num1);               // "Elzero" 
console.log(my);                                            // result ['Osama', 'Elham', 'Mazero', 'Ahmed']
console.log(sec);                                           // result ['Elham', 'Mazero']
console.log(`${sec[zero].slice(zero, $num1)}${third}`);     // result {Elzero}
console.log(`${third.charAt($num1)}${third.charAt(counter).toUpperCase()}`);  // result {rO}
```

### **8. Assignments:**

Q1

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- يجب عمل الحل والمطلوب بطريقتين مختلفتين
- يمكنك كتابة ما تريد خارج ال
    
    Console 
    
    لتنفيذ المطلوب
    

```jsx
let myFriends = ["Ahmed", "Elham", "Osama", "Gamal"];
let num = 3;

// Method 1
console.log("Your Code Here"); // ["Ahmed", "Elham", "Osama"];

// Method 2
console.log("Your Code Here"); // ["Ahmed", "Elham", "Osama"];
```

```jsx
// Assignment Link ==> https://elzero.org/javascript-bootcamp-assignments-lesson-from-040-to-047/
let myFriends = ["Ahmed", "Elham", "Osama", "Gamal"];
let num = 3;
myFriends.length = num;
// Method 1
console.log(myFriends); // ["Ahmed", "Elham", "Osama"];

myFriends.pop();
// Method 2
console.log(myFriends); // ["Ahmed", "Elham", "Osama"];
```

Q2

- ممنوع إستخدام الأرقام نهائيا
- ممنوع إستخدام ال
    
     slice Method
    
- يمكنك كتابة ما تريد خارج ال
    
    Console 
    
    لتنفيذ المطلوب
    

```jsx
let friends = ["Ahmed", "Eman", "Osama", "Gamal"];

// Write Your Code Here

console.log(friends); // ["Eman", "Osama"]
```

```jsx
let friends = ["Ahmed", "Eman", "Osama", "Gamal"];

// Write Your Code Here
friends.shift();
friends.pop();

console.log(friends); // ["Eman", "Osama"]
```

Q3

- ممنوع إستخدام الأرقام نهائيا
- يجب كتابة سطر
    
    Code 
    
    واحد فقط لتخرج القيمة المطلوبة
    

```jsx
let arrOne = ["C", "D", "X"];
let arrTwo = ["A", "B", "Z"];
let finalArr = [];

// Write One Single Line Of Code

console.log(finalArr); // ["Z", "X", "D", "C", "B", "A"]
```

```jsx
let arrOne = ["C", "D", "X"];
let arrTwo = ["A", "B", "Z"];
let finalArr = [];

// Write One Single Line Of Code
finalArr = finalArr.concat(arrOne, arrTwo).sort().reverse();

console.log(finalArr); // ["Z", "X", "D", "C", "B", "A"]
```

Q4

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام الرقم 0 فقط
- يجب كتابة سطر
    
    Code 
    
    واحد فقط لتخرج القيمة المطلوبة
    

```jsx

let website = "Go";
let words = [`${website}ogle`, "Facebook", ["Elzero", "Web", "School"]];

console.log(
  words[website.length][0][website.length].toUpperCase() +
    words[website.length][0]
      .slice(website.length + Array.isArray(words))
      .toUpperCase()
); // ZERO
```

Q5

- كل ما عليك هو التأكد أن قيمة متغير
    
    needle
    
     موجود داخل ال 
    
    Array 
    
    المسماه 
    
    haystack
    
- يجب عمل الحل بثلاث طرق مختلفة
- قم بطباعة كلمة
    
    Found 
    
    في ال 
    
    Console 
    
    إذا كانت الكلمة موجودة
    

```jsx
let needle = "JS";
let haystack = ["PHP", "JS", "Python"];

// Write 3 Solutions
```

```jsx
let needle = "JS";
let haystack = ["PHP", "JS", "Python"];

haystack.includes(needle.toUpperCase())
  ? console.log("Found")
  : console.log(-1);
haystack.indexOf(needle.toUpperCase()) !== -1
  ? console.log("Found")
  : console.log(-1);
haystack.lastIndexOf(needle.toUpperCase()) !== -1
  ? console.log("Found")
  : console.log(-1);
```

- قم بكتابة
    
    Code 
    
    فيه ما تعلمته لتخرج النتيجة الموجودة في المثال
    
- يمنع كتابة اي أرقام نهائيا في اي مكان في الحل

```jsx
let arr1 = ["A", "C", "X"];
let arr2 = ["D", "E", "F", "Y"];
let allArrs = [];

// Your Code Here
allArrs = allArrs
  .concat(arr1.slice(arr1.length - true), arr2.slice(arr1.length - true))
  .sort()
  .join("")
  .toLowerCase();

console.log(allArrs); // fxy
```

### **9. Search words:**

- [JavaScript Array Methods](https://www.freecodecamp.org/news/the-javascript-array-handbook/)
- [JavaScript Array Data Type](https://www.tutorialrepublic.com/javascript-tutorial/javascript-data-types.php)

---

![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%206.png)

# **The 7th week**

1. Loop For And Concept Of Loop .
2. Looping On Sequences .
3. Nested Loops And Training’s .
4. Loop Control – Continue, Break, Label .
5. Loop For Advanced Examples .
6. Practice – Add Products To Page .
7. Loop – While .
8. Loop – Do, While .
9. Loop Challenge .

### 1. Loop For And Concept Of Loop :

- **Loop**
  - For
  for ([1] [2] [3]) {
    // Block Of Code
}
****  - For
  for ([1 initiation ] [2 condition] [3 Action]) {
    // Block Of Code
}

```jsx
for (let i = 0; i < 10; i++) {
  console.log(i);
}
```

### 2. Looping On Sequences :

- Loop
  - Loop On Sequences

```jsx
let myFriends = ["Osama", "Ahmed", "Sayed", "Ali", "Amira"];
let onlyNames = [];

console.log(myFriends[0]);
console.log(myFriends[1]);
console.log(myFriends[2]);
console.log(myFriends[3]);
console.log(myFriends[4]);

for (let i = 0; i < 5; i++) {
  console.log(i); // result "0", "1", "2", "3", "4"
  console.log(myFriends[0]); // result "Osama", "Osama", "Osama", "Osama", "Osama"
  console.log(myFriends[i]); // result "Osama", "Ahmed", "Sayed", "Ali", "Amira"
}

for (let f = 0; f < 6; f++) {
  console.log(myFriends[f]); // result "Osama", "Ahmed", "Sayed", "Ali", "Amira", "Undifined"
}

for (let e = 0; e < myFriends.length; e++) {
  console.log(myFriends[e]); // result "Osama", "Ahmed", "Sayed", "Ali", "Amira"
}

if (typeof myFriends[0] === "string") {
  onlyNames.push(myFriends[0])
}
if (typeof myFriends[1] === "string") {
  onlyNames.push(myFriends[1])
}
if (typeof myFriends[2] === "string") {
  onlyNames.push(myFriends[2])
}
if (typeof myFriends[3] === "string") {
  onlyNames.push(myFriends[3])
  }
console.log(onlyNames); // result ['Osama', 'Ahmed']

for (let p = 0; p < myFriends.length; p++) {
  if (typeof myFriends[p] === "string") {
    onlyNames.push(myFriends[p]); 
  }
};

console.log(onlyNames); // ['Osama', 'Ahmed', 'Sayed', 'Ali', 'Amira']
```

**Loop**
  - Nested Loops

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor"];
let colors = ["Red", "Green", "Black"];
let models = [2020, 2021];

for (let i = 0; i < products.length; i++) {
  console.log("#".repeat(15));
  console.log(`# ${products[i]}`);
  console.log("#".repeat(15));
  console.log("Colors: ");
  for (let j = 0; j < colors.length; j++) {
    console.log(`- ${colors[j]}`);
  }
  console.log("Models: ");
  for (let k = 0; k < models.length; k++) {
    console.log(`- ${models[k]}`);
  }
}
/*###############
# Keyboard
###############
Colors: 
- Red
- Green
- Black
Models: 
- 2020
- 2021
###############
# Mouse
###############
Colors: 
- Red
- Green
- Black
Models: 
- 2020
- 2021
............*/
```

### **5. Loop Control – Continue, Break, Label :**

- **Loop Control**
  - Break
  - Continue
  - Label

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor"];
let colors = ["Red", "Green", "Black"];

for (let i = 0; i < products.length; i++) {
console.log(products[i]); // result "Keyboard", "Mouse", "Pen"
if (products[i] === "Pen"){
	break;
}
console.log(products[i]); // result "Keyboard", "Mouse"
}
```

```jsx
let products = ["Keyboard", "Mouse", 10, 20, "Pen", "Pad", 30, 40, "Monitor"];
let colors = ["Red", "Green", "Black"];

for (let i = 0; i < products.length; i++) {
console.log(products[i]); // result "Keyboard", "Mouse", 10, 20, "Pen", "Pad", 30, 40, "Monitor"
if (typeof products[i] === "number") {
  continue;
}
console.log(products[i]); // result "Keyboard", "Mouse", "Pen", "Pad", "Monitor"
}
```

```jsx
*let* products = ["Keyboard", "Mouse", "Pen", "Pad","Monitor"];
let colors = ["Red", "Green", "Black"];
mainLoop: for (let i = 0; i < products.length; i++) {
  console.log(products[i]); // result "Keyboard"
  nestedLoop:for (let j = 0; j < colors.length; j++) {
    console.log(`-${colors[j]}`); // result "Red", "Green"
    if (colors[j] === "Green") {
      break nestedLoop
    }
  }
}
/* all result
Keyboard
- Red
- Green
*/ 
```

### **6. Loop For Advanced Examples :**

**Loop For Advanced Example**

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor", "iPhone"];
let i = 0;
for (let /*i = 0*/;/* i < products.length*/;/* i++*/) {
  console.log(products[i]);
  i++;
  if (i === products.length) {
    break;
    /* or "if (i === products.length) break;" */
  }
};
```

### **7. Practice – Add Products To Page :**

**Products Practice**

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor", "iPhone"];
let colors = ["Red", "Green", "Blue"];
let showCount = 3;

document.write(`<h1>Show ${showCount} products </h1>`);
for (let i = 0; i < products.length; i++){
  document.write(`<div>`);
  document.write(`<h3>[${i + 1}]${products[i]}</h3>`);
  for (j = 0; j < colors.length; j++){
    document.write(`<p>${colors[j]}</p>`);
  }
  document.write(`<p>${colors.join(" | ")}</p>`);
  document.write(`</div>`);
}
/* result
[1]Keyboard
Red
Green
Blue
Red | Green | Blue
.....
...
....
....
*/
```

### **8. Loop – While :**

- **Loop**
  - While

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor", "iPhone"];
let index = 0;
while (index < 10) {
  console.log(index); // result "0","1","2"
  index++;
  if (index === 3) {
    break;
  }
}
```

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor", "iPhone"];
let index = 0;

while (index < products.length) {
  console.log(products[index]); // result "Keyboard", "Mouse", "Pen", "Pad", "Monitor", "iPhone"
  index++;
}
```

### **9. Loop – Do, While :**

- **Loop**
  - Do / While

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor", "iPhone"];
let i = 0;

while (false){
console.log(i); // not any result because it is false
i++;
}
```

```jsx
let products = ["Keyboard", "Mouse", "Pen", "Pad", "Monitor", "iPhone"];
let i = 0;

do {
  console.log(i); // result "0"
  i++;
} while (false);
console.log(i); // result "1"
/* result "0", "1" */
```

### **10. Loop Challenge**

**Loop Challenge**

You have information about the admins and the employees in the company,

- we write the number of admin elements.
- When you put a stop anywhere in an Array, it ignores Stop and beyond from admin elements.
- Employees are distributed among the joint officials in alphabetical order by their names.

![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%207.png)

```jsx
let myAdmins = ["Ahmed", "Osama", "Sayed", "Stop", "Samera"];
let myEmployees = ["Amgad", "Samah", "Ameer", "Omar", "Othman", "Amany", "Samia", "Anwar"];

document.write(`<div>We Have X Admins</div>`);
```

```jsx
let myAdmins = ["Ahmed", "Osama", "Sayed", "Stop", "Samera"];
let myEmployees = ["Amgad", "Samah", "Ameer", "Omar", "Othman", "Amany", "Samia", "Anwar"];
let counter = 0;

document.write(`<div><h1>We Have ${myAdmins.indexOf("Stop")} Admins</h1></div>`);
mainLoop: for (let i = 0; i < myAdmins.length; i++){
  document.write(`<hr>`);
  if (i === myAdmins.indexOf("Stop")) {
    break mainLoop;
  }
  document.write(`<div><h1>The Admin For Team ${i + 1} is ${myAdmins[i]}</h1>`);
  document.write(`<h2> Team Members:</h2>`);
  nestedLoop: for (let j = 0; j < myEmployees.length; j++){
    if (myEmployees[j].charAt(0) === myAdmins[i][0]) {
      counter += 1;

    document.write(`<h3>${counter}-${myEmployees[j]}</h3>`);
  }
  }
}
```

### ***Assignment For Array:***

## **Q1**

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- يجب طباعة الأرقام وإستثناء الرقم 40 كما في المثال
- يجب إستخدام ال Loop For لعمل المطلوب

```jsx
let start = 10;
let end = 100;
let exclude = 40;

// Output
/*
10
20
30
50
60
70
80
90
100
*/
```

```jsx
let start = 10;
let end = 100;
let exclude = 40;

for(let i = start; i <= end; i+=start){
  if(i === exclude){
    continue;
  }  
  console.log(`${i}`);
}
```

## Q2

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- يجب طباعة الأرقام كما في المثال والتوقف عند الرقم 3
- إذا كان الرقم اصغر من 10 قم بطباعة صفر قبله
- يجب إستخدام ال Loop For لعمل المطلوب

```jsx
let start2 = 10;
let end2 = 0;
let stop2 = 3;

/* Output
10
09
08
07
06
05
04
03
*/
```

```jsx
let start = 10;
let end = 0;
let stop = 3;

for(let i = start; i >= stop; i--){
  if(i < start){
    console.log(`0${i}`);
  }
  else{
  console.log(`${i}`);
  }
}
```

## Q3

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- يجب طباعة الأرقام كما في المثال
- يجب إستخدام ال Loop For لعمل المطلوب

```jsx
let start = 1;
let end = 6;
let breaker = 2;

/* Output
1
-- 2
-- 4
2
-- 2
-- 4
3
-- 2
-- 4
4
-- 2
-- 4
5
-- 2
-- 4
6
-- 2
-- 4 */
```

```jsx
let start = 1;
let end = 6;
let breaker = 2;

for(let i = start; i <= end; i++){
  console.log(`${i}`);
  for(let j = breaker; j < end; j+=breaker){
      console.log(`-- ${j}`);
  }
}
```

## Q4

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- يجب طباعة الأرقام كما في المثال
- قم بكتابة الكود الخاص بك داخل اللووب فقط ولا تقم بالتعديل على أي شيء آخر
- يجب إستخدام ال Loop For لعمل المطلوب

```jsx
let index = 10;
let jump = 2;
let end = 0;

for (;;) {
  // Write Your Code Here
}

// Output
10
8
6
4
```

```jsx
let index = 10;
let jump = 2;
let end = 0;

let i = index;
for (;;) {
  if(i > jump){
    console.log(`${i}`);
    i-=jump;
  }  
  else{
    break;
  }
}
```

## Q5

- ممنوع إستخدام الأرقام نهائيا ولا الحروف ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- يجب طباعة الأسماء كما في المثال مع وضع رقم قبل كل قيمة بطريقة ديناميكية
- قم بإسثتناء الأسماء التي تبدأ بحرف A
- يجب إستخدام ال Loop For لعمل المطلوب

```jsx
let friends = ["Ahmed", "Sayed", "Eman", "Mahmoud", "Ameer", "Osama", "Sameh"];
let letter = "a";

/* Output
"1 => Sayed"
"2 => Eman"
"3 => Mahmoud"
"4 => Osama"
"5 => Sameh"
*/
```

```jsx
let friends = ["Ahmed", "Sayed", "Eman", "Mahmoud", "Ameer", "Osama", "Sameh"];
let letter = "a";

counter = letter.length ;
for(let i = letter.length - letter.length ; i < friends.length ; i++){
  if(friends[i][0] === letter.toUpperCase()){
    continue;
  }
  else{
    console.log(`"${counter} => ${friends[i]}"`);
    counter++;
  }  
}
```

## Q6

- ممنوع إستخدام الأرقام أو الحروف نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- المطلوب بإستخدام اللووب تحويل الحروف الكبير لصغيرة والعكس. شاهد المثال
- يجب إستخدام ال Loop For لعمل المطلوب

```jsx
let start = 0;
let swappedName = "elZerO";

/* Output
"ELzERo"
*/
```

```jsx
let start6 = 0;
let swappedName = "elZerO";
let swappedNameFinished="";

for(let i = start6; i < swappedName.length; i++){
  if(swappedName[i] === swappedName[i].toUpperCase()){
    swappedNameFinished += swappedName[i].toLowerCase();
  }
  else{
    swappedNameFinished += swappedName[i].toUpperCase();
  }
}
console.log(`${swappedNameFinished}`);
```

## Q7

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- المطلوب طباعة الأرقام فقط من أول الرقم إثنين للنهاية
- فكر قليلا بالمنطق كيف ستجعل ال Loop يتجاهل الرقم 1
- يجب إستخدام ال Loop For لعمل المطلوب

```jsx
let start = 0;
let mix = [1, 2, 3, "A", "B", "C", 4];

/* Output
2
3
4 */
```

```jsx
let start = 0;
let mix = [1, 2, 3, "A", "B", "C", 4];

for (let i = start; i < mix.length; i++){
  if(typeof mix[i] === "string"){
    continue;
  }
  else if (mix[i] === 1) {
    continue;
  }
  else{
    console.log(`${mix[i]}`)   
  }
}
```

## Q8

- ممنوع إستخدام الأرقام نهائيا ويمكنك إستخدام قيم المتغيرات مع ما تعلمته لتنفيذ المطلوب
- يجب عدم طباعة الأرقام ولا الاسماء التي تبدأ بحرف A
- يجب إستخدام ال Loop While لعمل المطلوب

```jsx
let friends = ["Ahmed", "Sayed", "Ali", 1, 2, "Mahmoud", "Amany"];
let index = 0;
let counter = 0;

// Output
"1 => Sayed"
"2 => Mahmoud"
```

```jsx
let friends = ["Ahmed", "Sayed", "Ali", 1, 2, "Mahmoud", "Amany"];
let index = 0;
let counter = 0;

while(index < friends.length){
  if(typeof friends[index] === "number" || friends[index][0] === "A"){
    index++;
    continue;
  }
  else{
    console.log(`"${++counter} => ${friends[index]}"`);
    index++;
  } 
}
```

![Untitled](Learn%20JavaScript%205388d82320be404e91265faaa13aba88/Untitled%208.png)

# **The 8th week**

1.  Function Intro And Basic Usage
2.  Function Advanced Examples
3.  Function Return Statement And Use Cases
4.  Function Default Parameters
5.  Function Rest Parameters
6.  Function Ultimate Practice
7.  Random Arguments Function Challenge

### **1.  Function Intro And Basic Usage :**

Function
  - What Is Function ?
  - User-Defined vs Built In
  - Syntax + Basic Usage
  - Parameter + Argument
  - Practical Example

- ***What Is Function ?***

functionis a block of code designed to perform a particular task, 

it applies the principle of DRY (Don't repeat Yourself )

- ***User-Defined vs Built In***

Built-in function is a feature in the language that we are ready to use.

user defined function is the function the user creates it

```jsx
console.log(typeof console.log); // result "function"
```

- ***Syntax + Basic Usage***

```jsx
function sayHello() {
  console.log(`Hello Osama`);
}
sayHello();
```

- ***Parameter + Argument***

***parameter:-*** is the variable that is written inside the function to perform the task.

***Argument:-*** is the value of the variable.

```jsx
function sayHello("Enter Parameter") {
  console.log(`Hello Osama`);
}
sayHello("Argument");
// or
function sayHello("Enter Variable") {
  console.log(`Enter the Task`);
}
sayHello("value");
```

- ***Practical Example***

```jsx
function sayHello(userName) {
  console.log(`Hi ${userName}`);
}
sayHello("Osama");
sayHello("Sayed");
sayHello("Ali");
```

### **2. Function Advanced Examples**

```jsx
function sayHello(userName, age) {
  if (age < 20) {
    console.log(`App is Not Suitable For You`);
  } else {
    console.log(`Hello ${userName} Your Age is ${age}`);
  }
}
sayHello("Osama", 38);  // result "Hello Osama Your Age is 38"
sayHello("Sayed", 40);  // result "Hello Sayed Your Age is 40"
sayHello("Ali", 18);    // result "App is Not Suitable For You"
```

```jsx
function generateYears(start, end) {
  for (let i = start; i <= end; i++) {
    console.log(i);
  }
}
generateYears(2014, 2021); // result "2014, 2015, 2016, 2017, 2018, 2019, 2020", "2021"
```

```jsx
function generateYears(start, end,exclude) {
  for (let i = start; i <= end; i++) {
if (i === exclude){
	countine;
}
    console.log(i);
  }
}
generateYears(2014, 2021, 2020); // result "2014, 2015, 2016, 2017, 2018, 2019, 2021"
```

### **3. Function Return Statement And Use Cases**

- Function
  - Return
  - Automatic Semicolon Insertion [No Line Terminator Allowed]
  - Interrupting

1- Return

```jsx
function sayHello(userName) {
  return `Hello ${userName}`;
}
let result = sayHello("Osama");
console.log(result); // result "Hello Osama"
```

```jsx
function clac(num1, num2) {
  return num1 + num2;
}
let result = clac(10, 20);
console.log(result + 100); // result "130"
```

2- Automatic Semicolon Insertion [No Line Terminator Allowed]

```jsx
function clac(num1, num2) {
  return num1 + num2;
let x = 1;  // Unreachable code detected.
}
let result = clac(10, 20);
console.log(result + 100); // result "130"
```

```jsx
function clac(num1, num2) {
  return 
	num1 + num2;  // Unreachable code detected.
}
let result = clac(10, 20);
console.log(result + 100); // result "130"
```

3- Interrupting

```jsx
function generate(start, end) {
  for (let i = start; i <= end; i++){
    console.log(i); //result "10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20"
  }
}
generate(10, 20);

// interruptting

function generate(start, end) {
  for (let i = start; i <= end; i++){
    if (i === 15) {
      return `interruptting`;
    }
    console.log(i);//result "10, 11, 12, 13, 14, 15"
  }
}
generate(10, 20);
```

### **4. Function Default Parameters**

- Function
  - Default Function Parameters
  - Function Parameters Default [Undefined]
  - Old Strategies [Condition + Logical Or]
  - ES6 Method

1- Default Function Parameters,   

2- Function Parameters Default [Undefined]

```jsx
function sayHello(userName, age) {
  return `Hello ${userName} Your Age Is ${age}`
}
console.log(sayHello("Osama", 38)); // result "Hello Osama Your Age Is 38"
console.log(sayHello("Osama"));  // result Hello Osama Your Age Is undefined
```

3-  Old Strategies [Condition + Logical Or].

```jsx
function sayHello(userName, age) {
  if (age === undefined) {
    age = "Unknow";
  }
  return `Hello ${userName} Your Age Is ${age}`
}
console.log(sayHello("Osama", 38));  // result "Hello Osama Your Age Is 38"
console.log(sayHello("Osama"));  // result "Hello Osama Your Age Is Unknow"
```

```jsx
function sayHello(userName, age) {
  age = age || "Unknoen";
  return `Hello ${userName} Your Age Is ${age}`
}
console.log(sayHello("Osama", 38));  // result "Hello Osama Your Age Is 38"
console.log(sayHello("Osama"));  // result "Hello Osama Your Age Is Unknow"
```

4- ES6 Method.

```jsx
function sayHello(userName, age = "Unknown") {
  return `Hello ${userName} Your Age Is ${age}`
}
console.log(sayHello("Osama", 38));  // result "Hello Osama Your Age Is 38"
console.log(sayHello("Osama"));  // result "Hello Osama Your Age Is Unknow"
```

### **5. Function Rest Parameters**

- Function
  - Rest Parameters
  - Only One Allowed
  - Must Be Last Element

```jsx
function clac(num1, num2, num3) {
    return num1 + num2 + num3;
}
console.log(clac(10, 20, 30)); // result "60"
```

***1- Rest Parameters***

```jsx
function calc(...numbers) {
    for (let i = 0; i < numbers.length; i++){
        console.log(numbers[i]);
    }
}
console.log(calc (10, 20, 30, 40)); // result "10, 20, 30, 40"
```

```jsx
function calc(...numbers) {
    console.log(Array.isArray(numbers)); // result "true" >> then number is Array
}
console.log(calc(10, 20, 30, 40));
```

```jsx
function calc(...numbers) {
    let result = 0;
    for (let i = 0; i < numbers.length; i++){
        result += numbers[i]; // result = result + numbers[i]
    }
    return `Final Result is ${result}`;
}
console.log(calc (10, 20, 30, 40)); // result "Final Result is 100"
```

***2- Only One Allowed
3- Must Be Last Element***

```jsx
function calc(name+job + ...numbers) {  // "Rest Parameters[...numbers]" is only one Allawed 
																				// "Rest Parameters[...numbers]" is last Element
    for (let i = 0; i < numbers.length; i++){
        console.log(numbers[i]);
    }
}
console.log(calc (10, 20, 30, 40));
```

### **6. Function Ultimate Practice**
