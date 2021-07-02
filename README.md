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
##### Either
1. login to scc account and download script
2. In your terminal, `module load python3`
3. run `python3 -m venv /path/to/new/virtual/environment`
4. run `. bin/activate`
5. `pip install tensorflow==2.3.1`
6. `pip install git+https://github.com/google-research/bigbird.git`
7. restart ssh client
8. run `python nlp_sentiment_analysis.py`, or optionally run `qsub` with provided script

##### Or (much easier)
1. Open [our script](https://github.com/esbirol/CS523-summer2021/blob/main/CS523_BigBird_IMDB.ipynb) in Google Colab
2. Run every cell 
3. Voila! You have trained and evaluated your model on the sample data



### Data_Plot.ipynb
1. Save your accuracy values and iteration steps in an excel file
2. replace `example.xlsx` with your file name in `df = pd.read_excel(io.BytesIO(uploaded['example.xlsx']))`
3. replace `example.xlsx` with your file name in `data = pd.read_excel('example.xlsx')`

## Example Results

### Pretraining
![Training](https://github.com/esbirol/CS523-summer2021/blob/main/pretraining.png)

### Evaluation
![Evaluation](https://github.com/esbirol/CS523-summer2021/blob/main/eval.png)

### Accuracy Graph
<img src="https://github.com/esbirol/CS523-summer2021/blob/main/accuracy.png" width="550" height="400">

We have run 16000 iterations on our model.
> #### Discussion
> Our accuracy graph has reached upto 6% accuracy with only 16000 iterations. Our project was based on a model that had 1000000 iterations; however, replicating the 1000000 iterations would take a couple of days. Because of time constraints for the project, we ran our model on a smaller dataset and got our results with 16000 iterations. We see that with 16000 iterations, we have achieved around 6% accuracy. If we could replicate the 1000000 iterations, we foresee that we would get around 25% accuracy.


## References
https://arxiv.org/abs/2007.14062

`Big Bird: Transformers for Longer Sequences Manzil Zaheer, Guru Guruganesh, Avinava Dubey, Joshua Ainslie, Chris Alberti, Santiago Ontanon, Philip Pham, Anirudh Ravula, Qifan Wang, Li Yang, Amr Ahmed`

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5408915/

`KAT: a K-mer analysis toolkit to quality control NGS datasets and genome assemblies Daniel Mapleson, Gonzalo Garcia Accinelli, George Kettleborough, Jonathan Wright, and Bernardo J Clavijo` 

https://www.biorxiv.org/content/10.1101/2020.05.05.079327v2

`Optimizing experimental design for genome sequencing and assembly with Oxford Nanopore Technologies John M. Sutton, Joshua D. Millwood, A. Case McCormack, Janna L. Fierst `
