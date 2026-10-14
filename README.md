# econ3916-lab06-sampling
Lab 06 Submission

# Sampling for Machine Learning — Train-Test Splits

## Objective
I studied how the way I split and sample data affects whether a model's results can be trusted.

## Methodology
- I explored the Titanic dataset, which has 891 passengers, with survival as the target.
- I compared a naive train-test split with a stratified split, and checked that stratifying keeps the survival rate the same in both the training and test sets.
- I found data leakage in a StandardScaler step and a SimpleImputer step, and fixed both so they learn only from the training data.
- I wrote a function, `split_by_share()`, that splits a table using a test share and a seed, and checked its output against the lab's own split.
- I simulated the 1936 Literary Digest polling failure on a population of 10 million voters.
- I computed Meng's data defect correlation and compared a biased sample of [YOUR VALUE] responses with a random sample of 50,000.
- I ran 100 replications to compare the biased sample with the random sample.

## Key Findings
Sample design matters more than sample size. The biased sample of [YOUR VALUE] responses was less accurate than the random sample of 50,000. A data defect correlation of [YOUR VALUE] produced an error of [YOUR VALUE] percentage points. On the Titanic data, stratifying kept the survival rate the same in both halves of the split, and fitting the scaler and imputer only on the training data removed the leakage I found.
