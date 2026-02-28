README_FOLHA_DE_PAGAMENTO_AUTOMATIZADO
============================================================

Sistema de Conferência de Pagamentos por CPF
------------------------------------------------------------

Descrição
------------------------------------------------------------
Script desenvolvido em Python para execução no Google Colab,
com o objetivo de automatizar a conferência de pagamentos
entre duas planilhas Excel:

- Planilha do Banco
- Planilha da Empresa

A validação é realizada utilizando o CPF como chave principal
de correspondência entre as bases.


Funcionalidades
------------------------------------------------------------
- Leitura automática das duas planilhas
- Identificação do arquivo do banco e da empresa pelo nome
- Comparação de CPFs
- Busca da matrícula correspondente na base do banco
- Geração de planilha final consolidada
- Indicação de "Não Cadastrado no Banco" quando o CPF não é encontrado


Estrutura Esperada das Planilhas
------------------------------------------------------------

1) Planilha do Banco
   Coluna C (Index 2) → CPF
   Coluna D (Index 3) → Matrícula

2) Planilha da Empresa
   Coluna B (Index 1) → Nome do Beneficiário
   Coluna D (Index 3) → CPF
   Coluna H (Index 7) → Valor


Fluxo de Execução
------------------------------------------------------------
1. Executar o código no Google Colab
2. Fazer upload dos dois arquivos:
   - Um contendo "banco" no nome
   - Um contendo "empresa" no nome
3. Informar a Data de Competência
4. Aguardar o processamento
5. Realizar o download da planilha final gerada


Arquivo Gerado
------------------------------------------------------------
Planilha_Pagamento_Final_Por_CPF.xlsx

A planilha final contém:
- Nome do Beneficiário
- CPF
- Valor
- Data de Competência
- Matrícula (ou aviso de não cadastro)


Tecnologias Utilizadas
------------------------------------------------------------
- Python 3
- Pandas
- Google Colab


Objetivo
------------------------------------------------------------
Reduzir erros manuais na conferência de folha de pagamento,
automatizar validações e aumentar a eficiência do processo
financeiro.
============================================================