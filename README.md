# Commonsense Validation and Explanation

This is the official repo for SemEval 2020 Task 4: Commonsense Validation and Explanation.

This task is inspired and extension of the ACL 2019 paper: Does It Make Sense? And Why? A Pilot Study for Sense Making and Explanation. [link](https://arxiv.org/abs/1906.00363)

Welcome to pariticipate on our Codalab competition [here](https://competitions.codalab.org/competitions/21080)!

## Introduction

The task is to directly test whether a system can differentiate natural language statements that make sense from those that do not make sense. We designed three subtasks. The first task is to choose from two natural language statements with similar wordings which one makes sense and which one does not make sense; The second task is to find the key reason from three options why a given statement does not make sense; The third task asks machine to generate the reasons and we use BLEU to evaluate them.

The detailed description of the task can be found in [Task Proposal](./TaskProposal.pdf).

### Example

#### Task A: Validation

Which statement of the two is against common sense?

- Statement 1: He put a turkey into the fridge. *(correct)*
- Statement 2: He put an elephant into the fridge.

#### Task B: Explanation (Multi-Choice)

Select the most corresponding reason why this statement is against common sense.

- Statement: He put an elephant into the fridge.

- Reasons:

  - **A**: An elephant is much bigger than a fridge. *(correct)*
  - **B**: Elephants are usually white while fridges are usually white.
  - **C**: An elephant cannot eat a fridge.

#### Task C: Explanation (Generation)

Generate the reason why this statement is against common sense and we will use BELU to evaluate it.

- Statement: He put an elephant into the fridge.

- Referential Reasons:

  1. An elephant is much bigger than a fridge.
  2. A fridge is much smaller than an elephant.
  3. Most of the fridges aren’t large enough to contain an elephant.

## Evaluation

Subtask A and B will be evaluated using **accuracy**. Subtask C will be evaluated using BLEU score.

## Deadlines

- Trial data ready July 31, 2019
- Training data ready September 4, 2019
- Test data ready December 3, 2019
- Evaluation start January 10, 2020
- Evaluation end January 31, 2020
- Paper submission due February 23, 2020
- Notification to authors March 29, 2020
- Camera ready due April 5, 2020
- SemEval workshop Summer 2020

## License

The dataset is distributed under the [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/legalcode) license.
