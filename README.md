# p2


<!DOCTYPE html>
<head>
<title>Tip Calculator</title>
<link href="style.css" rel="stylesheet" type="text/css">
</head>

<body>
<div id="wrapper">
    <header>
        <h1>Tip Calculator</h1>
    </header>
    <form>
        Amount: $<input id="bill" type="text">
        <br>
        <button onclick="calc()">Calculate</button>
        <br>
        Tip: <span id="tip"></span>
        <br>
        Total: <span id="total"></span>
    </form>
</div>
<script>
    function calc() {
        var bill = document.getElementById('bill').value;
        var tip = bill * .15;
        var total = bill + tip;

        document.getElementById("tip").innerHTML= "$"+(tip).toFixed(2);
        document.getElementById("total").innerHTML= "$"+(total).toFixed(2);         
    }
</script>
</body>
