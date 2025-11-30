Lógica e Estruturas de Dados
O sistema utiliza estruturas de dados fundamentais para gerenciar informações elétricas e regras de segurança:

Lista de Listas (circuitos): Armazena todos os dados medidos de cada circuito (Nome, Tipo, Tensão, Corrente, Fator de Potência, etc.).

Dicionário (limites): Define as regras de conformidade e os limites máximos e mínimos para cada tipo de carga (motor, iluminação, etc.).

Análise de Conformidade
O sistema verifica se o circuito está em conformidade. O circuito é classificado como NÃO CONFORME se qualquer uma das seguintes regras for violada:

Tensão (V): Estiver fora da faixa de mais ou menos 10% (+/- 10%) da Tensão Nominal.

Corrente (I): Exceder o limite máximo permitido (I_Max) para o tipo de carga.

Fator de Potência (FP): For inferior ao mínimo exigido (FP_Min).

Módulo Extra: Consumo de Energia
O módulo extra estima o gasto energético e o custo diário dos circuitos, usando as medições e o tempo de uso fornecido pelo usuário.

Cálculos Chave (Fórmulas Copiáveis):

Potência Ativa (P em kW): P = (V * I * FP) / 1000

Energia Consumida (E em kWh): E = P (kW) * Tempo (h)

Custo Diário (R$): Custo = E (kWh) * Tarifa (R$/kWh)

Menu e Relatórios
O programa é operado por um menu de console intuitivo.

Opção 1 e 2: Gerencia as entradas de dados e atualiza as medições elétricas.

Opção 3 (Análise Completa): Executa a análise de conformidade e o Módulo Extra de Consumo.

Opção 5 (Salvar e Relatório): Cumpre o requisito de manipulação de Arquivos, salvando dados no circuitos.txt e gerando o relatorio_nao_conforme.txt com a lista dos circuitos com problemas.

Equipe e Tecnologia
Este projeto foi desenvolvido por:

João Gustavo Rodrigues de Almeida
Leonardo Pasturchak de Paula
Luis Gabriel Pereira de Barros
Pedro de Sousa Alves

Tecnologias: Python 3.x, Listas de Listas, Dicionários, Manipulação de Arquivos.
