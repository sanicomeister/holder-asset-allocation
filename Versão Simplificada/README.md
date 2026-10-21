# 🎯 HOLDER PREMIUM · Versão Simplificada

### Só o que importa: **o plano de compras do mês**

[⬅️ Voltar ao projeto](../README.md)

<div align="center">

<img src="../docs/img/dashboard-simplificada.png" alt="Dashboard da versão Simplificada" width="680">

</div>

---

## 🧭 Para quem é

✅ **É para você se:**

- você quer saber **o que comprar e quanto** a cada aporte, sem fazer conta;
- você já acompanha **preço médio, dividendos, rentabilidade e patrimônio** em outro app (MyProfit, por exemplo);
- você prefere uma planilha **leve e rápida de usar**.

❌ **Não é para você se:**

- você quer **controlar preço médio, dividendos e rentabilidade** dentro da planilha. Nesse caso, use a [🏦 Versão Premium](../Vers%C3%A3o%20PREMIUM).

## 📦 Arquivos

| Arquivo | O que é |
|---|---|
| 📗 [`HOLDER_PREMIUM_Simplificada.xlsx`](HOLDER_PREMIUM_Simplificada.xlsx) | Versão **limpa**, pronta para usar. Vem com objetivos de exemplo (40/20/20/10/5/5/0) e aporte de R$ 500, que você altera |
| 🧪 [`HOLDER_PREMIUM_Simplificada_DEMO.xlsx`](HOLDER_PREMIUM_Simplificada_DEMO.xlsx) | Mesma planilha com uma **carteira fictícia** (cerca de R$ 55 mil) para ver tudo funcionando |
| 📘 [`HOLDER_PREMIUM_Simplificada_Manual.pdf`](HOLDER_PREMIUM_Simplificada_Manual.pdf) | Manual passo a passo (14 páginas) |

## 🔁 Seu fluxo mensal em 5 passos

1. 💰 **Digite o valor do aporte** na célula azul no topo do Dashboard.
2. 👀 **Leia o PLANO DE COMPRAS**: ativo, quantidade e valor de cada ordem.
3. 🛒 **Compre no home broker.**
4. ✏️ **Atualize a Quantidade** dos ativos comprados (some o que comprou).
5. 🏦 Na **Renda Fixa** e nos **Ilíquidos**, some o valor aplicado ao **Valor Atual**.

> 💡 **Atalho:** se você comprou **exatamente** o que a planilha sugeriu, copie a coluna **Qtd. Após Compra** e cole como **valores** sobre a coluna **Quantidade**.

## 🗂️ As 12 abas

| Aba | Função | Você preenche? |
|---|---|---|
| 📊 **01 Dashboard** | **Aporte**, plano de compras, gráficos e controle de risco | Só o aporte |
| 🎯 **02 Macro Alocação** | % objetivo por classe, BUY/HOLD e distribuição do aporte | % Objetivo |
| 🇧🇷 **03 Ações BR** · **04 FIIs** | Ações e fundos imobiliários brasileiros | Sim |
| 🌎 **05 Stocks** · **06 REITs** | Ações, ETFs e REITs do exterior | Sim |
| 🏦 **07 Renda Fixa** | Tesouro, CDB, LCI/LCA etc. | Sim |
| 🪙 **08 Criptomoedas** | BTC, ETH, SOL e outras | Sim |
| 🏠 **09 Ativos Ilíquidos** | Imóveis, terrenos, participações | Sim |
| ⚙️ **10 Configurações** | Custos, câmbio e regras de compra por classe | Sim |
| 📚 **11 Auxiliar** | Listas (setores é editável) e tabelas dos gráficos | Só os setores |
| 🗄️ **12 Base de Dados** | Tabela consolidada de todas as posições | Não |

> 🎨 **Células azuis** = você preenche. **Células escuras** = fórmulas (não edite).

## 🛠️ Configuração inicial (uma única vez)

1. ⚙️ **Configurações**: custos (corretagem, IOF, spread), compra mínima e limites.
2. 💱 **Configurações → Câmbio**: confira o par Yahoo e preencha a **Cotação Manual** do dólar como reserva.
3. 🧩 **Configurações → Regras por classe**: fração, casas decimais e lote de cada classe.
4. 🎯 **Macro Alocação**: o % objetivo de cada classe. O card **SOMA DOS OBJETIVOS** deve ficar verde com **100%**.
5. 🧾 **Abas das classes**: cadastre seus ativos.

### 🧾 Colunas que você preenche nas abas de ativos

| Coluna | O que digitar | Exemplo |
|---|---|---|
| **Ticker** | Código, sem sufixo (`.SA` é automático) | `HGLG11` |
| **Nome** | Livre | CSHG Logística |
| **Setor** | Escolha na lista | FII - Logística |
| **Moeda** | Vazio = moeda padrão da classe | *(vazio)* |
| **Quantidade** ⭐ | O que você tem hoje. **É o campo que mais muda** | `8` |
| **Objetivo** | % do ativo **dentro da classe** (soma 100%) | `15%` |
| **Cotação Manual** | Opcional, mas **recomendado**: plano B se a automática falhar | `154,90` |

**Renda Fixa e Ilíquidos** não têm quantidade nem cotação: você informa o **Valor Atual** e o atualiza quando quiser.

## 🖼️ Como é por dentro

**Macro Alocação:**

![Macro Alocação](../docs/img/macro-alocacao.png)

**Aba de ativos:**

![Aba de ativos](../docs/img/aba-ativos-fiis.png)

## 📊 O que o Dashboard mostra

- 💼 **Patrimônio** total, Brasil, Exterior e Alternativos.
- 🛒 **Compra efetiva do mês** e **sobra do aporte**.
- 🎯 **Classes a aportar** e **ordens de compra**.
- 🧱 **Maior posição**, **ativos efetivos** (1/HHI) e **setor mais concentrado**.
- ⚠️ **Cotações sem preço** (deve ser 0).
- 📈 **6 gráficos**: alocação por classe, Brasil × Exterior × Alternativos, top 10 ativos, **atual × objetivo por classe**, concentração por setor e exposição por moeda.
- 🛡️ **Controle de risco** com alertas de concentração por ativo e por setor.

## 🧠 Como o Rebalance Score decide

```text
Déficit  = máximo(0 ; Objetivo × (Patrimônio + Aporte) − Valor Atual)
Score    = Déficit do item ÷ soma dos déficits dos itens elegíveis
Aporte do item = Aporte × Score
```

| Filtro (em Configurações) | Efeito |
|---|---|
| Valor mínimo de diferença | Itens muito próximos do objetivo ficam "Alinhados" (HOLD) |
| Máx. classes a aportar | Só as N classes mais defasadas recebem aporte |
| Máx. ativos por classe | Só os N ativos mais defasados de cada classe são comprados |
| Compra mínima | Ordens menores que o valor mínimo são descartadas |
| Lote e fração | Respeita as regras de cada classe |
| **Reaproveitamento da sobra** | O que não coube vai para o ativo de maior prioridade que ainda puder ser comprado |

> 💡 Aportes pequenos com muitos ativos geram ordens menores que uma cota. Reduza **Máx. ativos por classe** (3, ou até 1) para concentrar o dinheiro nos mais defasados.

## 🔌 Cotações

- **Automáticas** via Yahoo Finance (CoinGecko opcional para cripto), usando a função `WEBSERVICE`.
- Funcionam no **Excel para Windows** e no **LibreOffice**. No **Excel para Mac e Web**, use o modo **Manual**.
- Para atualizar: **Ctrl + Alt + F9** (Excel) ou **Ctrl + Shift + F9** (LibreOffice).
- Coluna **Fonte**: `Auto` ✅ · `Manual` · `Sem cotação` ⚠️ · `Sem câmbio` ⚠️.

> ⚠️ Sem preço médio na planilha, um ativo **sem cotação vale zero**. Por isso o card **COTAÇÕES SEM PREÇO** do Dashboard existe: ele deve mostrar **0**.

## ⚠️ Limitações

- 🌐 Cotações dependem de Yahoo Finance e CoinGecko (podem limitar ou falhar).
- 🧾 IOF (0,38%) e spread (1,5%) padrão vêm da planilha original. **Confirme com sua corretora.**
- 🏦 Renda Fixa e Ilíquidos: atualização manual.
- 🧮 O que sobra do arredondamento **não é redistribuído entre classes**: aparece como **Sobra** e fica para o próximo aporte.
- 📏 Capacidade: **920 posições** (200 em Ações, FIIs e Stocks; 100 em REITs e Renda Fixa; 60 em Cripto e Ilíquidos).

## ❓ FAQ

<details>
<summary><b>Por que não tem preço médio nem dividendos?</b></summary>

De propósito. Esta versão tem **um único trabalho**: o plano de compras. Preço médio, dividendos, rentabilidade e patrimônio ficam no seu app de acompanhamento. Se quiser tudo numa planilha só, use a [Versão Premium](../Vers%C3%A3o%20PREMIUM).
</details>

<details>
<summary><b>Cliquei em Excluir linha e deu erro. E agora?</b></summary>

Desfaça com **Ctrl + Z** na hora. Para remover um ativo, selecione só as **células azuis** da linha e aperte **Delete**. Nunca exclua linhas ou colunas.
</details>

<details>
<summary><b>O card "Soma dos objetivos" está amarelo.</b></summary>

Os percentuais não somam 100%. Ajuste os objetivos (na Macro Alocação, para as classes; na aba da classe, para os ativos).
</details>

<details>
<summary><b>Aparece BUY, mas a quantidade sugerida é 0.</b></summary>

O valor destinado ao ativo é menor que o preço de uma cota/lote ou menor que a compra mínima. Aumente o aporte, reduza o **Máx. ativos por classe** ou deixe a sobra para o mês seguinte. Se a classe de Ações estiver com **Usa lote = Sim**, desligue para aportes pequenos.
</details>

<details>
<summary><b>Posso usar sem internet?</b></summary>

Pode. Escolha **Modo de cotações = Manual** em Configurações e preencha a **Cotação Manual** dos ativos.
</details>

---

⚖️ *Material informativo e educacional, sem recomendação de investimento. Dados da DEMO são fictícios. Planilhas fornecidas sem garantias.*
