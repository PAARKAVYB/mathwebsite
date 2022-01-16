# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Math Website</title>
    <style>
        * {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
body {
  background-color:rgb(168, 203, 226);
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
}
.content {
  display: block;
  width: 100%;
  background-color: #db94d5;
  min-height: 500px;
  margin-top: 50px;
}

h1{
    text-align: center;
    padding-top: 50px;
    color: rgb(36, 23, 23);
}
.formelement{
    text-align: center;
    font-size:xx-large;
    margin-top: 5px;
    margin-bottom: 5px;
}
.footer{
    didplay:inline-block;
    width: 100%;
    height :35px;
    background-color: rgb(118, 145, 204);
    color: black;
    text-align: center;
    padding-top: 10px;
    font-size: large;
}
    </style>
</head>
<body><div class="container">
  <div class="content">
            <h1>VOLUME OF  A CYLINDER</h1>
            <form>
                <div class=formelement>
                    <lable for="bedit">Radius:</lable>
                    <input type="text" id="bedit" value=""/>Meters
                </div><br>
                <div class=formelement>
                    <lable for="aedit">Height:</lable>
                    <input type="text" id="aedit" value=""/>Meters
                </div><br>
                
                <div class=formelement>
                    <input type="button" value="CALCULATE VOLUME" id="calbutton1"/>
                </div>
                <div class=formelement>
                    <lable for="cedit">Volume:</lable>
                    <input type="text" id="cedit" readonly="0"/>Cubic Meters
                </div><br>
               
            </form>
        </div>
         <div class="footer">Developed by Paarkavy B</div>
         </div>
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton1");
            button.addEventListener("click",function(){
                var atext,btext,ctext;
                var aval,bval,cval;
                atext=document.querySelector("#aedit");
                btext=document.querySelector("#bedit");
                ctext=document.querySelector("#cedit");

                aval=parseInt(atext.value);
                bval=parseInt(btext.value);
                cval=22/7*aval*bval*bval;
                ctext.value=cval;
                ctext.value=cval;
            });
        </script>
         <div class="container">
        <div class="content">
            <h1>AREA OF A RECTANGLE</h1>
            <form>
                <div class="formelement">
                  <lable for="lengthedit">Length:</lable>
                  <input type="text" id="lengthedit" value=" "/>Meters
                </div><br>
                <div class="formelement">
                  <lable for="breadthedit">Breadth:</lable>
                  <input type="text" id="breadthedit" value=" "/>Meters
                </div><br>
                <div class="formelement">
                  <input type="button" value="CALCULATE AREA" id="calbutton2"/>
                </div><br>
                <div class="formelement">
                  <lable for="areaedit">Area:</lable>
                  <input type="text" id="areaedit" readonly="0"/>Square Meters
                </div><br>
                <div class="formelement">
               
                </div><br>
                
            </form>
          </div>
          <div class="footer">Developed by Paarkavy B</div>
        </div>
        <script type="text/javascript">
          var button;
          button=document.querySelector("#calbutton2");
          button.addEventListener("click",function(){
            
              var lengthtext,breadthtext,areatext;
              var aval,bval,cval;
    
              lengthtext=document.querySelector("#lengthedit");
              breadthtext=document.querySelector("#breadthedit");
              areatext=document.querySelector("#areaedit");
      
              aval=parseInt(lengthtext.value);
              bval=parseInt(breadthtext.value);
              cval=aval*bval
              areatext.value=cval;
        
      
            });
      
        </script> 
  
</body>
</html>






## OUTPUT:

![output](mathwebsite.png)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
