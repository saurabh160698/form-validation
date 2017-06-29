# form-validation
form validation without using regular expressions.
<html>
<head>
<title>Form validation</title>
</head>
<body>
<script>

function validate()

{

 var x=document.getElementById("fName").value;

 var m=document.getElementById("mName").value;

 var l=document.getElementById("lName").value;

 var y=document.getElementById("Mobile").value;

 var z=document.getElementById("email").value;  

 var w=document.getElementById("ans").value;  

var b=document.myForm.address.value;

if (x =="" || y =="" || z =="" || w =="" || m =="" || l =="" || b =="") 

  {

        alert("Please fill the (*) areas. ");

        return false;

  }

  if( isNaN(y) || y.length != 10 )
{
  alert("Not a valid phone number");
  return false;
}
if ( myForm.MyCheckbox1.checked == false && myForm.MyCheckbox2.checked == false && myForm.MyCheckbox3.checked == false && myForm.MyCheckbox4.checked == false) 
    {
        alert ("You need to choose any of the checkboxes!");
        return false;

}
if(b.length < 15 || b.length > 100)
{
  alert("Please enter the address correctly");
  return false;
}

}
</script>

<br>

<h2>Application for Passport</h2>

<br>

<form name="myForm" onsubmit="return validate()">

<h3 align="40px">First Name *</h3>

<input type="text" id="fName" placeholder="Enter your first name" />

<h3 align="40px">Father's Name *</h3>

<input type="text" id="mName" placeholder="Enter your fathers name" />

<h3 align="40px">Last Name *</h3>

<input type="text" id="lName" placeholder="Enter your last name" />
<br><br>
<tr>
 <td rowspan="6"> Address * </td>
 <td><textarea name="address" cols="60" rows="6"></textarea></td>
 </tr>
 <tr>
 <td></td>

<h3 align="40px">Mobile number *</h3>

<input type="text" id="Mobile" placeholder="Enter your number" />

<h3 align="40px">Email-ID *</h3>

<input type="email" id="email"  placeholder="Enter your email" />

<h3 align="40px">Gender</h3>

<input type="radio" name="gender" value="male" checked>Male

<br>

<input type="radio" name="gender" value="female">Female

<br>

<h3 align="40px">What documents do you have?</h3>

<input type="checkbox" name="MyCheckbox1" value="ration">Ration Card<br>

<input type="checkbox" name="MyCheckbox2" value="aadhar">Aadhar Card<br> 

<input type="checkbox" name="MyCheckbox3" value="pan">Pan Card<br>

<input type="checkbox" name="MyCheckbox4" value="driver">Driving License<br>

<h3>Security Question? *</h3>

<select>

  <option value="village">Where is your village?</option>

  <option value="Pet">What is your pet name?</option>

  <option value="birth">Where is your birth place?</option>	

</select>

<br><br>

<input type="text" id="ans" placeholder="Enter your answer" />

<br><br>

<textarea rows="5" cols="150">

Please note that this is an official site of Government of India.Therfore,please provide valid informations only.

</textarea>

<br><br>

<center>

<input type="submit" value="Submit" /></center>

</form>

</body>

</html> 
