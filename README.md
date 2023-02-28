# diamond-pattern

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diamond Patten print</title>
</head>
<body>
    <script>
       let n = 5;
let string = "";
// Upside pyramid
for (let i = 1; i <= n; i++) {
  
  for (let j = n; j > i; j--) {
    string += " ";
  }
  
  for (let k = 0; k < i * 2 - 1; k++) {
    string += "*";
  }
  string += "\n";
}
// downside pyramid
for (let i = 1; i <= n - 1; i++) {
  
  for (let j = 0; j < i; j++) {
    string += " ";
  }
  
  for (let k = (n - i) * 2 - 1; k > 0; k--) {
    string += "*";
  }
  string += "\n";
}
console.log(string);
    </script>
</body>
</html>
