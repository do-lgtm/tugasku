<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>kalkulator</title>

    <script>
        function hitung()
        {
            var form = document.formhitung;
            var x = eval (form.x.valeu)
            var y = eval (form.y.valeu)
            var pil = form.opt.valeu;
            if (pil == "+")
            {
                var z = x+y;
            } else if (pil == "-")
            {
                var z = x-y;
            } else if (pil == "*")
            {
                var z = x*y;                   
            } else if (pil == "/")
            {
                var z = x/y;
            }
            form.hasil.valeu = z
            form.x.valeu = "";
            form.y.valeu = "";
        }
    </script>
</head>
<body>
    <h1>kalkulator java</h1>
    <form name="formhitung" action="#">
        bil 1 <input type="number" name="x"><br>
        op
        <select>
            <option value="+">+</option>
            <option value="-">-</option>
            <option value="/">/</option>
            <option value="*">*</option>
        </select><br>
        bil 2 <input type="number" name="y"><br>
        <input type="button" value="=" onclick="hitung()"><br>
        HASIL <input type="number" name="hasil" disabled="true">
    </form>
</body>
</html>
