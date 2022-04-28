# Hindi Arithmetic Word Problems - HAWP

This repository provides HAWP(a first ever diverse dataset for Hindi) for evaluating and developing MWP Solvers for Hindi. It contains 2336 Hindi Math Word Problems (MWPs), and is published in the paper "HAWP: a Dataset for Hindi Arithmetic Word Problem Solving".


The dataset can be found in `hawp/dataset/`

## About the dataset
| Name          | HAWP                                            |
|---------------|-------------------------------------------------|
| Version       | v1.0                                            |
| Resource Type | Corpus                                          |
| Language Type | Monolingual                                     |
| Language      | Hindi                                           |
| Size          | 2336 MWPs                                       |
| Modality      | Written                                         |
| Annotation    | Equation, Relevant Indices, Number Of Operators |
| Use           | For Automatic Word Problem Solving              |
| Format        | JSON                                            |


## Snapshot of dataset:
```json
{
    "pIndex": 0,
    "Problem": "सोहन ने 7.423 की.ग्रा. चावल तथा 6.129 की.ग्रा. दाल खरीदी। सोहन ने कुल कितना सामान खरीदा?",
    "Equation": "X = ( 7.423 + 6.129 )",
    "Relevant Indices": [
      0,
      1
    ],
    "Number of Operators": 1
  }

```
- **pIndex**: A unique identifier for a MWP
- **Problem**: The word problem text (includes statements and clues for solving an MWP) and question to be solved based on the word problem text.
- **Equation**: The equation used to solve the MWP
- **Relevant Indices**: List of incides of quantities in the MWP that are relevant to solve the question. Whenever the MWP requires world knowledge or uses implict quantities, the relevant indices list contains `implicit` keyword.
- **Number of Operators**: Number of operations required to solve the MWP.
