# JSJunior

// DESCRIPTION
// Page 40
// change text "эЙ, кАК деЛа?" to "Эй, как дела?".

// SOLUTION
var string = "эЙ, кАк деЛа?"
string = string.toLowerCase();
string = string.slice(1);
string = "Э" + string;
