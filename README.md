# steam_game_sales

## Overview

This project aims to analyze the Steam games sales data to determine influential factors on developing a new video game that will yield maximal sales when released on Steam. The ultimate goal of this project is to provide 3 actionable recommendations to the game developing companies to consider when developing a new game and creating marketing strategies for new release once the game is fully developed.

## Business Situation

There are many factors going into having a successful launch of a newly developed video game, and these factors include platform, genre, user count, and rating. Knowing how these features influence the sales of 

## Data Overview

The dataset was create using [SteamSpy](https://nik-davis.github.io/posts/2019/steam-data-collection/) gathering from the [Steam Store](https://store.steampowered.com/). The ready-to-use format of the dataset was provided by this [Kaggle page](https://www.kaggle.com/datasets/nikdavis/steam-store-games).

## Methods

First, some filters are applied to focus on a subset of the dataset. Specifically, this project focuses on english games that are compatible with windows. Also, the price per unit is focusing on below $100. Several features are engineered, including all **genres** of games, **total number of rating**, **ratio of positive ratings**, **low** and **high sales**, and **sales average**. It is important to note that there are some **limitations** to the dataset. For example, sequel informations are not available but having series of games can greatly influence sales of the games. Another limitation is that sales can only be inferred based on low and high number of owners and price per unit.

Several models are implemented to investigate influencial factors when predicting sales, and here are the models explored:

1. Baseline model (Dummy Classifier)

2. Decision Tree

3. Random Forest

4. Logistic Regression

The evaluation metric used is the **accuracy**, and the final model is the **multinomial logistic regression** model. The coefficients from the logistic regression model can provide useful information on not only the important features but also help interpret in terms of sales prediction.

## Conclusions

Lastly, based on the outputs from the final model, this project provides 3 actionable insights:

1. **In-game event to encourage ratings on steam**. This is to maximize users inputing ratings on Steam, as the number of ratings is one of the most important feature in determining the sales class.

2. **Strategy, education and multi-player genres**. These genres appear to increase sales especially in high and medium sales category. Developing a new game that can be categorized into strategy, education, or multi-player genres can be beneficial for maximizing revenue.

3. **Consider early access before official launch**. This strategy can maximize hype around the official launch, and potentially increase sales.

If you have any questions, pleace contact:

Sangyun (Yun) Thom: [sangyun.thom@gmail.com](mailto:sangyun.thom@gmail.com)

## Repository Structure