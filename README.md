### Manipulando Arquivos Excel

- Este é um exemplo simples de como manipular arquivos Excel usando a biblioteca Python openpyxl. Você pode seguir este guia para criar e preencher um arquivo Excel com informações básicas, como seu nome e idade.

### Instalação

# Antes de começar, você precisa ter a biblioteca openpyxl instalada. Você pode instalá-la usando o comando pip:
pip install openpyxl

### Código de Exemplo

- Aqui está um código Python que cria um arquivo Excel chamado "exemplo.xlsx" e preenche as colunas "Seu nome" e "Sua idade" com informações fictícias:

# Importar bibliooteca
import openpyxl as xl

# Cria um novo arquivo Excel
arquivo = xl.Workbook()

# Seleciona a aba ativa (por padrão, há uma aba criada chamada 'Sheet')
aba = arquivo.active

# Adiciona títulos às colunas
aba['A1'] = 'Seu nome'
aba['B1'] = 'Sua idade'

# Preenche com informações fictícias (substitua com seus próprios dados)
aba['A2'] = 'João da Silva'
aba['B2'] = 30

# Salva o arquivo Excel
arquivo.save('exemplo.xlsx')

### Executando o Código
- Depois de escrever o código acima, você pode executá-lo. Isso criará um arquivo Excel chamado "exemplo.xlsx" no diretório em que você está executando o código, com os títulos e informações que você definiu.