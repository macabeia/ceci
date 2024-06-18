<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Site Pessoal</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 50px;
        }
        input[type="password"] {
            padding: 10px;
            font-size: 16px;
            margin-bottom: 20px;
        }
        input[type="submit"] {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #007bff;
            color: #fff;
            border: none;
        }
        input[type="submit"]:hover {
            background-color: #0056b3;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <form id="passwordForm">
        <label for="password">Digite a senha:</label><br>
        <input type="password" id="password" name="password"><br>
        <input type="submit" value="Enviar">
    </form>
    <div id="photo" class="hidden">
        <img src="" alt="Foto">
    </div>

    <script>
        document.getElementById('passwordForm').addEventListener('submit', function(event) {
            event.preventDefault();
            var password = document.getElementById('password').value;
            if (password === '01/04/2022') {
                document.getElementById('photo').innerHTML = '<img src="https://drive.google.com/uc?id=19N_ANeB8CJK_jTGr_Vwvii1UsBXmSRZI" alt="Foto">';
                document.getElementById('photo').classList.remove('hidden');
            } else {
                alert('Senha incorreta. Tente novamente.');
            }
        });
    </script>
</body>
</html>
# ceci
