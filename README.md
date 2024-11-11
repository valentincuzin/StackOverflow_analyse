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