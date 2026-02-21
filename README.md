💱 Conversor de Moedas – Aplicação Desktop em Python

Aplicação desktop desenvolvida em Python para conversão de moedas utilizando dados de cotação em tempo real por meio de integração com API externa.

O projeto combina desenvolvimento de interface gráfica com lógica de backend, consumo de API e manipulação de dados em XML.

🚀 Funcionalidades

Seleção dinâmica de moeda de origem e destino

Carregamento automático das conversões disponíveis

Consulta de cotação em tempo real via API

Exibição clara do resultado da conversão

Botão para inverter moedas (origem ↔ destino)

Lista rolável com moedas disponíveis

Interface moderna em modo escuro utilizando CustomTkinter

Validação de conversões indisponíveis

🛠 Tecnologias Utilizadas

Python 3

CustomTkinter – Interface gráfica moderna

Requests – Requisições HTTP para API de cotação

xmltodict – Leitura e conversão de arquivos XML

AwesomeAPI – Fonte das cotações em tempo real

Programação orientada a eventos

Arquitetura modular (separação de responsabilidades)

📂 Estrutura do Projeto
currency-converter/
│── main.py
│── pegar_moedas.py
│── pegar_cotacao.py
│── moedas.xml
│── conversoes.xml

🔹 main.py

Responsável por:

Criação da interface gráfica

Organização dos componentes visuais

Manipulação de eventos (botões e seleção de moedas)

Integração entre interface e lógica de negócio

🔹 pegar_moedas.py

Responsável por:

Leitura dos arquivos XML

Extração das moedas disponíveis

Construção dinâmica do dicionário de conversões

🔹 pegar_cotacao.py

Responsável por:

Realizar requisição HTTP para a API

Interpretar resposta em JSON

Retornar a cotação da moeda solicitada

🔄 Como Funciona

O sistema lê os arquivos XML que definem:

Moedas disponíveis

Conversões permitidas

Ao selecionar a moeda de origem:

O sistema carrega dinamicamente as moedas de destino válidas

Ao clicar em "Converter":

É feita uma requisição à API de cotação

O valor da moeda é extraído do JSON retornado

A interface é atualizada com o resultado

O botão "Inverter":

Troca moeda de origem e destino

Verifica se a conversão inversa está disponível

Atualiza dinamicamente os campos

🧠 Conceitos Aplicados

Separação de responsabilidades (interface vs lógica)

Consumo de API REST

Manipulação de JSON

Leitura e processamento de XML

Estruturas de dados (dicionários)

Programação orientada a eventos

Validação de dados

Organização modular de projeto

▶️ Como Executar
git clone https://github.com/TMaia0110/currency-converter-python.git
cd currency-converter-python
pip install customtkinter requests xmltodict
python main.py

📌 Melhorias Futuras

Campo para inserir valor personalizado (não apenas 1 unidade)

Tratamento de exceções para falhas na API

Indicador visual de carregamento durante requisição

Implementação de testes automatizados

🎯 Objetivo do Projeto

Este projeto foi desenvolvido com o objetivo de praticar:

Desenvolvimento de aplicações desktop

Integração com APIs externas

Estruturação de projetos Python em múltiplos módulos

Organização de código com foco em boas práticas
