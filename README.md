# Ex.08 Design of a Standard Calculator
## Date:19/04/24

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
</head>
<body style="background-image: url(math1.jpeg);background-size: cover;">
    <script>
        function fn(e) {

if (e.innerHTML == '=') {

output.value = eval(output.value);

}

else if (e.id == 'back') {

v = output.value;

output.value = v.substring( v.length-1, v.length);

}

else if (e.innerHTML == 'C') {

output.value = '';

}
else if (e.innerHTML == 'π'){
    output.value += 3.14;
}

else 

output.value += e.innerHTML;

}

    </script>
    <div class=" bg-dark row mx-auto text-center" style="width: 24rem;">
        <div ><p style="color: orange; font-family: 'Times New Roman', Times, serif; font-size: 20px;">Nandakesore (212223240103)</p></div>

        <div class="col-12 my-4"><input type="text" name="" id="output"

        
        style="width: 100%; height: 50px; border-radius: 25px;color: black;"></div> <div class="m-3 col-2 btn rounded-4"
        
        onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;">(</div> <div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;">)</div>
        
        <div class="m-3 col-2 btn btn-danger rounded-4" onclick="fn(this)" style="font-family: 'Times New Roman', Times, serif;color: black;">C</div>
        
        <div class="m-3 col-2 btn btn-danger rounded-4" onclick="fn(this)"
        
        id="back" style="font-family: 'Times New Roman', Times, serif;color: black;"><i class="bi bi-backspace"></i>
        
        </div>
        
        <div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">7</div>
        
        <div class="m-3 col-2 btn  rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">8</div>
        
        <div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">9</div>
        
        <div class="m-3 col-2 btn  rounded-4" onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;">*</div>
        <div class="m-3 col-2 btn  rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">4</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">5</div> <div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">6</div>

<div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;color: black;">-</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">1</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">2</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">3</div > <div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;">+</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">0</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: darkorange ;font-family: 'Times New Roman', Times, serif;">.</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;">%</div>

<div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;color: black;">/</div>

<div class="m-3 col-8 btn btn-warning rounded-4" onclick="fn(this)" style="background-color: rgb(255, 255, 255) ;font-family: 'Times New Roman', Times, serif;">=</div><div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: rgb(0, 255, 21);font-family: 'Times New Roman', Times, serif;">π</div>


<div class="m-3 col-2 btn rounded-4"
        
onclick="fn(this)" style="background-color: rgb(0, 255, 21) ;font-family: 'Times New Roman', Times, serif;">x²</div> <div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="background-color: rgb(242, 255, 0) ;font-family: 'Times New Roman', Times, serif;">Sin</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)" style="font-family: 'Times New Roman', Times, serif;color: black;background-color: rgb(242, 255, 0)">Cos</div>

<div class="m-3 col-2 btn rounded-4" onclick="fn(this)"

id="back" style="font-family: 'Times New Roman', Times, serif;color: black;background-color: rgb(242, 255, 0)">Tan</i>

</div>

</div> 

</div>
</body>
</html>
```

## OUTPUT:

![Screenshot (142)](https://github.com/Nandakesore0210/Calc/assets/149365088/471d261a-e4e4-430a-bdee-33a6bbc16336)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
