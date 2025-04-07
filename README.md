o projeto é uma automação de cadastro de produtos utilizando Python e a biblioteca PyAutoGUI.
Objetivo do Projeto
O código automatiza o cadastro de produtos em um sistema web, abrindo o navegador, acessando a página de login, inserindo as credenciais e preenchendo os campos com os dados de um arquivo CSV.
Passo a Passo do Código:
1. Abrir o Navegador e Acessar o Sistema
Usa PyAutoGUI para abrir o Google Chrome.

Digita o endereço do site de login: https://dlp.hashtagtreinamentos.com/python/intensivao/login.

Aguarda 10 segundos para garantir que a página carregue.

2. Fazer Login
Clica no campo de e-mail e digita pythonimpressionador@gmail.com.

Usa TAB para mudar para o campo de senha e digita "sua senha".

Clica no botão de login e aguarda 10 segundos para garantir o carregamento.

3. Importar a Base de Dados
Lê o arquivo produtos.csv usando Pandas.

Exibe os dados carregados para conferência.

4. Cadastrar os Produtos
Itera sobre cada linha da tabela e preenche os campos na página com os dados:

Código do produto

Marca

Tipo

Categoria

Preço unitário

Custo

Observações (se existirem)

Após preencher tudo, aperta Enter para confirmar o cadastro.

Usa scroll para garantir que a página não fique travada.

5. Repetir até Cadastrar Todos os Produtos
O processo se repete até que todos os produtos do produtos.csv tenham sido cadastrados.

Arquivos do Projeto
projeto.py – Script principal de automação.

produtos.csv – Arquivo contendo os produtos a serem cadastrados.

auxilio.py – Um script auxiliar que espera 10 segundos e imprime a posição do mouse (provavelmente para ajustar os cliques do pyautogui).
