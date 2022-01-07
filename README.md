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
