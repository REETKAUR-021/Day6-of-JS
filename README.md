// Array

let marks = [96 , 74 , 89 , 56];
console.log(marks);  //[ 96, 74, 89, 56 ]
console.log(marks.length);  //4
console.log(typeof marks); //object
console.log(marks[2]);   // 89

marks[3]=66;   // change the value
console.log(marks); //  [96, 74, 89, 66]

//loops in array
let numbers = [1 , 2 , 4  , 5, 6, 7, 8,];  

//for loop
for (let num = 0; num < numbers.length; num++){
    console.log(numbers[num]);
}

//for of loop
let cities = ["Delhi" , "Pune" , "Gurgaon" , "punjab"];
for(let city of cities){
    console.log(city);
}

//Array methods

let mark = ["45" , "56", "72" , "23" , "69"];

//push 
mark.push("79");   //add to end
console.log(mark);  //['45', '56', '72', '23', '69', '79']

//pop 
mark.pop();   //delete from end and return
console.log(mark);  //['45', '56', '72', '23', '69']

 //toString  / converts array to string
console.log(mark.toString());   //45,56,72,23,69

//concat()
let a = [1 , 2 , 3];
let b = [7 , 8,9];
let ab = a.concat(b);
console.log(ab); //[ 1, 2, 3, 7, 8, 9 ]

//unshift 
let i = [5 , 6, 7]; //add to start
i.unshift(4);
console.log(i);  //[ 4, 5, 6, 7 ]

//Shift 
i.shift();   //delete from start and return
console.log(i); //[ 5, 6, 7 ]

//slice / return a piece of the array
let number = [45 , 67 ,82 ,9 ];
console.log(number.slice(0 , 2));  //[ 45, 67 ]

//splice / change original array(add , remove , replace)
let arr = [1 , 3, 4, 5,6 ,7 ,8, 9];

//remove 
arr.splice(1 , 2);
console.log(arr); //[ 1, 5, 6, 7, 8, 9 ]

//add
arr.splice(1 , 0 , 23 , 42);
console.log(arr); //  [1, 23, 42, 5, 6,  7,  8, 9]

//replace
arr.splice(3 , 1 , 0);
console.log(arr); //  [1, 23, 42, 0, 6,  7,  8, 9]
