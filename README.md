# projeto-CSS
Projeto de grupo de estudos do curso de análise e desenvolvimento de sistemas  

Estrutura Básica: O código começa com a definição do tipo de documento HTML e a configuração da linguagem, charset e viewport para dispositivos móveis.

Bootstrap: O link para a folha de estilo do Bootstrap é incluído no cabeçalho, permitindo o uso de classes de estilo pré-definidas.

CSS Interno: Estilos personalizados são definidos dentro da tag <style> para ajustar a aparência de elementos como body, h1, p, botões e tabelas.

Conteúdo: O corpo da página contém um cabeçalho, três seções (introdução, tabela de dados e um formulário) e um rodapé.

Tabela e Formulário: A tabela usa classes do Bootstrap para uma aparência consistente e um formulário simples é apresentado com campos de entrada.

Interatividade: Um botão estilizado muda de cor quando o mouse passa sobre ele, demonstrando a interatividade simples do CSS.


---------------------------------------------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo de CSS e Bootstrap</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f9fa;
            color: #333;
        }

        h1 {
            color: #007bff;
            text-align: center;
        }

        p {
            font-size: 1.2em;
            line-height: 1.5;
        }

        .button {
            background-color: #28a745;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #218838;
        }

        .custom-table {
            margin: 20px 0;
        }

        /* Estilo para a tabela */
        .custom-table th, .custom-table td {
            text-align: center;
            padding: 15px;
        }

        .custom-table th {
            background-color: #007bff;
            color: white;
        }

        /* Seletores de classe */
        .important {
            font-weight: bold;
            color: red;
        }
    </style>
</head>
<body>

    <header>
        <h1>Bem-vindo ao Exemplo de CSS e Bootstrap</h1>
    </header>

    <main class="container">
        <section>
            <h2>Seção de Introdução</h2>
            <p>Este é um exemplo que demonstra como usar CSS para estilizar páginas web. O CSS separa o conteúdo do estilo, permitindo uma melhor manutenção.</p>
            <button class="button">Clique aqui</button>
        </section>

        <section>
            <h2>Tabela de Dados</h2>
            <table class="table table-bordered custom-table">
                <thead>
                    <tr>
                        <th>Nome</th>
                        <th>Idade</th>
                        <th>Cidade</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>João</td>
                        <td>25</td>
                        <td>São Paulo</td>
                    </tr>
                    <tr>
                        <td>Maria</td>
                        <td>30</td>
                        <td>Rio de Janeiro</td>
                    </tr>
                    <tr>
                        <td class="important">Carlos</td>
                        <td class="important">35</td>
                        <td class="important">Belo Horizonte</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <section>
            <h2>Formulário Exemplo</h2>
            <form>
                <div class="form-group">
                    <label for="nome">Nome:</label>
                    <input type="text" class="form-control" id="nome" placeholder="Digite seu nome">
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" class="form-control" id="email" placeholder="Digite seu email">
                </div>
                <button type="submit" class="button">Enviar</button>
            </form>
        </section>
    </main>

    <footer class="text-center" style="margin-top: 20px;">
        <p>&copy; Prof. Iago Ricardo. Exemplo de CSS. Todos os direitos reservados.</p>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.0.7/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
