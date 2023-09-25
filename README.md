# Video-Game-Recommender
Recommend Video Games to users based on their personal interests and choices and gaming habits.

## Dataset:
steam-200k.csv - https://www.kaggle.com/tamber/steam-video-games

steam-200k.csv dataset is used for collaborative filtering recommender system. Steam is the world's most popular PC Gaming hub, with over 6,000 games and a   community of millions of gamers. With a massive collection that includes everything from AAA blockbusters to small indie titles, great discovery tools are a highly valuable     
asset for Steam.  This dataset is generated entirely from public Steam data. This dataset is publicly available in kaggle.

 
 ## Objectives
  1. Exploration and Analysis of steam-200k.csv dataset.
  2. Create rating using Expectation Maximization algorithm
  3. Generate recommendations using collaborative filtering algorithm: SVD Algorithm.
  4. Improving and optimizing SVD algorithm performance using Stochastic Gradient Descent.

  
## Metrics
  Root Mean Square Error(RMSE) is used as metrics.

## Data Visualization
  ![image](https://github.com/BiswarupMukherjee1/Video-Game-Recommender/assets/89087014/e21d8ef8-651d-40a4-9633-d50711372bf6)

## Expectation Maximization Algorithm
 EM algorithm find groups (5) of people with similar gaming habits and that would potentially rate a game in a similar way
 ![image](https://github.com/BiswarupMukherjee1/Video-Game-Recommender/assets/89087014/43a6fe42-9e43-49bb-b011-566ee6ecb6d6)

  ![image](https://github.com/BiswarupMukherjee1/Video-Game-Recommender/assets/89087014/5b7eb636-1e69-4fdd-b7d7-470a1dca40ef)

## SVD with Stochastic Gradient Descent
![image](https://github.com/BiswarupMukherjee1/Video-Game-Recommender/assets/89087014/2260d450-5b1e-412f-98fa-338b2ece4b57)

The plot shows that the SVD via gradient descent converges to zero on the train dataset, while the RMSE for our train dataset stays around 0.60 approximately . 

We see that after the 75 - 100th iteration, the accuracy on the test dataset stops improving (the RMSE remains around the same value). The accuracy on the test data could be improved by using more leading components(latent factors), the trade-off being more computation time required. 

## Results 
| S.N | Algorithm            | RMSE  |
| ----|:-------------:| -----:|
|  1  | SVD                  | 2.93 |
|  2  | SVD Gradient Descent |  0.424 |

RMSE calculated for basic SVD is greater than for SVD using gradient descent. So accuracy of prediction for SVD using gradient descent is better.

Using EM Algorithm on Predicted User Item Matrix to find a reasonable 1-5 star rating.
![image](https://github.com/BiswarupMukherjee1/Video-Game-Recommender/assets/89087014/9c241710-2b75-4b4e-a502-36717d8c3400)

## Final Prediction using predicted user item matrix
![image](https://github.com/BiswarupMukherjee1/Video-Game-Recommender/assets/89087014/b8a12379-5f41-4bab-bba6-d8cbf53104f6)



