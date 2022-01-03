framest.html-
<html>
<head>
<frameset rows="50%,50%">
<frame src="first.html">
<frameset cols="50%,50%">
<frame src="p1.html" scrolling="yes">
<frame src="p2.html">
</frameset>
</frameset>
</head>
</html>
info.html-
<html>
<head>

<body>
<h15>LENOVO </h15>
<p>price is 30000
</p>
</body>
</html>

info1.html-
<html>
<head>
</head>
<body>
<h20>Samsung </h20>
<p>Price is 50000 </h15>
</body>
</html>

p1.html-
<html>
<head>
</head>
<body>
<p> <u>This website is degin for shopping purpose </u> </p>
</body>
</html>

p2.html-
<html>
<head>
</head>
<body>
<a href="page1.html" target="abc"> <img src="print.gif" height=200> </a>
<a href="first.html" target="abc"> <img src="print.gif" height=50> </a>
</body>
</html>

page1.html-
<html>
<head>
<frameset cols="50%,50%">

<frame name="abc" src="page2.html">
<frame name="abb" src="page3.html">
</frameset>
</head>
</html>

page2.html-
<html>
<head>
</head>
<body>
<h5>Category list
<ul type="disk">
<li> < href="info.html" target="abb">Lenovo </li>
<li> <a href="info1.html" target="abb">Samsung </li>
</ul>
</body>
</html>

page3.html-
<html>
<body background="Sunset.jpg">
<h2 align=center>Information </h2>
</body>
</html>

first.html-
<html>
<body background="AA.jpg">
<img src="web.gif">
<h2 align=center>WWW.Shopping.com </h2>
</body>
</html>
img folder-aa.jpg






2)
<html>
<head>
<title>
Input a number
</title>

<body>

<input type="text" id="n1" value="2"/>
<input type="text" id="operator" value="+"/>
<input type="text" id="n2" value="2"/>

<input type="button" value="Check" onclick="solve()"/> 




<script>


function solve()
{

var x = document.getElementById("n1").value + document.getElementById("operator").value + document.getElementById("n2").value
var y = eval(x)


alert("Answer is: "+ y);
}

</script>
</body>


</html>










3)
<html>
<head>
<script type="text/javascript" src="validateform.js"></script>

</head>
 
<body>
<form action="#" name="StudenSignupForm" onsubmit="return(validateHTMlform());">
 
 
<p><b>Student Registration Form</b> <br>
 

First Name
<input type=text  name=textnames id="textname" size="30">
<br>
 
Last Name
<input type=text name=lastnames id="lastname" size="30">
<br>
  
 
 
 
Gender
<input type="radio" name="sex" value="male" size="10">Male
<input type="radio" name="sex" value="Female" size="10">Female
<br>
 
 

Course
<select name="Course">
<option value="-1" selected>select..</option>
<option value="B.Tech">B.TECH</option>
<option value="MCA">MCA</option>
<option value="MBA">MBA</option>
<option value="BCA">BCA</option>
</select>

 
<br>
 
 
student email
<input type="text" name="emailid" id="emailid" size="30">
<br>
 
 
Mobile Number
<input type="text" name="mobilenumber" id="mobilenumber" size="30">
<br>


<input type="reset">
<input type="submit" value="Submit Form" />


</form>
</body>
</html>




Js:

function validateHTMlform()
{
  form = document.StudenSignupForm;
   if ( form.textnames.value == "" || form. textnames.value.length > 25 )
   {
     alert( "Enter Your First Name!" );
     form.textnames.focus() ;
     return;
   }
   if( form.lastnames.value == "" )
   {
     alert ( "Enter Your Last Name!" );
     form.textnames.focus() ;
     return;
   }
  

  

   if( form.Course.value == "-1" )
   {
     alert( "Enter Your Course!" );
    
     return;
   }  

var email = form.emailid.value;
  atpos = email.indexOf("@");
  dotpos = email.lastIndexOf(".");
if (email == "" || atpos < 1 || ( dotpos - atpos < 2 ))
{
     alert("Enter your correct email ID")
     form.emailid.focus() ;
     return;
}






  if( form.mobileno.value == "" || form.mobileno.value.length != 10 || isNaN( form.mobileno.value) ||)
   {
     alert( "Enter your Mobile No. in the format 123." );
     form.mobileno.focus() ;
     return;
   }
   return( true );
}
































