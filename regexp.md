<html>
<head>
<title>Form validation</title>
<script src="valid.js">
</script>
</head>

<body>
<br>

<h2>Application for Passport</h2>

<br>

<form name="myForm" onsubmit="return formvalidate()">

<h3 align="40px">First Name *</h3>

<input type="text" id="fName" placeholder="Enter your first name" />

<h3 align="40px">Father's Name *</h3>

<input type="text" id="mName" placeholder="Enter your fathers name" />

<h3 align="40px">Last Name *</h3>

<input type="text" id="lName" placeholder="Enter your last name" />
<br><br>
<tr>
 <td rowspan="6"> Address * </td>
 <td><textarea id="address" cols="60" rows="6"></textarea></td>
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


