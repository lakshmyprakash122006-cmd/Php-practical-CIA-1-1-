# Php-practical-CIA-1-1-
Program 
<html>
<head>
<style>
body {
    font-family: Arial;
}
form {
    width: 300px;
    padding: 20px;
    border: 1px solid black;
}
</style>
</head>

<body>

<h2>Student Grade</h2>

<form method="post">

Enter Marks:
<input type="number" name="marks"><br><br>

<input type="submit" name="submit" value="Find Grade">

</form>

<?php

if(isset($_POST['submit']))
{
    $marks = $_POST['marks'];

    if($marks >= 90)
    {
        echo "Grade: A";
    }
    elseif($marks >= 80)
    {
        echo "Grade: B";
    }
    elseif($marks >= 70)
    {
        echo "Grade: C";
    }
    elseif($marks >= 60)
    {
        echo "Grade: D";
    }
    else
    {
        echo "Grade: F";
    }
}

?>

</body>
</html>

Output: Grade: B
