# PROJETO ETL NO SQL
## INSERÇÃO DE DADOS NO SQL SERVER

 <img align="center" alt="html5" src="https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927.svg?style=for-the-badge&logo=Microsoft-SQL-Server&logoColor=white" />

**Problema:** 

- Arquivo em .csv em um diretório que precisa estar em um banco de dados para posterior análise em uma ferramenta de SSBI.

 **Objetivo:** 

- Criar um banco de dados para o arquivo;
-  Inputar no banco de dados o arquivo recebido;
-  Normalizar os dados;
-  Criar _procedure_ para automação do processo.

**Ferramentas:**

- Solução desenvolvida 100% no **SQL Server** com o uso de sripts SQL.


### Projeto

O projeto consiste em automatizar a extração dos dados de um arquivo .csv dentro de um diretório e normalizar os dados em tabelas fato e dimensão, garantindo a governança de disponibilização dos dados em um único local para posterior análise dos dados.

![PIPELINE](https://github.com/user-attachments/assets/ac680a00-6104-499b-9748-716ff79cf072)

**Passos:**

- Criação do banco de dados;
- Criação da tabela transacional;
- Criação das tabelas dimensões e fato;
- Truncate em todas as tabelas;
- Insert de dados nas tabelas criadas;
- Truncate na tabela transacional;
- Criação da procedure.


- Arquivo .CSV Desnormalizado:

![ARQUIVO CSV](https://github.com/user-attachments/assets/deaa40ff-3182-42bd-832d-436ba509e6a1)


- Tabela Fato Normalizada:

![RESULTADO FINAL](https://github.com/user-attachments/assets/c238dd66-f457-4244-a246-dd679640bc86)


### Conclusão

A escolha do  insert incremental ou por truncate (limpar tabelas existentes) vai depender da necessidade do negócio. Neste caso, foi usado a forma de inputar todos os dados do arquivo, levando cerca de alguns segundos para a realização da tarefa.
Existe outras formas e feramentas que chagam neste mesmo objetivo, poré, o principal objetivo aqui é o desenvolvimento do conhecimento.
