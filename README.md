<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proposta Romântica</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
        }
        .message {
            margin-bottom: 20px;
            font-size: 24px;
        }
        .buttons {
            display: flex;
            gap: 20px;
        }
        .btn {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
        .btn-no {
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="message">Vamos dar uns beijos na boca hoje?</div>
    <div class="buttons">
        <button class="btn btn-yes">Sim</button>
        <button class="btn btn-no">Não</button>
    </div>
    <script>
        const btnNo = document.querySelector('.btn-no');
        const btnYes = document.querySelector('.btn-yes');

        btnNo.addEventListener('mouseover', () => {
            const x = Math.random() * (window.innerWidth - btnNo.clientWidth);
            const y = Math.random() * (window.innerHeight - btnNo.clientHeight);
            btnNo.style.left = `${x}px`;
            btnNo.style.top = `${y}px`;
        });

        btnYes.addEventListener('click', () => {
            alert('Ótimo! Vamos!');
        });
    </script>
</body>
</html>
