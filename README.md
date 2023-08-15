# datasus-al-2014-2023

Olá, Meu nome é Marcelo Mesquita e este é um projeto de ETL que fiz para minha a Dra. Tainá Teixeira (http://lattes.cnpq.br/7917475836129025), também conhecida como minha esposa.

Para realizar algumas análises para um cliente dela, precisamos coletar dados do SIH/SUS - Sistema de Informações Hospitalares do SUS. Nesse projeto realizamos o download dos arquivos de informações de 2014 a 2023 para o estado de Alagoas e realizamos a limpeza e processamento dos dados obtidos via arquivos .dbc.

Como os arquivos .dbc precisam de um aplicativo específico chamado tabnet, que não nos permite realizar a extração em massa, utilizamos uma biblioteca de python chamada PySUS para fazer o download via FTP e converter os dados em DataFrames do Pandas.

Para facilitar a reutilização dos dados, inserimos os dados em um banco MySQL hospedado na Hostinger.

Por fim, apenas para fins acadêmicos, criei um dashboard em Power BI para apresentar os dados de maneira mais acessível.

