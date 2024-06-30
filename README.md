<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FerraridaSorte</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 15px 0;
            text-align: center;
        }
        .container {
            width: 80%;
            margin: 0 auto;
            padding: 20px;
        }
        .raffle-item {
            background-color: white;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            padding: 20px;
        }
        .raffle-item h2 {
            margin-top: 0;
        }
        .raffle-item p {
            margin: 10px 0;
        }
        .raffle-item button {
            background-color: #4CAF50;
            border: none;
            color: white;
            padding: 10px 20px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            border-radius: 5px;
            cursor: pointer;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #f1f1f1;
            position: absolute;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bem-vindo à FerraridaSorte</h1>
    </header>
    <div class="container">
        <div class="raffle-item">
            <h2>Prêmio:</h2>
            <p>Descrição do prêmio e detalhes sobre a rifa.</p>
            <form id="raffleForm">
                <label for="name">Nome:</label><br>
                <input type="text" id="name" name="name"><br><br>
                <label for="number">Número do Bilhete:</label><br>
                <input type="text" id="number" name="number"><br><br>
                <label for="phone">Celular:</label><br>
                <input type="text" id="phone" name="phone"><br><br>
                <button type="button" onclick="submitForm()">Enviar</button>
            </form>
        </div>
    </div>
    <footer>
        <p>&copy; 2024 FerraridaSorte. Todos os direitos reservados. | Contato: <a href="mailto:jhol1986@hotmail.com">jhol1986@hotmail.com</a></p>
    </footer>

    <script>
        function submitForm() {
            // Obter os valores dos campos
            var name = document.getElementById('name').value;
            var number = document.getElementById('number').value;
            var phone = document.getElementById('phone').value;

            // Validar se os campos estão preenchidos
            if (name === '' || number === '' || phone === '') {
                alert('Por favor, preencha todos os campos.');
                return;
            }

            // Exibir os valores (ou enviar para um servidor)
            alert('Nome: ' + name + '\nNúmero do Bilhete: ' + number + '\nCelular: ' + phone);

            // Limpar o formulário após o envio
            document.getElementById('raffleForm').reset();
        }
    </script>
</body>
</html>

