# Calculator
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="background">
        <div class="calculator">
            <form>
                <div class="screen">
                    <input type="text" name="screen">
                </div>
                <div>
                    <input type="button" value="C" onclick="screen.value= ''">
                    <input type="button" value="del" onclick="screen.value=screen.value.toString().slice(0,-1)">
                    <input type="button" value="." onclick="screen.value+= '.'">
                    <input type="button" value="/" class="operation" onclick="screen.value+= '/'">
                </div>
                <div>
                    <input type="button" value="7" onclick="screen.value+= '7'">
                    <input type="button" value="8" onclick="screen.value+= '8'">
                    <input type="button" value="9" onclick="screen.value+= '9'">
                    <input type="button" value="+" class="operation" onclick="screen.value+= '+'">
                </div>
                <div>
                    <input type="button" value="6" onclick="screen.value+= '6'">
                    <input type="button" value="5" onclick="screen.value+= '5'">
                    <input type="button" value="4" onclick="screen.value+= '4'">
                    <input type="button" value="-" class="operation" onclick="screen.value+= '-'">
                </div>
                <div>
                    <input type="button" value="3" onclick="screen.value+= '3'">
                    <input type="button" value="2" onclick="screen.value+= '2'">
                    <input type="button" value="1" onclick="screen.value+= '1'">
                    <input type="button" value="*" class="operation" onclick="screen.value+= '*'">
                </div>
                <div>
                    <input type="button" value="0" onclick="screen.value+= '0'">
                    <input type="button" value="=" class="equalto" onclick="screen.value=eval(screen.value)">
                    <span class="name">@amanramola</span>
                </div>
            </form>
        </div>
    </div>
</body>
</html>

*{
    padding:0;
    margin:0;
    box-sizing: border-box;
}
.background{
    background:rgb(255,197,20);
    background: linear-gradient(90deg,rgb(255, 191, 0)0%, rgb(255, 57, 18)100%);
    width:100%;
    height:100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}
.calculator{
    background-color:rgba(0, 0, 0, 0.962);
    padding:15px;
    border-radius:10px;
}
.calculator input{
    border:0px;
    margin:1px;
    width:50px;
    height:50px;
    border:1px solid rgb(0, 0, 0);
    cursor:pointer;
    font-size: 1.5rem;
} 
.operation{
    background-color: #e06d06;
    color:white;
}  
.equalto{
    background-color: #f77f00;
    color:white;
}
.screen{
    display: flex;
    justify-content: flex-end;
    margin:10px 0px;
}
.screen input{
    text-align: right;
    flex:1;
    font-size: 1.6rem;
    box-shadow: none;
    background-color:rgba(255, 255, 255, 0.036);
    color:white;
}
div .name{
    color:white;
    font-family:Arial, Helvetica, sans-serif;
}
