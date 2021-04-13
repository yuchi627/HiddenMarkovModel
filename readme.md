# Genome Informatics (基因體資訊) 2020. Homework assignment
## Data
Genome Informatics (基因體資訊) 2020. Homework assignment 20200408.
Download chromosome 6 From [Human Genome Resources at NCBI](https://www.ncbi.nlm.nih.gov/genome/guide/human/), select link GRCh38, Fasta.

Extract entry NC_000006.12 Homo sapiens chromosome 6, GRCh38.p13 Primary Assembly.

Extract bases [100,000–1,099,999]; starting with ttggtaccat and ending in TAATTGCAGT. Denote this as S. (標作S).

(In 2020, we used a smaller training region: bases [100,000–199,999]; starting with ttggtaccat and ending in CTTTGCCTG).
For simplicity map all letters to lower case; i.e. A-->a, C-->c, etc.

## Model
### Markov models of order0, 1, 2
Write a program (in C or whatever) implementing (plain) Markov models of order 0,1 and 2; for generating DNA sequences. Fit the parameters of these three models to S and compute the log base 2 probability of each of them generating S (given that they generate a sequence of that length).
### Hidden Markov model
Write a program (in C or whatever) implementing a hidden Markov model to generate sequences.
Because this is an exercise for learning, please implement the models yourself (do not use any software packages for Markov or hidden Markov models).
Compute the log base 2 probability of your model generating S (given that it generates some sequence that length).
You may hand tune your parameters or use a learning algorithm (extra credit for implementing Baum-Welch or similar learning algorithm yourself), to make the probability of S as large as possible; however you may not use more than 30 free parameters (for comparison a 1st order Markov model has 16 parameters (P[x|y] for x,y ∈ {a,c,g,t}, but 4 "sum-to-one" constraints, yielding 12 free parameters.
See if your parameters can be tuned to give a higher probability than the plain Markov models.

To keep the models general, models are not allowed to emit more than 3 bases in one step (in particular the model cannot simply emit S in one step!).
### Test
Compute the most likely state sequence that the model would traverse when emitting S.

After designing your model and fitting its parameters to S; compute the probabilities that they would generate:

The 100Mb section of chromosome 6 from [1,100,000–2,099,999]; starting with GCTCTGCCTT and ending in CTTGGAGAAC
A 100Mb section of another chromosome (state the section used)

