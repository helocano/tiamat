<img width="2480" height="254" alt="Cabecalho 3" src="https://github.com/user-attachments/assets/14f721de-0601-4f8d-9782-06dc02ec0d44" />
<h1>Tiamat</h1> 

Heloísa Fernandes Cano - T26

O seguinte projeto consiste na segunda entrega da disciplina de Aprendizado de Máquina, ministrada pelo professor doutor Daniel Roberto Casar, durante o 2º semestre de 2026 no curso de Bacharelado em Ciência e Tecnologia da Ilum - Escola de Ciência.

Arquivos:
- MainTiamat_HeloisaCano.ipynb: Contém tudo o que foi desenvolvido no trabalho
- AnaliseDados_Tiamat.ipynb: Apenas a parte de análise e limpeza dos dados do dataset
- arquivos_dados:
  - AVONET_Raw_Data: Arquivo 'cru'
  - dados_limpos.csv: Arquivo limpo e filtrado, como utilizado nos modelos desenvolvidos

<h2>Enunciado</h2>
<h3>Objetivo</h3>
Escolha um conjunto de dados que siga as considerações abaixo e compare o desempenho de pelo menos 3 algoritmos/pipelines de aprendizado de máquina (sem contar o baseline). É necessário testar pelo menos 100 conjuntos diferentes de hiperparâmetros para cada algoritmo/pipeline escolhido utilizando o optuna (sem contar o modelo baseline). A entrega deverá ser realizada em repositório tipo git com README que guia o leitor sobre o que é e como navegar no repositório. Este é o projeto final da disciplina de Aprendizado de Máquina, logo é esperado que esta seja uma entrega científica que fundamenta bem o problema, trazendo resultados e discutindo eles. Se você optar por fazer scripts de Python (não é necessário, porém alguns estudantes fazem essa opção), lembre‑se que ainda é necessário um relatório científico para acompanhar a entrega (seja em pdf ou notebook Jupyter, jamais em arquivo de Word).

<h3>Considerações</h3>
O conjunto de dados deve ter as seguintes características:
- Pelo menos 10 atributos
- Pelo menos 1 target (não há necessidade de mais que 1 target e pode ser um target categórico ou numérico, a sua escolha)
- Pelo menos 300 exemplos
- Não pode ser o conjunto de dados utilizado na entrega do Cubo Gelatinoso
- Não utilizar datasets sintéticos ou didáticos como o iris, pinguins, titanic, vinhos, diamantes, gorjetas, etc. (alguns exemplos destes datasets didáticos podem ser conferidos aqui)

<h3>Expectativas</h3>
É esperado que o trabalho siga as boas práticas apresentadas na disciplina, apresente resultados de forma gráfica, use seções bem nomeadas e bem divididas no notebook de Jupyter e encerre a entrega com uma seção chamada “Conclusões e principais aprendizados”. Não é necessário utilizar todas as estratégias e ferramentas discutidas em sala, porém, por se tratar de um projeto final da disciplina, é esperado que a entrega seja suficientemente abrangente e detalhada, demonstrando o entendimento e a aplicação prática dos conceitos discutidos ao longo da disciplina. Pode utilizar estratégias e ferramentas não apresentadas durante a disciplina caso tenha interesse e faça sentido dentro do escopo do projeto (desde que saiba explicar como elas funcionam). É recomendado não utilizar dados sequencias ou espacialmente autocorrelacionados para esta atividade (séries temporais ou dados que contenham latitude e longitude, por exemplo) pois eles exigem um tratamento de dados que ainda não foi apresentado no curso da Ilum. O trabalho deve ter uma seção chamada “Descrição do uso de IA neste trabalho” detalhando como foi a interação com ferramentas de IA para a construção dos textos e códigos.

<h3>Pontuação Base</h3>
Pontuação base: 6 (válida apenas caso o objetivo tenha sido realizado)

Descontos usuais da pontuação base:
- Alguma expectativa não foi atingida
- Não realizou uma análise exploratória dos dados
- Trabalho não seguiu boas práticas apresentadas na disciplina. Lembre‑se de revisar o material apresentado e suas anotações durante a aula
- Lembre‑se que treinar um modelo baseline é uma boa prática apresentada na disciplina
- Dados não foram normalizados em situações onde era esperado que fossem normalizados
- Trabalho não apresentou resultados de forma gráfica
- Entrega não apresenta os conceitos de forma didática, guiando o leitor a aprender o que está sendo apresentado
- Não guiou o leitor na entrega
- Não interpretou e discutiu os resultados
- Gráfico sem legenda em um ou mais eixos
- Código que acusa erro ao rodar na ordem de cima para baixo
- Entrega sem referências
- Uso incorreto ou omisso de citações (incluindo falta de citação sobre uso de IA)
- Não soube explicar sobre estratégias e códigos utilizados na entrega
- Respostas incorretas às perguntas realizadas pelo professor durante o momento avaliativo
- Respostas incorretas às perguntas realizadas pelo Perguntador 2000™ durante o momento avaliativo
- Repositório git tem arquivos desnecessários (caches, arquivos temporários do Jupyter, etc.). Sugestão: escolha o arquivo .gitignore adequado quando criar seu repositório
- Repositório git não tem o nome do(s) autor(es) e sua instituição
- Repositório git não guia o leitor sobre os arquivos do repositório
- Repositório git não guia o leitor sobre o trabalho realizado (não precisa escrever um livro, mas pelo menos um parágrafo indicando sobre do que se trata o repositório é necessário)
- Não justificou para o leitor a escolha dos valores/intervalos dos hiperparâmetros de cada algoritmo/pipeline
- A escolha dos hiperparâmetros otimizados pelo optuna ficou muito rasa (isto é, hiperparâmetros muito importantes não foram considerados)
- Houve vazamento de dados no processo realizado no trabalho, como por exemplo:
  - Normalizar os dados antes de dividir em treino e teste
  - Usar informação do conjunto de teste para escolher o melhor modelo durante a otimização de hiperparâmetros
- Atraso na entrega do trabalho no Teams

<h3>Pontuação complementar</h3>
Pontuação complementar: 4 (cada item abaixo pode valer até no máximo 1 ponto, exceto quando escrito o contrário)
- Comparou pelo menos 5 algoritmos/pipelines diferentes (sem contar o baseline)
- Utilizou de forma correta validação cruzada para comparar diferentes algoritmos/pipelines
Realizou redução de dimensionalidade ou seleção de atributos nos dados, permitindo que o optuna controlasse esse processo (isto é, otimizando os hiperparâmetros destas estratégias) (nota: é necessário ter pelo menos 20 atributos para optar por esta estratégia)
- Realizou a otimização de hiperparâmetros no HPC (necessário que os scripts utilizados, arquivo do job.sh do slurm e output do slurm façam parte do repositório)
- Usou ferramenta de explicação de modelos (gráfico de dependência parcial, permutation importance, LIME ou SHAP) para extrair informações sobre o(s) modelo(s) selecionado(s), com devida discussão sobre o resultado e sobre como a ferramenta de explicação funciona
- Fez alguma estratégia suficientemente interessante (e bem discutida na entrega) que não está contemplada nos demais itens
- Estudante (ou dupla, se for o caso) criou um nome, brasão e frase de efeito para representar sua casa perante ao Rei Milu Iluminarius MLVI (vale 0,2 pontos se fizer o brasão sem usar IA ou 0,1 pontos se fizer o brasão usando IA)

<h3>Outras observações</h3>
Motivação e aprendizado: A execução de um projeto de Aprendizado de Máquina envolve não apenas conhecimento mas muito planejamento. É executando um projeto que conectamos prática e teoria e exercitamos nossa habilidade de desenvolver um estudo sequencial que faça sentido.

Sugestão de uso de IA nesta tarefa: Um bom uso de IA pode ser para encontrar conjuntos de dados de seu interesse. Fora isso, debater com a IA sobre quais pontos complementares fazer, ponderando aprendizado e interesse, também é uma boa estratégia.

Lore: O que é uma boa aventura sem um ou dois dragões, não é mesmo? Melhor ainda, que tal um dragão com múltiplas cabeças? Vostrasirus Baba, em uma de suas visões premonitórias, jura de pé junto que um dragão lendário irá atacar o reino de Lumi neste semestre. Vossa Iluminância, Rei Milu Iluminarius MLVI, está absurdamente inquieto e pede para que todos os membros das guildas se preparem para este ataque iminente. A Patrulha já está de prontidão!
