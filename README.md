# Data Analise
### Resumo do projeto
_Analise de válvulas da MSGAS que precisam de elevação de cota_

### History Telling
Foi solicitada uma demanda pela chefia para filtrar as válvulas recapiadas.

A primeira solução foi passar _in loco_ para verificar válvula por válvula para ver se realmente estavam recapidas ou posivelmente foi um apontamento por engano

* __Solução__

      Ao invés de ir _in loco_ para verificar válvula por válvula foi realizado o cruzamento de dados e a analise deles.
      A empresa possui um sistema que consegue exibir tabelas, com as quais podemos manipular e analisar cada uma.
      Poderia-se analisar tabela por tabela, linha por linha, com certeza isso seria solicitado para o estagiário, rssrsrsr.
      Porém com os conhecimentos de analise de dados em pouco tempo conseguimos analisa todas essas 3 tabelas com multidões de dados utilizando o PANDAS!! (e um pouco de racicionio Python)
  
### Metodologia
Para realizar essa analise foi definido o escopo para cumprir esses requisitos:
1. Válvulas que precisa abrir OS
2. Válvulas que precisa atualizar os Status
3. Válvulas que estão pendentes para elevar/instalar laje que já tem OS e __não são bucha__
4. Válvulas que estão pendentes para elevar/instalar laje que já tem OS e __são bucha__

        OBS: O que são "bucha"??
        São válvulas que já tentaram elevar ou instalar laje porém o serviço era mais complexo que o usual
   
Desses somente o 4 não seria possivel extrair utilizando dados das planilhas fornecidas pelo sistema.
O restante você pode conferir no arquivo ```main.ipynb```!

---
Não foi disponibilizado os .csv pois são arquivos pessoais da empresa, porém no arquivo ```main.ipynb``` está com os outputs que pode ser vizualizado uma prévia da planilha
  
