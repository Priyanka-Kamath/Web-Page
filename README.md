# Web-Page
Survey Form


//PHP

<head>


<title>xxx Priyanka Kamath xxx</title>
<style type="text/css">
.auto-style1 {

}
</style>

<meta content="revealTrans(Duration=1.0,Transition=2)" http-equiv="Page-Enter" />
<style>
    div.styleize p { font-family: "Times New Roman", Times, serif; }
</style>

<style type="text/css">
.auto-style1 {
	font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande", "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
}
.auto-style8 {
	border-style: solid;
	border-width: 1px;
	color: rgb(0, 0, 0);
	font-size: medium;
	font-style: normal;
	font-variant: normal;
	font-weight: normal;
	letter-spacing: normal;
	line-height: normal;
	text-align: start;
	text-indent: 0px;
	text-transform: none;
	white-space: normal;
	word-spacing: 0px;
	display: normal;
}
.auto-style5 
{
font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande", "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
			}
.auto-style18
{
	text-align: center;
}



.auto-style21 {
	border-width: 0px;
	font-family: Georgia, "Times New Roman", Times, serif;
}



.auto-style3 {
	font-family: Georgia, "Times New Roman", Times, serif;
}



.auto-style22 {
	border-style: solid;
	border-width: 1px;
}
.auto-style23 {
	border-style: solid;
	border-width: 1px;
	font-family: Georgia, "Times New Roman", Times, serif;
}



.auto-style6 {
	text-align: center;
}
.auto-style7 {
	font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande", "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
	color: #808080;
	font-size: x-small;
}



.auto-style24 {
	border-style: solid;
	border-width: 1px;
	font-size: small;
}



</style>
</head>

<body class="auto-style1">
<div class="styleize"'>
<?php
extract($_REQUEST);


$val ="";
if (is_array($subject)){


foreach ( $subject as $key=>$value )
{

$val = $val . "<br>" . $value;

}

}


$val1 ="";
if (is_array($grade)){


foreach($grade as $key=>$value1)
{

$val1 = $val1 ."<br>" .$value1;

}

}

?>



<table align="center" class="auto-style21" style="width: 70%; height: 234px" cellpadding="5" cellspacing="4">
	<tr>
		<td colspan="3" class="auto-style22">
		<strong>

		<div class="auto-style18">
			<strong>Student Survey Questionnarie on Need</strong><span class="auto-style5"><hr /></div>
</span></strong>
		</td>
	</tr>
	<tr>
		<td colspan="3" class="auto-style22">
		<strong>PART I</strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">
		&nbsp;</td>
		<td style="width: 320px; orphans: auto; widows: 1; -webkit-text-stroke-width: 0px; float: none;" class="auto-style8">
		What is your school?</td>
		<td class="auto-style24"><strong><?php print $school ?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">1.</td>
		<td style="width: 320px" class="auto-style22">What is yor major?</td>
		<td class="auto-style24"><strong><?php print $major?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">2.</td>
		<td style="width: 320px" class="auto-style23">
			Are you interested in teaching?</td>
		<td class="auto-style24"><strong><?php print $radio1 ?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style23">If <strong>No</strong>,</td>
		<td style="width: 320px" class="auto-style23">&nbsp;Please explain your reason(s) and explain.</td>
		<td class="auto-style24"><strong><?php print $comment ?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">If <strong>Yes</strong></strong>,</td>
		<td style="width: 320px" class="auto-style22">a. Which subject(s) would you prefer to teach?</td>
		<td class="auto-style24"><strong><?php print $val ?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22" rowspan="3">&nbsp;</td>
		<td style="width: 320px" class="auto-style22">b. What grade level(s) would you 
		prefer to teach?</td>
		<td class="auto-style24"><strong><?php print $val1 ?></strong></td>
	</tr>
	<tr>
		<td style="width: 320px" class="auto-style22">c. Are you willing to teach in a 
		high need school?</td>
		<td class="auto-style24"><strong><?php print $radio2 ?></strong></td>
	</tr>
	<tr>
		<td style="width: 320px" class="auto-style22">d. Do you need financial aid to 
		enroll in the teacher <span class="auto-style3">&nbsp;&nbsp;&nbsp; </span>preparation program?</td>
		<td class="auto-style24"><strong><?php print $radio3 ?></strong></td>
	</tr>
	<tr>
		<td colspan="3" class="auto-style22">
		<strong>PART II</strong></td>
		</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">1.</td>
		<td style="width: 320px" class="auto-style22">
			Which county do you live in?</td>
		<td class="auto-style22"><strong><?php print $country ?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">2.</td>
		<td style="width: 320px" class="auto-style22">
			What is your age?</td>
		<td class="auto-style22"><strong><?php print $age ?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">3.</td>
		<td style="width: 320px" class="auto-style22">
			What is your gender?</td>
		<td class="auto-style22"><strong><?php print $radio4 ?></strong></td>
	</tr>
	<tr>
		<td style="width: 40px" class="auto-style22">4.</td>
		<td style="width: 320px" class="auto-style22">
			What is your ethnicity?</td>
		<td class="auto-style22"><strong><?php print $radio5 ?></strong></td>
	</tr>
	<tr>
		<td class="auto-style22" colspan="3">
		<div class="auto-style6">
			<span class="auto-style7"> Web Programming</span><br class="auto-style7" />
			<span class="auto-style7">Survey 01</span><br class="auto-style7" />
			<span class="auto-style7">Priyanka Kamath</span><br class="auto-style7" />
			<span class="auto-style7">xxx<br />
			<a href="mailto:priyanka.kamath@xxx.xxx.xxx">
			priyanka.kamath@xxx.xxx.xxx</a></span></div>
			</td>
	</tr>
</table>

<?php $message = "Student Survey Questionnarie Results:\n\n1.  $school\n2.  $major\ n3.  $radio1\n4. $comment \n5. $val  \n6.  $val1 \n7. $radio2 \n8. $radio3 \n9. $country \n10. $age \n11. $radio4 \n12. $radio5 ";
    $myfile = "StudentSurveyReplyBy" . $school . $major . date("Ymdgis") . ".txt";
    $fh = fopen($myfile,'w') or die ("can't open file");

fwrite($fh,$message);

fclose($fh);

//DB Connection

//DB connection


$db="priyanka";

$link = @mysql_connect("localhost","root","");

if( !$link ) {   

die( "Couldn't connect to MySQL: ".mysql_error() ); 

}   

@mysql_select_db( $db ) or die ( "Couldn't open $db: ".mysql_error() );   

//Student Survey Questionnarie Results:\n\n1.  $school\n2.  $major\ n3.  $radio1\n4. $comment \n5. $val  \n6.  $val1 \n7. $radio2 \n8. $radio3 \n9. $country \n10. $age \n11. $radio4 \n12. $radio5   

$query = "INSERT INTO assignment VALUES('$school','$major','$radio1','$comment','$val','$val1','$radio2','$radio3','$country','$age','$radio4','$radio5')";

mysql_query($query) or die ( "INSERT error: ".mysql_error() );   

mysql_close( $link );    





    ?>


</body>

</html>
