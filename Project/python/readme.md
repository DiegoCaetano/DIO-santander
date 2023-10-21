Santander Dev Week 2023 (ETL com Python)


Contexto: Você é um cientista de dados e recebeu a tarefa de identificar os municipos que não entregaram a Matriz de Saldos Contábeis, ou simplesmente MSC ao Site da https://siconfi.tesouro.gov.br/.

Condições do Problema:

Você recebeu uma planilha simples, em formato CSV ('SDW2023.csv'), com uma lista de códigos de IBGE do minicipo:

IBGE_Id
2507507
2500106
2700102

Seu trabalho é consumir o endpoint curl -X 'GET'
'https://apidatalake.tesouro.gov.br/ords/siconfi/tt/extrato_entregas?id_ente={IBGE_ID}&an_referencia={ano_referencia}' (API da Tesouro.gov.br) para obter os dados de cada municipo.
Depois de obter os dados dos Municipios, ira verificar qual a instituição esta faltando a entregar a MSC e notifica-la.
