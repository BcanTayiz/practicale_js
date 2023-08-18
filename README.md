# Practicle Js

# Usage of Functions

<pre>
```
let list = [1,2,3,4,5,6]
let object = {'a':1,'b':2,'c':3}
const objectsList = [
    { name: 'John', age: 25 },
    { name: 'Alice', age: 30 },
    { name: 'Bob' ,age:2},
    {name: 'mikael',age:15}
];

const originalObject = {
    name: 'John',
    age: 30,
    hobbies: ['reading', 'swimming'],
    address: {
        city: 'New York',
        country: 'USA'
    }
};

console.log(pf.checkValue(list,[4,5]))
console.log(pf.modulerCheck(list,[1,2,3]))
console.log(pf.deleteValues(list,[1,2,3]))
console.log(pf.deleteValues(object,['a','b']))

console.log(pf.simpleValidateEmail('asdasd@index.com'))
console.log(pf.createRandomUuid4())
console.log(pf.objectSort(objectsList,'age'))
console.log(pf.hasKeyInObjectsList(objectsList,'name'))

console.log(pf.valueEmpty('0'))
console.log(pf.valueEmpty([]))
console.log(pf.deepClone(originalObject))

console.log(pf.checkValue(originalObject,'John'))
console.log(pf.transformBoolean('true'))

const currentDate = new Date();
console.log(pf.dateToString(currentDate, 'tr-TR', 'day-month-year', '/'));
console.log(pf.dateToString(currentDate, 'tr-TR', 'month-year', '-'));
console.log(pf.dateToString(currentDate, 'tr-TR', 'month-day', '.'));

const originalString = 'This is an example string that we want to split into multiple lines based on word count.';
const wordCount = 5;
const multiLineHTML = pf.convertToMultilineHTML(originalString, wordCount);
console.log(multiLineHTML)

const jsonData = {
    name: 'John',
                                            age: 30,
                        city: 'New York',
    great:{
        values:[1,2,3,4,      5,2,3,],mean:{'a':4,'b':5}
    }
};
console.log(pf.prettifierJson(jsonData))


console.log(pf.checkArray({'a':1,'b':2,'c':3}))

const objList = [
    { key1: 'value1', key2: 'value2' },
    { key3: 'value3', key4: 'value4' }
];

console.log(pf.mergeObjects(objList))
console.log(pf.objectLength(pf.mergeObjects(objList)))

async function main() {
    try {
        const result = await pf.fileToArray(['text.txt', 'text2.txt']);
        console.log(result);
    } catch (error) {
        console.error('Hata:', error);
    }
}

main();

var d1 = new Date();
var d2 = new Date(d1);

console.log(pf.checkDates(d1,d2),'CHECK DATES')

// usage example:
var a = ['a', 1, 'a', 2, '1'];
console.log(pf.filterUnique(a,true,false))
console.log(pf.filterUnique(a,false,false))
console.log(pf.filterUnique(a,true,true))
console.log(pf.filterUnique(a,false,true))


console.log(pf.multipleConditions([1,2,3,4,5],[1,2,3,4,5]),'MULTIPLE CONDITIONS')

console.log(pf.numberWithCommas(10000000000),'NUMBER WITH COMMAS')



console.log(pf.isNumeric(100.23123),'IS NUMERIC?')
console.log(pf.isNumeric('1000.1239239'),'IS NUMERIC?')
console.log(pf.isNumeric('10230.sasdasd'),'IS NUMERIC?')


console.log(pf.randomRange(20,30),'RANDOM RANGE')
console.log(pf.randomRange(20,30,3),'RANDOM RANGE')
console.log(pf.randomRange(20,30,5),'RANDOM RANGE')

console.log(pf.isNumeric(100.23123,true),'IS NUMERIC?')
console.log(pf.isNumeric('1000.1239239',true),'IS NUMERIC?')
console.log(pf.isNumeric('10230.sasdasd',true),'IS NUMERIC?')

console.log(pf.getNumbers(2,10,3),'GET NUMBERS')
console.log(pf.getNumbers(10,1,-3),'GET NUMBERS')

var d1 = new Date();
console.log(pf.isValidDate(d1),'VAL DATE')
console.log(pf.isValidDate('10.1.2020'),'VAL DATE')
console.log(pf.isValidDate('10-20-300'),'VAL DATE')


console.log(pf.shuffleArrayRandom([1,2,4,123,4,5,2,100]),'SHUFFLE ARRAY')

console.log(pf.createObjectFromLists([1,2,3,4,5,6],[1,2,3]),'OBJECT FROM LISTS')
console.log(pf.createObjectFromLists([1,2],[1,2,3]),'OBJECT FROM LISTS')

let objValue = {'a':1,'b':2,'c':3}
console.log(pf.alterObjectValues(objValue,'sum',4),'ALTER OBJECT VALUES')
console.log(pf.alterObjectValues(objValue,'multiply',4),'ALTER OBJECT VALUES')
console.log(pf.alterObjectValues(objValue,'divide',4),'ALTER OBJECT VALUES')
console.log(pf.alterObjectValues(objValue,'substract',4),'ALTER OBJECT VALUES')

let array = [1,2,3,4,5,6,7,8,9,10]
console.log(pf.listReducer(array,'sum'),'listReducer VALUES')
console.log(pf.listReducer(array,'multiply'),'listReducer VALUES')
console.log(pf.listReducer(array,'divide'),'listReducer VALUES')
console.log(pf.listReducer(array,'substract'),'listReducer VALUES')

const lol = () => {
    console.log('ha')
}

console.log(pf.getType('a'))
console.log(pf.getType(123))
console.log(pf.getType(lol))
console.log(pf.getType(array))


const originalArray = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const randomItems = pf.getRandomItemsFromArray(originalArray, 3);
console.log(randomItems);


var hello = "Hello World";
console.log(pf.replaceAt(hello,2,'!!'))


console.log(pf.swapArrayElements(originalArray,2,4),'SWAP ELEMENTS')
console.log(pf.swapArrayElements(originalArray,0,9),'SWAP ELEMENTS')

console.log(pf.compareLists([1,2,3,4],[1,2,3]))


console.log(pf.findMaxMin([12,3,4,123,4,5234,3,44],'max',1),'RETURN MAX MIN')
console.log(pf.findMaxMin([12,3,4,123,4,5234,3,44],'min',1),'RETURN MAX MIN')
console.log(pf.findMaxMin([12,3,4,123,4,5234,3,44],'max',3),'RETURN MAX MIN')
console.log(pf.findMaxMin([12,3,4,123,4,5234,3,44],'min',3),'RETURN MAX MIN')

const duplicateKeyObj = [
    { id: 1, name: 'Alice' },
    { id: 2, name: 'Bob' },
    { id: 3, name: 'Alice' },
    { id: 4, name: 'Charlie' },
    { id: 4, name: 'David' },
    { id: 3, name: 'Jeff' },
    {id:5,name:'Charles'},
    {id:6,name:'Charlie'}

];

console.log(pf.removeDuplicatesByKey(duplicateKeyObj,'name'),'DUPLICATE KEY')
console.log(pf.removeDuplicatesByKey(duplicateKeyObj,'id'),'DUPLICATE KEY')


// Example equation: a^2 + b^2 == c^2
function pythagoreanEquation(a, b, c) {
    return a * a + b * b === c * c;
}

function anotherEquation(a,b,c,d,e,f){
    return a+b*2+(c+d)*e+(a*b) === f*2
}

const conditionFunction = pythagoreanEquation; // Replace with your condition function
const inputArgs = [3, 4, 5, 6, 8, 10]; // Replace with your input values array
const numVariables = 3; // Replace with the desired number of variables (3 or 4)

const result = pf.findMatchingCombinations(conditionFunction, inputArgs, numVariables);
console.log(`Matching ${numVariables}-variable combinations:`, result);

const cond2 = anotherEquation; // Replace with your condition function
const args = pf.getNumbers(1,20); // Replace with your input values array
const varNums = 5; // Replace with the desired number of variables (3 or 4)

const result2 = pf.findMatchingCombinations(cond2, args, varNums);
console.log(`Matching ${varNums}-variable combinations:`, result2);

const operation = "divide"; // Change this to "sum", "multiply", "factorial", "fibonacci", "subtract", "divide", etc.
const numbers = [10, 2, 2]; // Provide numbers as an array

const recursiveResult = pf.recursiveMathOperation(operation, ...numbers);
console.log(`Result of ${operation}(${numbers.join(", ")}): ${recursiveResult}`);

const nums = [1, 3, 4, 2, 2,3,1,10,10,123,32,72]; // Replace with your input array
const duplicate = pf.findDuplicate(nums);
console.log("Duplicate element:", duplicate);


const dublicateNums = [4, 3, 2, 7, 8, 2, 1, 4]; // Replace with your input array
const duplicateElements = pf.findDuplicateElements(dublicateNums);
console.log("Duplicate elements:", duplicateElements);

const testCases = ["racecar", "Hello", 12321, "A man, a plan, a canal, Panama!"]; // Add more test cases as needed

for (const testCase of testCases) {
    const result = pf.isPalindrome(testCase);
    console.log(`"${testCase}" is a palindrome: ${result}`);
}


const inputArray = pf.shuffleArrayRandom(pf.getNumbers(1,10000)); // Replace with your array of a million integers
const chunkSize = 1000; // Adjust the chunk size as needed

const sortedArray = pf.externalMergeSort(inputArray, chunkSize);
console.log(sortedArray);


const inputList = [9, 4, 6, 2, 7, 4, 3, 9, 1, 15, 10, 12, 8, 17, 14, 13, 9, 1]; // Replace with user's input list
const pivots = [4, 10]; // Add pivot values

const nPartResult = pf.nPartitions(inputList, pivots);
console.log(nPartResult);

const k = 60; // Replace with the desired value of k
const regularNumbers = pf.generateRegularNumbers(k);
console.log("First", k, "regular numbers:", regularNumbers)

const stockPrices = pf.shuffleArrayRandom(pf.getNumbers(1,1000))
const stockResult = pf.maxProfit(stockPrices);
console.log("Maximum profit:", stockResult); // Output: 5

const detialedPrices = pf.shuffleArrayRandom(pf.getNumbers(1,10000))
const detailedResult = pf.maxProfitDetails(detialedPrices);

const summary = pf.summarizeDecisions(detailedResult);
console.log(summary)

const stringArray = ["apple", "banana", "cherry", "date", "elderberry", "fig"];
const searchTerm = "an";
const mode = "includes";

try {
    const filteredStrings = pf.filterStringsByTerm(stringArray, searchTerm, mode);
    console.log("Filtered strings:", filteredStrings);
} catch (error) {
    console.error("Error:", error.message);
}


```
</pre>

# Examples 2

<pre>
```
// Example usage
var desiredLength = 20;
var piValue = pf.calculatePi(desiredLength);
console.log(piValue);


// Example usage for an octagon (8-gon) with width 10
var shapeIdentifier = 8;
var width = 10;
var area = pf.calculateArea(shapeIdentifier, width);
console.log("Area:", area);


// Example usage for length = 10
var length = 30;
var eulerValue = pf.calculateEulerNum(length);
console.log("Euler's number with", length, "decimal places:", eulerValue);


var side1 = 5;
var side2 = 7;
var angleInDegrees = 45;
var triangleArea = pf.calculateTriFieldAngle(side1, side2, angleInDegrees);
console.log("Triangle Area:", triangleArea);

let num = 123.2301492300000
console.log(pf.removeZeros(num))

let logNum = 123
console.log(pf.logBase(123,2))

// Example usage with target color [255, 0, 0] (red)
const targetColor = [255, 0, 0];
const cssFilter = pf.getRecolorFilter(targetColor);
console.log("CSS Filter:", cssFilter);

const numRound = 1234923
console.log(pf.roundX(numRound,3))
console.log(pf.roundX(numRound,5))
console.log(pf.roundX(numRound,7))

console.log(pf.customPad(pf.randomRange(1,100),10))
console.log(pf.customPad(pf.randomRange(1,100),3))
console.log(pf.customPad(pf.randomRange(1,100),14))
console.log(pf.customPad((pf.randomRange(1,100),20)))

console.log(pf.toDegrees(pf.randomRange(1,100)))
console.log(pf.toRadians(pf.randomRange(1,100)))

var number1 = 4.954848;
var number2 = 5.9797;

console.log(pf.makePercentage(number1,number2))

console.log( "1+2+3", '=' , pf.parseFormula("1+2+3"));
console.log( "1 + 2 * 3", '=' , pf.parseFormula("1 + 2 * 3"));

// Example usage with an array
const inputArray = [10, 5, 2, 8, 15];
const lowerThreshold = 4;
const upperThreshold = 12;

const modifiedArray = pf.modifyValues(inputArray, lowerThreshold, upperThreshold);
console.log("Modified Array:", modifiedArray);

// Example usage with an object
const inputObject = { a: 10, b: 5, c: 2, d: 8, e: 15 };
const modifiedObject = pf.modifyValues(inputObject, lowerThreshold, upperThreshold);
console.log("Modified Object:", modifiedObject);

// Example usage
const digitNumber = 12345;
const digits = pf.getIndividualDigits(digitNumber);
console.log("Individual Digits:", digits);

// Example usage
const values = ['2.3', '2.4', '3.1'];
const decimalPlaces = 2;

const result = pf.sumAndFixDecimal(values, decimalPlaces);
console.log("Sum with fixed decimal places:", result);

// Example usage
const numberList = [12, 18, 24];
const gcdResult = pf.gcd(numberList);
console.log("GCD of the list:", gcdResult);

// Example usage
const circleRadius = 5;
const numberOfPoints = 10;
const randomPoints = pf.genRandPointCircle(circleRadius, numberOfPoints);
console.log("Random Points within Circle:", randomPoints);


console.log(pf.getDateOfWeek(3,2023))

const colorList = ["#FF0000", "rgba(0, 0, 255, 0.5)", "#00FF00"]; // Red, semi-transparent blue, green
const midpointColor = pf.getMixColor(colorList);
console.log("Midpoint Color:", midpointColor);

// Example usage
const datasets = [
    [0, 4, 5, 3, 2, 5, 6],
    [33, 26, 54, 23, 86, 23],
    [98, 253, 87, 876, 263]
];

for (const dataset of datasets) {
    const maxValue = Math.max(...dataset);
    const yScaleMax = pf.calculateYScaleMax(maxValue);
    console.log("Max Value:", maxValue, "Y-Scale Max:", yScaleMax);
}


// Example usage
const rectangleCount = 5;
const maxCanvasWidth = 500;
const maxCanvasHeight = 500;

const rectangles = pf.genNonOverLapRect(rectangleCount, maxCanvasWidth, maxCanvasHeight);
console.log("Generated Rectangles:", rectangles,rectangles.length);

// Example usage
const numberToDivide = 20;
const numberOfParts = 4;

const dividedParts = pf.divEqParts(numberToDivide, numberOfParts);
console.log("Divided Parts:", dividedParts);

// Example usage
const numberToDivide2 = 123123;
const numberOfParts2 = 23;

const dividedParts2 = pf.divEqParts(numberToDivide2, numberOfParts2);
console.log("Divided Parts:", dividedParts2);


// Example usage
const originalList = [2, 5, 10, 7, 3];
const minRange = 0;
const maxRange = 1;
const normalizedValues = pf.normalizeList(originalList, minRange, maxRange);
console.log("Normalized Values:", normalizedValues);

// Example usage
const numberNdividorsList = [6, 8, 9, 12, 16, 18, 25, 36,123,100,14,15];
const N = 4;

const matchingNumbers = pf.findNDividers(numberNdividorsList, N);
console.log("Numbers with", N, "divisors:", matchingNumbers);


// Example usage
const originalValue = 2048; // 2048 bits
let startUnit = 'bit'
let unitConvert = 'kilobyte'
const convertedValue = pf.convertMemory(originalValue, startUnit, unitConvert);
console.log(convertedValue + ' ' + unitConvert);

const originalValue2 = 1000; // 2048 bits
let startUnit2 = 'byte'
let unitConvert2 = 'gigabyte'
const convertedValue2 = pf.convertMemory(originalValue, startUnit2, unitConvert2);
console.log(convertedValue2 + ' ' + unitConvert2);

// Example usage
const numberArray = [12, 18, 24];
const lcm = pf.findLCMOfArray(numberArray);
console.log("LCM of", numberArray, "is", lcm);

```
</pre>


* You can check the code from github
* code is made to simplfy the steps on javascript
* I will update the code and function when I find new problems
* Project is open source


