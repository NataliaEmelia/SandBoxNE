# JSJunior

// DESCRIPTION
// Page 40
// change text "эЙ, кАК деЛа?" to "Эй, как дела?".

// SOLUTION
var string = "эЙ, кАк деЛа?"
string = string.toLowerCase();
string = string.slice(1);
string = "Э" + string;

// DESCRIPTION
// Page 47
// var age = 11;
// var accompanied = true;
// ???
// Допишите этот код, чтобы он определял, можно ли 11-летнему посетителю
// посмотреть фильм (возраст задается в переменной age, а переменная
// accompanied равна true, если посетитель пришел со взрослым).
// Попробуйте поменять эти значения (например, пусть в age будет число 12,
// а в accompanied — true) и убедитесь, что код по-прежнему находит
// верное решение.

// SOLUTION
var age = 12;
var accompanied = true;
var ageMoved = age >= 12 || accompanied;

// DESCRIPTION
// Page 69
// У нас есть три массива со словами, и в строках ,  и  мы с помощью трех индексов берем
// из каждого массива по случайному слову. Затем мы склеиваем их, помещая результат
// в переменную randomInsult, — это и есть готовая дразнилка. В строках  и  мы используем
// множитель 3, поскольку и в randomAdjective, и в randomBodyPart по три элемента.
// Аналогично в строке  мы умножаем на 5, ведь в randomWords пять элементов.
// Обратите внимание, что мы добавили между randomAdjective и randomWord

//SOLUTION
var randomColor = ["red", "green", "gray", "blue", "black"]
var randomPart = ["face", "leg", "hair", "hand"]
var randomState = ["sticky", "nasty", "slimy", "smelly"]

var randomColors = randomColor[Math.floor(Math.random() * randomColor.length)];
var randomParts = randomPart[Math.floor(Math.random() * randomPart.length)];
var randomStates = randomState[Math.floor(Math.random() * randomState.length)];

var randomInsult = "Your " + randomParts + "like " + randomColors + " " + randomStates + " " + randomParts + "!";
randomInsult;

var randomInsultJoin = ["At your place", randomParts, "like", randomStates, randomParts + "!!!"].join(" ");
randomInsult;
