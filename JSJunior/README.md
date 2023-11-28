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

// DESCRIPTION
// Page 69 #4.
// Соединение чисел
// Как с помощью метода join превратить массив [3, 2, 1]
// в строку "3 is greater than 2 is greater than 1"?

//SOLUTION
var masJoin = [3, 2, 1];
var masJoins = [masJoin[0], "is greater than", masJoin[1], "is greater than", masJoin[2]].join(" ");
masJoins;

// DESCRIPTION
// Page 82 #4.1
// Подсчет очков
// Представьте, что вы играете в какую-нибудь игру со своими друзьями и вам нужно
// вести счет. Создайте для этого объект и назовите его scores. Пусть ключами
// будут имена ваших друзей, а значениями — набранные ими очки (0 или больше).
// Счет игроков надо будет увеличивать по мере того, как они зарабатывают новые
// очки. Как вы будете менять счет игрока, хранящийся в объекте scores?

//SOLUTION
var scores = {};
scores["Kate"] = 0;
scores["Paul"] = 0;
scores["Marie"] = 0;
scores["Marie"] += 1;

// DESCRIPTION
// Page 82 #4.2
// Вглубь объектов и массивов
// Пускай у вас есть такой объект:
// var myCrazyObject = {
// "name": "Нелепый объект",
// "some array": [7, 9, { purpose: "путаница", number: 123 }, 3.3],
// "random animal": "Банановая акула"
// };
// Как одной строкой JavaScript-кода извлечь из этого объекта число 123?

//SOLUTION
var myCrazyObject = {
"name": "Нелепый объект",
"some array": [7, 9, { purpose: "путаница", number: 123 }, 3.3],
"random animal": "Банановая акула"
};
myCrazyObject["some array"][2].number;

/ DESCRIPTION
// Page 101 #6
// Напишите программу с переменной name. Если в этой переменной находится
// ваше имя, напечатайте: «Привет мне!» — иначе напечатайте: «Привет,
// незнакомец!» (Подсказка: используйте === для сравнения переменной name
// с вашим именем.)
// Теперь дополните программу, чтобы она здоровалась с вашим папой,
// если в name его имя, и с вашей мамой, если в name ее имя. Если же там
// что-то иное, по-прежнему печатайте «Привет, незнакомец!».

//SOLUTION
var name;
if (name === "Natalia") {
console.log("Hi to me");
} else if (name === "Evgeniy"){
console.log("Hi cat");
} else if (name === "Maria"){
console.log("Hi kitty");
} else {
console.log("Hi stranger");
}
name = "Maria";
