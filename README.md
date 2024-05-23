# calculater-task
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.2/dist/umd/popper.min.js" integrity="sha384-IQsoLXl5PILFhosVNubq5LC7Qb9DXgDA9i+tQ8Zj3iwWAwPtgFTxbJ8NT4GN1R8p" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.min.js" integrity="sha384-cVKIPhGWiC2Al4u+LWgxfKTRIcfu0JTxR+EQDz/bgldoEyl4H0zUF0QKbrJ0EcQF" crossorigin="anonymous"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>
    <div class="container">
        <form name="calculation">
            <div class="row">
                <div class="col-4">
                    <label>Enter A value </label>
                    <input type="number" name="aValue" id="aValue" class="form-control">
                </div>
                <div class="col-4">
                    <label>Enter B value </label>
                    <input type="number" name="bValue" id="bValue" class="form-control">
                </div>
                <div class="col-4">
                    <label>C Value &nbsp;&nbsp;&nbsp;</label><label id="functionType" class="text-danger" ></label>
                    <input type="number" name="cValue" id="cValue" class="form-control" readonly>
                </div>
            </div>
        </form>
        <div class="row mt-3">
            <div class="col-3 text-center"><button class="btn btn-primary btn-sm" onclick="Addition()" type="button"><i class="fa-solid fa-plus"></i>&nbsp;&nbsp;Addition</button></div>
            <div class="col-3 text-center"><button class="btn btn-danger btn-sm" onclick="Subtraction()" type="button"><i class="fa-solid fa-minus"></i>&nbsp;&nbsp;Subtraction</button></div>
            <div class="col-3 text-center"><button class="btn btn-success btn-sm" onclick="Multiplication()" type="button"><i class="fa-solid fa-xmark"></i>&nbsp;&nbsp;Multiplication</button></div>
            <div class="col-3 text-center"><button class="btn btn-info btn-sm" onclick="Division()" type="button"><i class="fa-solid fa-divide"></i>&nbsp;&nbsp;Division</button></div>
        </div>
    </div>
</body>
</html>
<script>
    function Addition(){
        var a=document.getElementById("aValue").value;
        var b=document.getElementById("bValue").value;
        var c=document.getElementById("cValue");
        var ft=document.getElementById("functionType");
        c.value=Number(a)+Number(b)
        ft.innerHTML="Addition Function"
    }
    function Subtraction(){
        var a=document.getElementById("aValue").value;
        var b=document.getElementById("bValue").value;
        var c=document.getElementById("cValue");
        var ft=document.getElementById("functionType");
        c.value=Number(a)-Number(b)
        ft.innerHTML="Subtraction Function"
    }
    function Multiplication(){
        var a=document.getElementById("aValue").value;
        var b=document.getElementById("bValue").value;
        var c=document.getElementById("cValue");
        var ft=document.getElementById("functionType");
        c.value=Number(a)*Number(b)
        ft.innerHTML="Multiplication Function"
    }
    function Division(){
        var a=document.getElementById("aValue").value;
        var b=document.getElementById("bValue").value;
        var c=document.getElementById("cValue");
        var ft=document.getElementById("functionType");
        c.value=Number(a)/Number(b)
        ft.innerHTML="Division Function"
    }
</script>
