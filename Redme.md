# Aplicação POWER-BI ( MKT-Faturamento)

> Breve descrição sobre mim: Meu Nome é Paulo Matheus Gomes e sou apaixonado por dados, atualmente faço uma pós graduação em Ciência de Dados e Machine Learning na Fiap.

<img src="https://media.licdn.com/dms/image/v2/D4D03AQE3Ako91luc9Q/profile-displayphoto-shrink_800_800/profile-displayphoto-shrink_800_800/0/1730928598467?e=1744243200&v=beta&t=THh9lQY5HsbcdeV1wTiERnGygRbx8mpUlecZEkMRvc8" alt="Logo" width="200"/>

> Breve descrição e finalidade do Projeto.

## Índice

- [Descrição](#descrição)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Pré-Requisitos](#pré-requisitos)
- [Link-Git](#link-git)
- [Contato](#contato)
- [Uso](#uso)

## Descrição

Projeto de aplicação Power BI com o objetivo de Visualizar os principáis indicadores envolvendo Faturamento da Empresa. Foi desenvolvido em linguagem Dax.

Exemplo:
- Este projeto facilita o controle de informações ao realizar requisições para visualizar indicadores, metas e seus melhores meses.

## Tecnologias Utilizadas

- **Figma.fg** - Design de Dashboards (Storytelling).
- **Power BI** - Desenvolvimento das Requisições e visualização no Power BI.
- **Vercel** - Framework para hospedgem de aplicação web.
- **SQL** - Linguagem SQL usado no Back-end de algumas tabelas como dcalendario e data de carga.
- **Sharepoint** - Tecnologia que hospedou a tabela de Receitas na Web.

## Pré-Requisitos

Antes de começar, você precisa ter o seguinte instalado na sua máquina:

- [Figma.fg](https://www.figma.com/) (Versão 14 ou superior)
- [Power-BI](https://login.microsoftonline.com/)
- [Python](https://python.org.br/instalacao-windows/)
- [SQL](https://www.microsoft.com/pt-br/sql-server/sql-server-2022)

Certifique-se de que o serviço esteja em execução se estiver utilizando localmente.

## Link-Git

1. Clone o repositório:
    ```bash
    git clone https://github.com/Paullo-Matheus/Projeto_Fiap_Fase01.git
    ```

2. Navegue até o diretório do projeto:
    ```bash
    cd Projeto_Fiap_Fase01
    ```

Acesse o endereço local: `http://localhost:5000/swagger`.

## Contato

- **E-mail**: Paullomatheus.226@gmail.com
- **E-mail**: Paulo.maraujo@telefonica.com
- **RM**: A0152641
- **Celular**: (11)-99235-6351 

## Link Acesso

`https://app.powerbi.com/links/3UmY307WWk?ctid=9744600e-3e04-492e-baa1-25ec245c6f10&pbi_source=linkShare`




## Uso

`uso.py` 

```python
import sys
import os

Print("Segue link do Relatório:")

#Power-BI
https://app.powerbi.com/links/3UmY307WWk?ctid=9744600e-3e04-492e-baa1-25ec245c6f10&pbi_source=linkShare

# Adicionando o caminho da pasta 'src' e path guardando o link em diretório
link_powerbi = "https://app.powerbi.com/links/3UmY307WWk?ctid=9744600e-3e04-492e-baa1-25ec245c6f10&pbi_source=linkShare"
with open("link_powerbi.txt", "w") as file:
    file.write(link_powerbi)


from routes.api_routes import init_routes
from server.instancia import server
from flask_restx import Api

