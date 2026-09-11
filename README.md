# Cubo_Gelatinoso

## Descrição
Notebook desenvolvido para a atividade "Cubo Gelatinoso", com o objetivo de estudar o desempenho do algoritmo de k vizinhos mais próximos (k-NN) em uma tarefa de classificação binária, testando diferentes combinações de hiperparâmetros. Dado um livro que esteve entre os mais vendidos da Amazon, o modelo prevê se ele é um livro de ficção ou não-ficção, a partir de atributos como nota do usuário, número de avaliações, preço, ano e autor.

## Dataset
[Amazon Top 50 Bestselling Books 2009-2019](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019), 550 registros de livros reais que estiveram entre os mais vendidos da Amazon nesse período.

| Coluna | Tipo	| Descrição |
| `Name` |	texto |	Título do livro (descartado — identificador único) |
| `Author` |	categórico |	Autor do livro |
| `User Rating` |	numérico |	Nota média do usuário |
| `Reviews` |	numérico |	Número de avaliações |
| `Price` |	numérico |	Preço do livro |
| `Year`	| numérico	| Ano em que esteve na lista de mais vendidos |
| `Genre` |	categórico (target)	| `Fiction` ou `Non Fiction` |

## Estrutura do notebook
1. Introdução
2. Carregamento dos dados
3. Tratamento dos dados
4. Divisão treino e teste
5. Modelo baseline
6. Normalização dos atributos
7. Testando diferentes tipos de hiperparâmetros
8. Modelo Final
9. Conclusão

## Resultados
| Modelo | 	Acurácia no teste |
| Baseline (`DummyClassifier`) |	60,00% |
| k-NN (`n_neighbors=3`, `p=1`) |	82,73% |

## Como rodar
```bash
pip install pandas scikit-learn seaborn jupyter
jupyter notebook cubo_gelatinoso_knn.ipynb
```
O notebook carrega o dataset diretamente de uma cópia pública no GitHub, então não é necessário baixar nenhum arquivo manualmente.

## Tecnologias
- Python
- pandas
- scikit-learn
- seaborn

## Nota sobre uso de IA
O código deste notebook foi implementado com apoio do assistente de IA Claude (Anthropic), utilizado como ferramenta de apoio para a escrita e explicação do código.

## Professor

### Daniel Roberto Cassar

Doutorado: Ciência e Engenharia de Materiais (UFSCar) – Pós-doutorado: UFSCar. Área de atuação: Informática de materiais.

## Autoria 

### Leticia Campos da Silva

Técnica em Edificações e estudante de Ciência e Tecnologia na Ilum Escola de Ciência.

## Refências

SOOTERSAALU. **Amazon Top 50 Bestselling Books 2009-2019**. Kaggle, 2020. Disponível em: https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019. Acesso em: 10 set. 2026.

CASSAR, Daniel R. **Tratamento de dados com pandas: ATP-203 1.1**, Aprendizado de Máquina. [Ilum Escola de Ciência], [2026]. 1 notebook Jupyter. Notas de aula.

CASSAR, Daniel R. **Aprendizado de máquina, k-NN e métricas: ATP-203 2.1**, Aprendizado de Máquina. [Ilum Escola de Ciência], [2026]. 1 notebook Jupyter. Notas de aula.

CASSAR, Daniel R. **Divisão de dados em treino e teste: ATP-203 2.2**, Aprendizado de Máquina. [Ilum Escola de Ciência], [2026]. 1 notebook Jupyter. Notas de aula.

CASSAR, Daniel R. **Modelo linear e baseline: ATP-203 3.0**, Aprendizado de Máquina. [Ilum Escola de Ciência], [2026]. 1 notebook Jupyter. Notas de aula.

CASSAR, Daniel R. **Classificação binária: ATP-203 5.0**, Aprendizado de Máquina. [Ilum Escola de Ciência], [2026]. 1 notebook Jupyter. Notas de aula.

