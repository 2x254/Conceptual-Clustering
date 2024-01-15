This is the implementation of the CCA-k-RFP approach. To run the code, follow the steps below:
1) Download the files and the dataset.
2) To generate k-RFP, use the command below to run the solver. This is an example for generating classical patterns for the mushroom dataset:

./xsat4DAR -kx=0 -ky=1 -minsupp=1  -gdar=1 -msi=1 dataset/mushroomfinal.txt | grep "^[1-9]" >RelaxedPatterns/patternsk0.txt

For the parameters, kx is relaxation, minsupp is the minimum support (alpha), and msi is the minimum item frequency (gamma).

3) Install numpy: pip install numpy
4) Install pulp: pip install pulp
5) Run the Python files ILP_classical_patterns.py (for classic patterns) and ILP_k_RFP.py (for k-RFP).
