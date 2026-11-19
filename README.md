# Project1_C7147_module
Programming for Life Sciences Project 1 Assessment: Identifying Mutations in NGS Data

Purpose:
This programme analyses next-generation sequencing reads from samples to identify DNA mismatches with a reference sequence. The aim is to compare mutation patterns between treatment and control groups and determine whether treatment is associated with increased mutation frequency.

How to run the programme:
Open the Project 1 notebook in Google Colab and run the setup cells to load the reference sequence and read dataset. Then run each code cell in order. The programme will analyse the sequencing reads, generate sample summaries, compare mutation positions between experimental groups, and print the final statistical results.

Inputs and outputs:
The programme uses two input files:
reference.txt containing the reference DNA sequence
reads.csv containing sequencing reads and associated metadata

Code design:
The programme was designed using separate functions for each step of the analysis. Each function performed a single specific task. The functions were created independently before being combined in later steps. Dictionaries were used frequently to store related information using key names. Invalid reads were not removed from the analysis, they were labelled with validation errors.

Testing:
Several tests were performed to ensure correctness. First valid sequences were tested to confirm that mutations were correctly identified. Then lowercase sequences were used to verify that reads were changed to uppercase during validation. Next, invalid sequences containing incorrect lengths and invalid characters were tested to ensure that appropriate error codes were returned without causing the programme to crash. Additional tests were carried out using custom datasets.
