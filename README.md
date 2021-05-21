

describing what the project is about and what packages must be installed so that all code works as expected (you can find a sample README.md here: https://github.com/PiotrZiolo/drln-navigation)

## Package versions
pandas > 1.2 (the most important)
numpy
matplotlib
seaborn
copy
random
itertools

## Scores

| Soultion          | Score HR@10   | Set                                       | tune_recommender                | note    |
| ---               | ---           | ---                                       | ---                             | ---     |
|RecAndEva-1.ipynb  | 0.001645      | user_room_segment, user_n_people_bucket   | LinearRegressionCBUIRecommender |         |
|v2                 | 0.002303      | user_room_segment, user_n_people_bucket   | LinearRegressionCBUIRecommender |         |
|v2                 | 0.026983      | full                                      | LinearRegressionCBUIRecommender |         |
|v2                 | 0.046726      | full                                      | SVRCBUIRecommender              | slow    |
|v2                 | 0.037183      | full                                      | RandomForestCBUIRecommender     |         |
|v2                 | 0.001645      | full                                      | XGBoostCBUIRecommender     |         |
|v2                 | 0.022047      | full                                      | LinearRegressionCBUIRecommender | update room_segment -> every 100        |