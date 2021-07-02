# Introduction to Deep Sequencing Analysis with BigBird NLP

### Final Project for CS523 Summer 2021

Our work was adapted from [Big Bird: Transformers for Longer Sequences](https://arxiv.org/abs/2007.14062). The GitHub link of the BigBird can be found [here](https://github.com/google-research/bigbird). The specific script used in our project can be found [here](https://github.com/google-research/bigbird/blob/master/bigbird/classifier/imdb.ipynb)

Our Team:

 > Adam McCormack <acmccorm@bu.edu>
 > 
 > Ece Sureyya Birol <esbirol@bu.edu>

[Our Presentation Slides can be found here](https://drive.google.com/file/d/1OCpqMj7tmB-o5oDo5Vbq7QsL62_J3LnI/view?usp=sharing)

## Running Our Script

### CS523_BigBird_IMDB.ipynb

### Data_Plot.ipynb
- Save your accuracy values and iteration steps in an excel file
- replace `example.xlsx` with your file name in `df = pd.read_excel(io.BytesIO(uploaded['example.xlsx']))`
- replace `example.xlsx` with your file name in `data = pd.read_excel('example.xlsx')`

## Example Results

### Pretraining
![Training](https://github.com/esbirol/CS523-summer2021/blob/main/pretraining.png)

### Evaluation
![Evaluation](https://github.com/esbirol/CS523-summer2021/blob/main/eval.png)

### Accuracy Graph
<img src="https://github.com/esbirol/CS523-summer2021/blob/main/accuracy.png" width="550" height="400">

We have run 16000 iterations on our model.


## References
1. [Big Bird: Transformers for Longer Sequences](https://arxiv.org/abs/2007.14062)
2. [KAT: a K-mer analysis toolkit to quality control NGS datasets and genome assemblies](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5408915/)
3. [Optimizing experimental design for genome sequencing and assembly with Oxford Nanopore Technologies](https://www.biorxiv.org/content/10.1101/2020.05.05.079327v2)
