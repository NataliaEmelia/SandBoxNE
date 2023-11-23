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
