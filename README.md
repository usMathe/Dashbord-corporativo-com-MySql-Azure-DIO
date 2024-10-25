# Dashbord-corporativo-com-MySql-Azure

![Dashboard da Empresa](relatorio-analise-empresa.png)

O objetivo era a criação de um painel no Power BI integrado a uma base de dados no MySQL hospedado na Azure, antes da criação a ideia era realizar a transformações dos dados para que eles estivesem aptos para a criação desse relatório no PowerBI.

1. **Criação de Instância MySQL no Azure:**
   - Uma instância do banco de dados MySQL foi provisionada na Azure, permitindo o armazenamento e consulta da base de dados da empresa.

2. **Criação do Banco de Dados:**
   - O banco foi criado com dados disponíveis no GitHub e o banco de dados foi integrado ao Power BI, possibilitando a visualização e manipulação dos dados em relatórios interativos.

3. **Verificação de Cabeçalhos e Tipos de Dados:**
   - Os cabeçalhos e tipos de dados foram revisados para garantir a consistência. Tipos de dados incorretos foram ajustados conforme necessário.

4. **Valores Monetários:**
   - Todos os valores de salário foram convertidos para o tipo de dado `double` preciso, permitindo cálculos mais detalhados.

5. **Verificação de Nulos:**
   - Verificou-se a existência de valores nulos, principalmente na coluna `Super_ssn`. Os colaboradores com `Super_ssn` nulos foram tratados como gerentes, e lacunas foram preenchidas.

6. **Mescla de Colunas Complexas:**
   - Colunas que apresentavam dados redundantes ou complexos foram mescladas. Nome e Sobrenome dos colaboradores foram unidos em uma única coluna para facilitar a leitura.

7. **Associação de Colaboradores com Departamentos:**
   - As tabelas de colaboradores e departamentos foram mescladas, criando uma única tabela que relaciona cada colaborador ao seu respectivo departamento.

8. **Mescla de Departamentos e Localizações:**
   - Departamentos e localizações foram mesclados, criando combinações únicas. Essa etapa é essencial para a criação de um modelo estrela futuro.

9. **Remoção de Colunas Desnecessárias:**
   - Foram eliminadas colunas que não seriam utilizadas no relatório final, simplificando o modelo de dados.

## Relatório no Power BI:

10. **Análise Salarial:**
    - Um gráfico de barras mostra a soma de salários por colaborador, ajudando a visualizar quais funcionários têm os maiores salários.

11. **Distribuição por Departamento:**
    - Um gráfico de pizza exibe a quantidade de funcionários por departamento, facilitando a visualização da distribuição da força de trabalho.

12. **Salário por Cidade:**
    - Um gráfico de linha destaca a soma de salários por cidade, indicando quais localizações têm a maior concentração de remuneração.

13. **Quantidade de Projetos por Departamento:**
    - Um gráfico de barras mostra o número de projetos alocados a cada departamento, com destaque para a Administração.
