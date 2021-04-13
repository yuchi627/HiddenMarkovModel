# Genome Informatics (基因體資訊) 2020. Homework assignment

Download chromosome 6 From [Human Genome Resources at NCBI](https://www.ncbi.nlm.nih.gov/genome/guide/human/), select link GRCh38, Fasta.

A 100Mb section of another chromosome: NT_187361.1 Homo sapiens chromosome 1 unlocalized genomic scaffold, GRCh38.p13 Primary Assembly HSCHR1_CTG1_UNLOCALIZED [100,000–199,999]

## Markov models of order 0
> Calculate each nucleobase(a,t,c,g) probability of occurrence.

the log base 2 probability of order 0 Markov model generating bases [100,000–1,099,999]: -1987487.013403616
the log base 2 probability of order 0 Markov model generating bases [1,100,000–2,099,999]: -1986855.279184155
the log base 2 probability of order 0 Markov model generating >NT_187361.1 Homo sapiens chromosome 1 unlocalized genomic scaffold, GRCh38.p13 Primary Assembly HSCHR1_CTG1_UNLOCALIZED bases [100,000–1,099,999]: -148850.35756241082

## Markov models of order 1
> Calculate each nucleobase(a,t,c,g) probability of occurrence after order1.

the log base 2 probability of order 1 Markov model generating bases [100,000–1,099,999]: -3932505.4760067393
the log base 2 probability of order 1 Markov model generating bases [1,100,000–2,099,999]: -3932053.910575677
the log base 2 probability of order 1 Markov model generating >NT_187361.1 Homo sapiens chromosome 1 unlocalized genomic scaffold, GRCh38.p13 Primary Assembly HSCHR1_CTG1_UNLOCALIZED bases [100,000–1,099,999]: -294763.4161986726

## Markov models of order 2
> Calculate each nucleobase(a,t,c,g) probability of occurrence after order2.

the log base 2 probability of order 2 Markov model generating bases [100,000–1,099,999]: -5865356.202508941
the log base 2 probability of order 2 Markov model generating bases [1,100,000–2,099,999]: -5865131.653288243
the log base 2 probability of order 2 Markov model generating >NT_187361.1 Homo sapiens chromosome 1 unlocalized genomic scaffold, GRCh38.p13 Primary Assembly HSCHR1_CTG1_UNLOCALIZED bases [100,000–1,099,999]: -439887.7625512469

## Hidden Markov model
> Calculate transform matrix of each state(aaa,cg,single_nucleobase): 9 parameters.
  Calculate each nucleobase(a,t,c,g) probability of occurrence in each state(aaa,cg,single_nucleobase): 12 parameters.
  Use Viterbi Algorithm to find the max probability of generating nucleobase sequence. 
  Number of free parameters: 21.
 
the log base 2 probability of Hidden Markov model generating bases [100,000–1,099,999]: -2058702.295249597
the log base 2 probability of Hidden Markov model generating bases [1,100,000–2,099,999]: -2061644.2097264999
the log base 2 probability of Hidden Markov model generating >NT_187361.1 Homo sapiens chromosome 1 unlocalized genomic scaffold, GRCh38.p13 Primary Assembly HSCHR1_CTG1_UNLOCALIZED bases [100000–1099999]: -154260.93062852055

## running time and memory usage
running time : 5.938091s
memory usage : 4.810811MB