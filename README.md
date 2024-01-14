# calculator-html-css-
<!DOCTYPE html>
<html>
<head>
    <script src="a1.js"></script>
    <title> My calculator</title>
    <style>
        .clear{
            background-color: yellow;
        }
        .operator{
            background-color: greenyellow;
        }
        .variable{
            background-color: cyan;
        }
        table{
            border: 1px solid black;
            margin-left: auto;
            margin-right: auto;
        }

        input[type="button"]{
            width: 100%;
            padding: 20px 40px;
            color: brown;
            font-size: 30px;
            font-weight: bold;
            border: none;
            border-radius: 7px;
        }
        input[type="text"]{
            padding: 30px 40px;
            font-size: 28px;
            font-weight: black;
            border: none;
            border-radius: 7px;
            border: 4px solid black;
        }
    </style>
</head>
<body>
<table id="calculator1"> 
        <tr> 
            <td colspan="3"><input type="text" id="result" ></td>
            <td><input type="button" value="reset" onclick="clr()" class="clear"></td> 
        </tr> 
    
        <tr> 
            <td><input type="button" value="(" onclick="display('(')" onkeydown="myFunction(event)"class="operator"></td> 
            <td><input type="button" value=")" onclick="display(')')" onkeydown="myFunction(event)" class="operator"></td> 
            <td><input type="button" value="." onclick="display('.')" onkeydown="myFunction(event)" class="operator"></td> 
            <td><input type="button" value="%" onclick="display('%')" onkeydown="myFunction(event)" class="operator"></td> 
        </tr>
        <tr> 
            <td><input type="button" value="7" onclick="display('7')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="8" onclick="display('8')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="9" onclick="display('9')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="/" onclick="display('/')" onkeydown="myFunction(event)" class="operator"></td> 
        </tr> 
        <tr> 
            <td><input type="button" value="4" onclick="display('4')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="5" onclick="display('5')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="6" onclick="display('6')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="*" onclick="display('*')" onkeydown="myFunction(event)" class="operator"></td> 
        </tr> 
        <tr> 
            <td><input type="button" value="1" onclick="display('1')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="2" onclick="display('2')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="3" onclick="display('3')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="-" onclick="display('-')" onkeydown="myFunction(event)" class="operator"></td> 
        </tr> 
        <tr> 
            <td><input type="button" value="PI" onclick="display('3.1415')" onkeydown="myFunction(event)" class="variable"></td>
            <td><input type="button" value="0" onclick="display('0')" onkeydown="myFunction(event)" class="variable"></td> 
            <td><input type="button" value="=" onclick="solve()" class="operator"></td> 
            <td><input type="button" value="+" onclick="display('+')" onkeydown="myFunction(event)" class="operator"></td> 
        </tr> 
    </table> 
</body> 
  
</html> 
