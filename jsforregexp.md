
function formvalidate()
{
var firstname = document.getElementById("fname");
var middlename = document.getElementById("mname");
var lastname = document.getElementById("lname");
var address = document.getElementById("address");
var mob = document.getElementById("Mobile");

if (finputAlphabet(firstname, "* For your name please use alphabets only *")) {
if (minputAlphabet(middlename, "* For your name please use alphabets only *")) {
if (linputAlphabet(lastname, "* For your name please use alphabets only *")) {	
if (textAlphanumeric(address, "* For Address please use numbers and letters *")) {
if (textNumeric(mob, " Please enter a valid mobile number")) {
return true;
}
}
}
return false;
}
function textNumeric(inputtext, alertMsg) {
var numericExpression = /^[0-9]+$/;
if (inputtext.value.match(numericExpression)) {
return true;
} else {
document.getElementById("Mobile").innerText = alertMsg; 
inputtext.focus();
return false;
}
}
function finputAlphabet(inputtext, alertMsg) {
var alphaExp = /^[a-zA-Z]+$/;
if (inputtext.value.match(alphaExp)) {
return true;
} else {
document.getElementById("fName").innerText = alertMsg; 
//alert
inputtext.focus();
return false;
}
}
function minputAlphabet(inputtext, alertMsg) {
var alphaExp = /^[a-zA-Z]+$/;
if (inputtext.value.match(alphaExp)) {
return true;
} else {
document.getElementById("mName").innerText = alertMsg; 
//alert
inputtext.focus();
return false;
}
}
function linputAlphabet(inputtext, alertMsg) {
var alphaExp = /^[a-zA-Z]+$/;
if (inputtext.value.match(alphaExp)) {
return true;
} else {
document.getElementById("lName").innerText = alertMsg; 
//alert
inputtext.focus();
return false;
}
}
function textAlphanumeric(inputtext, alertMsg) {
var alphaExp = /^[0-9a-zA-Z]+$/;
if (inputtext.value.match(alphaExp)) {
return true;
} 
else {
document.getElementById("address").innerText = alertMsg; 
inputtext.focus();
return false;
}
}

}
