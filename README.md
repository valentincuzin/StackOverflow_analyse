# StackOverflow_analyse
[sources](https://www.kaggle.com/datasets/stackoverflow/stackoverflow)

# Requete SQL
[bigQuerie](https://console.cloud.google.com/bigquery?sq=873335312714:99a48ba060e245a0adebaac43df8aa41&project=test-bot-389206&ws=!1m9!1m3!8m2!1s873335312714!2s99a48ba060e245a0adebaac43df8aa41!1m4!1m3!1stest-bot-389206!2sbquxjob_73982a43_1926adbc33a!3sUS!1m20!1m4!4m3!1sbigquery-public-data!2sstackoverflow!3sposts_questions!1m4!4m3!1sbigquery-public-data!2sstackoverflow!3sposts_answers!1m4!4m3!1sbigquery-public-data!2sstackoverflow!3stags!1m4!4m3!1sbigquery-public-data!2sstackoverflow!3sposts_privilege_wiki)

```SQL
SELECT
  *
FROM
  `bigquery-public-data.stackoverflow.posts_answers` as bd
WHERE
  bd.creation_date >= '2018-01-01' 
  AND bd.creation_date < '2018-02-01'
ORDER BY
  bd.creation_date
```



# Recherche
## Detection anomalies
https://arxiv.org/pdf/1704.07706
Avec R : https://github.com/twitter/AnomalyDetection/
Seasonal ESD (S-ESD)

## Detection de periode de cyvle
https://stackoverflow.com/questions/59265603/how-to-find-period-of-signal-autocorrelation-vs-fast-fourier-transform-vs-power/59267175#59267175
https://medium.com/@krzysztofdrelczuk/acf-autocorrelation-function-simple-explanation-with-python-example-492484c32711
from statsmodels.graphics.tsaplots import plot_acf

## Time warping
from dtaidistance import 
https://dtaidistance.readthedocs.io/en/latest/usage/dtw.html
https://medium.com/@markstent/dynamic-time-warping-a8c5027defb6

## Clustering with DTW
https://tslearn.readthedocs.io/en/stable/user_guide/clustering.html

## Frequent pattern mining
https://medium.com/@codingTuts/python-code-for-frequent-pattern-mining-45ae6fb167bb