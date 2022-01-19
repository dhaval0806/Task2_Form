# Task2_Form

<html>
    <body>
<form action="task3.html" method="post">
    <table>
        <tr>
            <td>
                <label for="uname"> User Name </label>
            </td>
            <td>
                <input type="text" id="uname" name="User name">
            </td>
        </tr>
        <tr>
            <td>
                <label> Address</label>
            </td>
            <td>
                <textarea rows="5" cols="40"></textarea>
            </td>
        </tr>
        <tr>
            <td>
                <label for="vid">Video</label>
            </td>
            <td>
                <input type="file" id="vid" onchange="playvideo()">
            </td>
        </tr>
        <tr>
            <td></td>
            <td>
                <input type="submit" value="Submit">
                <input type="reset">
                
                
                
                
                
                
                
                
                
                
                
                
                
                
                <!DOCTYPE html>
<html>
<head>
<title></title>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<script type="text/javascript">
var citiesByState = {
Gujarat: ["Ahmedabad","Surat","Rajkot","Anand","vadodara"],
Rajasthan: ["Jaipur","Udaipur"]
}
function makeSubmenu(value) {
if(value.length==0) document.getElementById("citySelect").innerHTML = "<option></option>";
else {
var citiesOptions = "";
for(cityId in citiesByState[value]) {
citiesOptions+="<option>"+citiesByState[value][cityId]+"</option>";
}
document.getElementById("citySelect").innerHTML = citiesOptions;
}
}
function displaySelected() { var country = document.getElementById("countrySelect").value;
var city = document.getElementById("citySelect").value;
alert(country+"\n"+city);
}
function resetSelection() {
document.getElementById("countrySelect").selectedIndex = 0;
document.getElementById("citySelect").selectedIndex = 0;
}
</script>
</head>
<body onload="resetSelection()">
<h1>Javascript Form</h1>
<label>Name:</label>
<input type="text" name="name"/><br><br>
<label>Address:</label>
<textarea type="text" name="name"></textarea><br><br>
<label>Mobile number:</label>
<input type="text" mobile number="mobile"><br><br>
<label>Gender:</label>
<input type="radio" name="gender">Male
<input type="radio" name="gender"/>Female<br><br>
<br><br>
<select id="countrySelect" size="1" onchange="makeSubmenu(this.value)">
<option value="" disabled selected>Choose State</option>
<option>Gujarat</option>
<option>Rajasthan</option>
</select>
<select id="citySelect" size="1" >
<option value="" disabled selected>Choose City</option>
<option></option>
</select>
<button onclick="displaySelected()">show selected</button><br><br>
<input type="submit" name="submit" />
</body>
</html>
            </td>
        </tr>
        
        <a href="" id="path">video</a>
           
        </tr>
    </table>
</form>
<script>
    function playvideo(){
       var path = document.getElementById("vid");
$('#path').attr('href',path);
    }
</script>
</body>
</html>
