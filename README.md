<html lang="hu">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eljönnél velem korizni?</title>
    <style>
        body {
            background-color: black;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        label {
            margin: 10px 0;
        }
    </style>
</head>
<body>
    <h1>Eljönnél velem korizni Budapestre kettesben?</h1>
    <h2>(A jegyek már megvannak) </h2>
    
    <form id="korizniForm">
        <label>
            <input type="radio" name="korizni" value="igen" id="igenRadio"> Igen
        </label>
        <label>
            <input type="radio" name="korizni" value="nem" id="nemRadio"> Nem
        </label>
        <button type="button" onclick="ellenoriz()">Küldés</button>
    </form>

    <script>
        function ellenoriz() {
            var igenRadio = document.getElementById("igenRadio");
            
            if (igenRadio.checked) {
                alert("Gyere oda, elmagyarázom!");
            } else {
                alert("Sajnálom, hogy nem jössz el. Talán legközelebb!");
            }
        }
    </script>
</body>
</html>
