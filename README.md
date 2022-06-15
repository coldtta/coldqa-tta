# Robust Question Answering against Distribution Shifts with Test-time Adaption: An Empirical Study


## We show the benchmarking results on ColdQA as follows:

Metric: EM/F1

### Benchmarking results on ColdQA for XLMR-base

| Model     |     NoiseQA-syn     |   NoiseQA-na    |        XQuAD        |        MLQA         |        MRQA         |         Avg         |
| :-------- | :-----------------: | :-------------: | :-----------------: | :-----------------: | :-----------------: | :-----------------: |
| xlmr-base |     66.64/78.67     |   66.05/77.91   |     55.59/71.42     |     47.14/65.27     |     40.11/52.78     |     55.11/69.21     |
| MVR       |     68.85/80.10     |   67.87/78.91   |     58.08/73.34     |     48.45/66.33     |     41.40/53.84     |     56.93/70.51     |
| xTune     |     70.95/81.52     |   69.75/80.66   |     58.78/73.75     |     49.87/67.76     |     43.36/56.03     |     58.54/71.94     |
| Tent      |     68.02/79.38     |   67.80/78.92   |     57.40/72.56     |     47.59/65.13     |     40.39/52.43     |     56.24/69.68     |
| PL        |     68.50/79.62     |   68.14/79.22   |     57.91/72.69     |     47.75/65.17     |     39.94/52.20     |     56.45/69.78     |
| OIL       |     68.75/79.86     |   68.40/79.40   |     57.96/72.64     |     48.39/66.08     |     41.80/53.92     |     57.06/70.38     |
| xTune+PL  |     71.73/82.12     | **70.87**/81.10 | **60.23**/**74.56** |     50.33/68.10     |     41.14/53.58     |     58.86/71.89     |
| xTune+OIL | **71.90**/**82.24** | 70.81/**81.15** |     60.13/74.46     | **50.67**/**68.53** | **44.65**/**57.00** | **59.63**/**72.68** |



### Benchmarking results on ColdQA for XLMR-large

| Model      |     NoiseQA-syn     |   NoiseQA-na    |      XQuAD      |      MLQA       |        MRQA         |         Avg         |
| :--------- | :-----------------: | :-------------: | :-------------: | :-------------: | :-----------------: | :-----------------: |
| xlmr-large |     65.55/79.91     |   64.17/78.37   |   63.15/78.77   |   53.87/72.58   |     46.18/59.46     |     58.58/73.82     |
| FGM        |     64.93/79.71     |   62.94/77.96   |   63.21/78.74   |   54.14/72.72   |     45.09/58.65     |     58.06/73.56     |
| PGD        |     65.91/80.16     |   63.75/78.05   |   63.80/78.91   |   54.28/72.82   |     46.25/60.19     |     58.80/74.02     |
| Freelb     |     66.22/79.97     |   64.37/77.88   |   63.34/78.79   |   53.93/72.51   |     46.07/59.99     |     58.79/73.83     |
| InfoBert   |     64.59/79.52     |   62.66/77.46   |   62.31/78.28   |   53.98/72.52   |     45.05/59.14     |     57.72/73.39     |
| MVR        |     67.06/80.96     |   64.76/78.59   |   63.35/78.61   |   54.47/72.80   |     47.97/61.60     |     59.52/74.51     |
| xTune      |     70.11/83.17     |   67.20/80.54   |   65.00/79.91   |   56.30/74.33   |     48.94/62.37     |     61.51/76.06     |
| Tent       |     52.91/69.01     |   54.29/69.87   |   63.22/78.91   |   53.85/72.17   |     49.65/62.95     |     54.78/70.58     |
| PL         |     71.26/83.60     |   69.32/81.67   |   64.05/79.21   |   54.27/72.57   |     50.12/63.21     |     61.80/76.05     |
| OIL        |     71.57/83.93     |   70.11/82.22   |   64.19/79.37   |   54.41/72.90   |     49.93/62.55     |     62.04/76.19     |
| xTune+PL   |     76.01/86.60     | **73.83**/84.55 | 65.74/**80.15** | **55.78**/73.92 |     47.29/59.81     |     63.73/77.01     |
| xTune+OIL  | **76.13**/**86.72** | 73.69/**84.61** | **65.83**/80.12 | 56.24/**74.34** | **51.00**/**63.86** | **64.57**/**77.93** |

