<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio | Rávila Costa</title>
    
    <style>
        :root {
            --primary: #2563eb;
            --dark: #1e293b;
            --light: #f8fafc;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--light);
            color: var(--dark);
            display: flex;
            justify-content: center;
            padding: 40px 20px;
            margin: 0;
        }

        .container {
            background: white;
            max-width: 600px;
            width: 100%;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-top: 8px solid var(--primary);
        }

        h1 { color: var(--primary); margin-bottom: 5px; }
        .subtitle { font-weight: bold; color: #64748b; margin-bottom: 20px; }
        
        .section {
            background: #f1f5f9;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        ul { padding-left: 20px; }
        li { margin-bottom: 5px; }

        .btn-contato {
            background: var(--primary);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 6px;
            cursor: pointer;
            width: 100%;
            font-size: 16px;
            transition: 0.3s;
        }

        .btn-contato:hover { background: #1d4ed8; }
        #log-status { 
            margin-top: 15px; 
            font-family: monospace; 
            font-size: 0.9em; 
            color: #059669; 
            text-align: center;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Rávila Costa</h1>
        <p class="subtitle">Técnico em Desenvolvimento de Sistemas (4º Semestre)</p>

        <div class="section">
            <strong>🔭 Foco Atual:</strong>
            <p>Internet das Coisas (IoT) e Implantação de Sistemas.</p>
        </div>

        <div class="section">
            <strong>📒 Disciplinas Cursadas:</strong>
            <ul id="lista-disciplinas">
                </ul>
        </div>

        <button class="btn-contato" onclick="executarSimulacao()">Simular Deploy (JS + Log Java)</button>
        <div id="log-status"></div>
    </div>

    <script>
        const disciplinas = [
            "Lógica de Programação", "Programação de Aplicativos", 
            "Banco de Dados", "Modelagem de Sistema", 
            "Desenvolvimentos de Sistema", "Teste de Sistema"
        ];

        // Populando a lista dinamicamente
        const listaUl = document.getElementById('lista-disciplinas');
        disciplinas.forEach(item => {
            let li = document.createElement('li');
            li.textContent = item;
            listaUl.appendChild(li);
        });

        function executarSimulacao() {
            const status = document.getElementById('log-status');
            status.innerText = "Status: Sistema Implantado com Sucesso! (Verifique o código-fonte para ver o Java)";
            console.log("Rávila Costa: Candidata selecionada para estágio.");
        }
    </script>

    </body>
</html>
