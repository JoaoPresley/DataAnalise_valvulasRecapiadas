# 📊 Data Analysis: Gestão de Ativos MSGAS
### Análise de Válvulas para Elevação de Cota e Instalação de Laje

---

## 📖 Resumo do Projeto
Este projeto automatiza a identificação e o status de manutenção das válvulas da rede MSGAS, cruzando dados de inspeção *in loco* com o histórico de ordens de serviço (OS). O objetivo principal é otimizar a gestão de ativos, eliminando a necessidade de verificações manuais repetitivas e garantindo a integridade dos dados cadastrais.

## 💡 Storytelling: Do Manual ao Automatizado
A demanda surgiu da necessidade de filtrar válvulas que foram recapeadas (cobertas pelo asfalto). A abordagem inicial previa uma conferência manual, válvula por válvula — um trabalho exaustivo, demorado e suscetível a erros humanos.

**A Mudança de Paradigma:**
Em vez da conferência física imediata, aplicamos **Data Science**. Utilizando a biblioteca **Pandas** e lógica em Python, realizamos o cruzamento de três bases de dados distintas. O que levaria dias de análise manual foi resolvido com scripts que garantem precisão, escalabilidade e uma economia significativa de horas de trabalho.

## 🛠️ Metodologia e Escopo
O projeto processa os dados para classificar as válvulas em quatro categorias críticas:

1. **Válvulas que precisam abrir OS:** Identificadas com necessidade de intervenção, mas sem ordem de serviço ativa no sistema.
2. **Válvulas que precisam atualizar Status:** Divergência entre o apontamento de campo e o status atual no sistema.
3. **Pendentes de Elevação (Fluxo Padrão):** Válvulas com OS ativa para elevar/instalar laje (casos de complexidade comum).
4. **Pendentes de Elevação (Casos "Bucha"):** Válvulas com OS ativa onde o serviço exige maior complexidade técnica.

> **O que são "Buchas"?**
> Termo operacional para válvulas onde houve tentativa de execução, mas foram encontrados impedimentos técnicos (redes profundas, interferências externas) que exigem um planejamento de engenharia mais complexo que o usual.

## 🚀 Tecnologias Utilizadas
* **Python 3.x**
* **Pandas:** Manipulação de DataFrames, Merges (Joins) e filtros temporais.
* **Jupyter Notebook:** Ambiente de desenvolvimento e documentação.

## 📂 Visualização dos Resultados
Por questões de confidencialidade e segurança da informação (políticas internas da empresa), os arquivos `.csv` originais não foram disponibilizados neste repositório.

No entanto, toda a lógica de tratamento, cruzamento de dados e filtros pode ser conferida no arquivo:
👉 `main.ipynb` (os outputs foram preservados para demonstrar a estrutura final dos dados gerados).

---
*Desenvolvido para otimização de processos de manutenção e engenharia.*
