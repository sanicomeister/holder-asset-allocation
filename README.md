Fiz uma planilha para resolver a pergunta que me faço todo mês: **"com o dinheiro que vou investir agora, o que eu compro e quanto?"**

Ela é uma evolução da lógica da planilha Holder, que muita gente aqui já conhece. Funciona no **Excel 365 e no LibreOffice Calc**, sem macros.

**Como funciona**

1. Você define o % objetivo de cada classe (Ações, FIIs, Renda Fixa, Stocks, REITs, Cripto, Ilíquidos) e de cada ativo dentro da classe.
2. Informa o que já tem (quantidade e preço médio) e o valor do aporte.
3. A planilha calcula o quanto cada item está distante do objetivo (Rebalance Score), divide o aporte entre as classes e entre os ativos, e devolve **quantidade e valor de cada ordem**, já considerando lote/fração, corretagem, IOF e spread.
4. O que sobra do arredondamento de cotas vai para o ativo mais defasado que ainda dá para comprar.

**O que tem**

- 15 abas: Dashboard, Macro Alocação, uma aba por classe, históricos de aportes/dividendos/patrimônio, configurações
- Dashboard com 12 KPIs, plano de compras, 6 gráficos e controle de risco (concentração por ativo, setor, moeda)
- Dividendos: renda passiva mensal, Dividend Yield, Yield on Cost
- Rentabilidade: carteira, por classe, por ativo, acumulada, 12M e por ano
- Cotações automáticas (Yahoo Finance; CoinGecko opcional para cripto), com plano B manual
- Múltiplas moedas, até 920 posições, 10 anos de histórico

**Arquivos**

- Planilha limpa, pronta para usar
- Planilha DEMO com uma carteira fictícia, para ver tudo funcionando
- Manual em PDF (24 páginas) com o passo a passo de preenchimento

**Limitações (para ninguém se frustrar)**

- A cotação automática usa a função WEBSERVICE: funciona no Excel para Windows e no LibreOffice. No Excel para Mac/Web use o modo manual.
- O Yahoo pode limitar consultas. Se falhar, a planilha usa a cotação manual que você deixou preenchida.
- O histórico patrimonial é registrado por você, uma vez por mês.
- Os valores de IOF/spread são os da planilha original; confirme com sua corretora.

Feedback, bugs e sugestões são muito bem-vindos.

*Material educacional, não é recomendação de investimento. Os dados da DEMO são fictícios.*
