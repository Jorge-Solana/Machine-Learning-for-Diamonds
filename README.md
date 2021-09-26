# Machine Learning for Diamond Price

![portada](https://github.com/Jorge-Solana/Machine-Learning-for-Diamonds/blob/main/images/1_U7QAaRAsfm455j7ljF2TgA.png)

## Scope

The scope of this project is simple yet effective.

Make the best machine learning model to predict the price of diamonds given certain characteristics.

The characteristics given for the diamonds are the following:

- Carat: weight of the diamond
- Cut: quality of the cut (Fair, Good, Very Good, Premium, Ideal)   
- Color: diamond colour
- Clarity: a measurement of how clear the diamond is
- x: length in mm
- y: width in mm
- z: depth in mm
- Depth: total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)
- Table: width of top of diamond relative to widest point (43--95)


## Methodology

For this project, it has been developed by training and testing some Machine Learning models to see which one of them performs better under the metric of the Root Mean Squared Error (RMSE).

Some of the variables mentioned before were categoriacal at first, so before triying any regression model, they had to been converted into non categorical (floats ot integers).

The technique for this was by doing a mapping where all the unique variables inside this columns were assigned a number based on its order of matter.

The different models that had beed tried are:

- Decision tree regressor
- Random forest regressor
- Gradient boosting regressor

All this model had been developed and searched under a Grid Search and given some hypeparameters to perform lots and lots of models and then extracting the best model out of all from the Grid Search.

This three models were trained with a given sample which was divided into train and test. Trained with this train partition and then tested with the test partition.

All the waiting:

![image](https://github.com/Jorge-Solana/Machine-Learning-for-Diamonds/blob/main/images/9afd181fb537e19024c43ed50394d6ce.png)

After that the best model of each grid for each model was implemented into the `test.csv` for a later upload to kaggle.

## End results

In the end, the best model found was a gradient boos with the following characteristics:

- max_depth = 12
- max_features = 7
- min_samples_split = 30
- n_estimators = 300

## Libraries used
- [Pandas](https://pandas.pydata.org/)

- [Numpy](https://numpy.org/)

- [Seaborn](https://seaborn.pydata.org/)

- [Matplotlib](https://matplotlib.org/)

- [SciKit-Learn](https://scikit-learn.org/stable/)

