<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web cek usia</title>
    <link rel="stylesheet" href="style.css"
</head>
<body>
    <div class="contener">
        <h2>Cek Usia Anda</h1>
        <label>masukan tahun kelahiran anda</label>
        <input type="number" placeholder="contoh: 1945" id="birthday"/>
        <button id="check-button" onclick="checkResult()">cek usia</button>
        <p class="result" id="resultView"></p>
    </div> 

    <script>

        function checkResult(){
         const birthdayInput = document.getElementById("birthday")
         const birthday = birthdayInput.value;   
       
         const now = new Date().getFullYear(); 
         const age = now - birthday
        
         const resultView = document.getElementById("resultView")
         resultView.innerHTML = "usia anda saat ini adalah " + age
        }
    </script>       
</body>
</html>
