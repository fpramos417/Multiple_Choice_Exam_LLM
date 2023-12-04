# LLM to Solve Multiple Choice Science Exam


## Dataset Description

Your challenge in this competition is to answer multiple-choice questions written by an LLM. While the specifics of the process used to generate these questions aren't public, we've included 200 sample questions with answers to show the format, and to give a general sense of the kind of questions in the test set. However, there may be a distributional shift between the sample questions and the test set, so solutions that generalize to a broad set of questions are likely to perform better. Each question consists of a prompt (the question), 5 options labeled A, B, C, D, and E, and the correct answer labeled answer (this holds the label of the most correct answer, as defined by the generating LLM).

This competition uses a hidden test. When your submitted notebook is scored, the actual test data (including a sample submission) will be made available to your notebook. The test set has the same format as the provided test.csv but has ~4000 questions that may be different is subject matter.

## Files

train.csv - a set of 200 questions with the answer column 

test.csv - the test set; your task it to predict the top three most probable answers given the prompt. NOTE: the test data you see here just a copy of the training data without the answers. The unseen re-run test set is comprised of ~4,000 different prompts. 

sample_submission.csv - a sample submission file in the correct format

## Columns

prompt - the text of the question being asked 

A - option A; if this option is correct, then answer will be A 

B - option B; if this option is correct, then answer will be B 

C - option C; if this option is correct, then answer will be C 

D - option D; if this option is correct, then answer will be D 

E - option E; if this option is correct, then answer will be E 

answer - the most correct answer, as defined by the generating LLM (one of A, B, C, D, or E).
