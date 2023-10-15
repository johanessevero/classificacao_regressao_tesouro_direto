# Modelos treinados para classificação e regressão de taxa de rendimento de títulos do tesouro direto

Modelos treinados para classificação e regressão de taxa de rendimento na venda em curto prazo de títulos do tesouro direto com base em indicadores calculados.

- Consistiu das seguintes etapas:
  - Extração os dados dos arquivos de preços e taxas:
    - LTN_*ano*.xls',
    - NTN-C_*ano*.xls',
    - NTN-B_*ano*.xls',
    - NTN-F_*ano*.xls',
    - LFT_*ano*.xls',
    - NTN-B_Principal_*ano*.xls'
    - Disponíveis em: https://www.tesourodireto.com.br/titulos/historico-de-precos-e-taxas.htm
  - Criação da base de dados no sqlite:
    -  <img src = 'mr_historico_titulo.png'>
    ![image](https://github.com/johanessevero/classificacao_regressao_tesouro_direto/assets/22893251/2f1bbdb1-de5f-4763-bcd5-74dc638b54c3)
    - Os dados sobre títulos do Tesouro Direto brasileiro fornecem informações específicas sobre um título:
      - data: refere-se à data em que os valores foram registrados ou atualizados.
      - taxa_compra: indica a taxa de compra associada ao título na data específica.
      - taxa_venda: representa a taxa de venda associada ao título na data específica.
      - preco_compra: refere-se ao preço de compra do título nessa data específica.
      - preco_venda: indica o preço de venda do título na data em questão.
      - preco_base: representa o preço base do título.
      - nome_titulo: corresponde ao nome ou descrição do título do Tesouro Direto. Essa informação fornece detalhes sobre o tipo de título e seu vencimento.
  - Montagem da base de treino e teste com os indicadores calculados para treinamento do modelo de regressão e classificação;
  - Treinamento do modelo e ajuste dos hiperparâmetros;
  - Avaliação do modelo.
 
- *Por questões de simplicidade nesse repositório somente foi adicionado os notebooks com a avaliação do modelo nos dados de teste.


