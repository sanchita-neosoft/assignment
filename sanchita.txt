<!Doctype html>
<html>
<head>
			<link rel="stylesheet" type="text/css" href="style.css">
			<script src="script.js"></script>
			<script>
				$(document).ready(function {
					$("form").submit(function(event) {
                     event.preventDefault();
                     var name=$("#mail-name").val();
                     $(".form-message").load("mail.php",{
                     name=name,
                     });
					});
					
				});
			</script>

	<title>Passport Registration form!!!!</title>
		<body>
	<form action="validation.php">
				<h1>Service Required</h1>
				
				Applying for:<select name="applyingfor">
					 <option value="freshpassport/newpassport">Fresh passport/New passport</option>
         <option value="reissuepassport">Reissuepassport</option>
         <select><br><br>
         	Type of Application: <select name="typeofapplication">
					 <option value="normal">Normal</option>
         <option value="tatkaal">Tatkaal</option>
         <select>&nbsp;&nbsp;&nbsp;
         	Type of Passbook Booklet: <select name="typeofpassbookbooklet">
					 <option value="36pages">36 Pages</option>
         <option value="60pages">60 Pages</option>
         <select>&nbsp;&nbsp;&nbsp;
            Validity Required: <select name="validityreqired">
					 <option value="10years">10 years</option>
           <option value="uptoage18">Upto age 18</option>
         <select><br><br>

         	<h2>Applicant Details</h2>
         	Applicant's Given name: <input type="text" name="applicantgivenname" required>&nbsp;&nbsp;&nbsp;
				Surname:<input type="text" name="surname" required><br><br>
				Are you known by any other names (aliases)?: <select name="aliases">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select>&nbsp;&nbsp;&nbsp;
         	Have you ever changed your name?: <select name="changename">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select>&nbsp;&nbsp;&nbsp;
         	Date of Birth (dd-mm-yyyy): <input type="date" name="date"><br><br>
			Place of Birth: <input type="text" name="placeofbirth">&nbsp;&nbsp;&nbsp;
				District: <input type="text" name="district">&nbsp;&nbsp;&nbsp;
				State: <input type="text" name="state">&nbsp;&nbsp;&nbsp;
				Country: <input type="text" name="country"><br><br>
				<input type="radio" name="gender" value="male" checked> Male  <input type="radio" name="gender" value="female"> Female  
				 <input type="radio" name="gender" value="other"> Other &nbsp;&nbsp;&nbsp;
                   Marital status: <select name="marital">
					 <option value="married">Married</option>
         <option value="unmarried">Single</option>
         <select>&nbsp;&nbsp;&nbsp;
               Nationality: <select name="nationality">
					 <option value="indian">Indian</option>
         <option value="other">Other</option>
         <select><br><br>    
             Pan: <input type="text" name="pan" required>&nbsp;&nbsp;&nbsp;
             Aadhar: <input type="text" name="aadhar" required>&nbsp;&nbsp;&nbsp;
              Employment Type: <select name="Employment">&nbsp;&nbsp;&nbsp;
					 <option value="PSU">PSU</option>
					 <option value="Government">Government</option>
					 <option value="Statutory Body">Statutory Body</option>
					 <option value="Retired Government Servant">Retired Government Servant</option>
					 <option value="Self Employed">Self Employed</option>
					 <option value="Self Employed">Self Employed</option>
					 <option value="Homemaker">Homemaker</option>
					 <option value="Not Employed">Not Employed</option>
					 <option value="Retired-Private Service">Retired-Private Service</option>
					 <option value="Student">Student</option>
					 <option value="Others">Others</option>
					 <option value="Owners, Partners &amp; Directors of companies which are members of CII, FICCI &amp; ASSOCHAM">Owners, Partners &amp; Directors of companies which are members of CII, FICCI &amp; ASSOCHAM</option>
					 
					 
         <select><br><br>
         	 Educational Qualification: <select name="qualification">
					<option value="10th pass and above">10th pass and above</option>
         <option value="Graduate and above">Graduate and above</option>
         <select><br><br> 

         <h2>Family Details</h2>
         	Father Given name: <input type="text" name="father">&nbsp;&nbsp;&nbsp;
				      Surname:<input type="text" name="surname"><br><br> 
		
         	Mother Given name: <input type="text" name="mother">&nbsp;&nbsp;&nbsp;
				      Surname:<input type="text" name="surname"><br><br>
				
            Spouse Given name: <input type="text" name="spouse">&nbsp;&nbsp;&nbsp;
				      Surname:<input type="text" name="surname"><br><br> 
       		
          Guardian Given name: <input type="text" name="guardian">&nbsp;&nbsp;&nbsp;
				      Surname:<input type="text" name="surname"><br><br> 
      <label> If applicant is minor, provide following details</label><br><br>
    <label>  Parent Passport Details (If passport has been applied for but not received, give File Number)</label><br><br>

     Father/ Legal Guardian File/ Passport Number: <input type="text" name="father">&nbsp;&nbsp;&nbsp; 
Father/ Legal Guardian Nationality, if not Indian: <input type="text" name="father"><br><br> 
	 Mother/ Legal Guardian File/ Passport Number: <input type="text" name="father">&nbsp;&nbsp;&nbsp;
	
Father/ Legal Guardian Nationality, if not Indian: <input type="text" name="father"><br><br> 
		
         	<h4> Present Residential Address Details</h4>
         	Residing Since (MM-YYYY): <input type="text" name="name">&nbsp;&nbsp;&nbsp; 
           House No. and Street Name: <input type="text" name="name" required><br><br> 
             Village or Town or City: <input type="text" name="name" required>&nbsp;&nbsp;&nbsp; 
                            District: <input type="text" name="name" required><br><br> 
         	          Police Station: <input type="text" name="name">&nbsp;&nbsp;&nbsp;
         	               State/ UT: <input type="text" name="name" required><br><br> 
                                 PIN: <input type="text" name="name" required>&nbsp;&nbsp;&nbsp;
         	           Mobile Number: <input type="text" name="mobileno" required><br><br> 
         	        Telephone Number: <input type="text" name="telephoneno">&nbsp;&nbsp;&nbsp;
                           E-mail ID: <input type="email" name="email" required><br><br> 
         Is permanent address same as present address?: <select name="address">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br>

  <h2> Previous Passport/ Application Details</h2>
    <label> Details of latest held/ existing/ lost/ damaged Ordinary Passport/ Identity Certificate</label><br><br>
    Passport/ Identity Certificate Number: <input type="text" name="surname">&nbsp;&nbsp;&nbsp; 
               Date of Issue (DD-MM-YYYY): <input type="date" name="date"><br><br> 
              Date of Expiry (DD-MM-YYYY): <input type="date" name="date">&nbsp;&nbsp;&nbsp;
                           Place of Issue: <input type="text" name="surname"><br><br> 
Have you ever applied for passport, but not issued?: <select name="passport">
					<option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br> 

         	<h5> Other details</h5>
         	 Have you ever been charged with criminal proceedings or any arrest warrant/ summon Yes No pending before a court in India?:
         	  <select name="question">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br>
         		 Have you at any time during the period of 5 years immediately preceding the date of this application been convicted by a court in India for any criminal offence & sentenced to imprisonment for two years or more?: <select name="question">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br>
     	Have you ever been refused or denied passport?: <select name="question">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br>
         	 Has your Passport ever been Impounded or Revoked?: <select name="question">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br>
         		 Have you ever applied for/ been granted political asylum to/ by any foreign country?: <select name="question">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br>
         	Have you ever returned to India on Emergency Certificate (EC) or were ever deported or repatriated?: <select name="question">
					 <option value="yes">Yes</option>
         <option value="no">No</option>
         <select><br><br>
<input type="radio" name="chb" value="chb" checked>I have read and agree with the terms & conditions and policies of this application process
<br><br>
<input type="submit" name="submit" value="CONFIRM & PROCEED">
			</form>
		</body>
	
	</head>
</html>