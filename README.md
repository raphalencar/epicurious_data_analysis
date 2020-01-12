# Epicurious Data Analysis
Análise realizada sobre os dados do arquivo [receitas.json]. Os dados são referentes as receitas disponíveis em [Epicurious](https://www.epicurious.com/)

**Autor:** Raphael Brito Alencar

**Linguagem:** Python 3.7

### Descrição dos dados
Nos dados estão presentes 20130 registros, cada um disposto em 11 colunas, que são:

**directions:**  Forma de preparo                (object)<br>
**fat:**         Índice de gordura               (float64)<br>
**date:**        Data de cadastro                (datetime64)<br>
**categories:**  Categorias associadas a receita (object)<br>
**calories:**    Índice de calorias              (float64)<br>
**desc:**        Descrição da receita            (object)<br>
**protein:**     Índice de proteína              (float64)<br>
**rating:**      Avaliação da receita            (float64)<br>
**title:**       Título da receita               (object)<br>
**ingredients:** Ingredientes usados na receita  (object)<br>
**sodium:**      Índice de sódio                 (float64)<br>

### Exercício sugerido e realizado na análise
1) A que categorias pertencem as comidas mais calóricas? 
2) Quais os top 10 ingredientes contidos nas receitas mais calóricas?
3) Se você tivesse que recomendar 3 receitas baseando-se nos dados, quais seriam?
4) Alguma característica presente nos dados determina a alta nota de uma receita?
5) Considerando-se as categorias das top 100 receitas em avaliação, quantas receitas há atualmente no site https://www.epicurious.com para cada categoria
6) Criar um modelo para sugerir categorias para novas receitas, baseado nos dados

### Build e execução

```
# Configurar ambiente com conda
conda create -n myenv python=3.6
conda install --yes --file requirements.txt

# Configurar ambiente com pip
python3 -m venv venv
. ./venv/bin/activate
pip3 install -r requirements.txt

# Inicializar o Jupyter Notebook
docker run -it --rm -p 8888:8888 -p 4040:4040 -v $PWD:/home/jovyan/workspace jupyter/all-spark-notebook
```
