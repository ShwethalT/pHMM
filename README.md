# pHMM
This is a custom Profile Hidden Markov Model used to identify Zinc Finger Motifs in peptide sequences of amino acids. It utilizes the Viterbi Algorithm to find the motif sequence. All matrices were manually made in R programming language with specific values.

Code is implemented in R. The version of RStudio that I created it in on is R.4.4.0 but if HMM package is installed then I think it should run on either IDEs as well.
I recommend RStudio just for convenience.

To load the code please click on the R source file entitled CS223_Project_HMM in IDE of choice (RStudio recommended)
Note: I have taken guidance from the in class exercise and the profile HMM scripts we used during lecture to make this script.

## Running the script
Run all commands till u reach observations
User can input sequence of choice in observations
Eg run:
### Sequence 1
observations <- c("T","A", "C", "T", "G", "A","G")

viterbi_result <- viterbi(hmm, observations)

print(viterbi_result)

avg_length <- avg_length + length(viterbi_result)

print("")
### Output:
The above prints out the sequence of hidden states and the motif (if any ) is identified as MI, M2, M3 , M4 , M5 or m1, m2, m3, m4 , m5  depending on which motif.
The first sequence corresponds to ACTGA and the second corresponds to TAACG.
