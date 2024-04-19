## Checkout the [Tableau Education](https://public.tableau.com/app/profile/leandro.lima/viz/EducationData_16503419309010/Story1?publish=yes) before continuing to read the project.

## Important steps in the project...

### Get_dummies() Section

#### Example

Here is an example of how `pd.get_dummies()` works.

![Get_Dummies() Part 1](https://github.com/samuelroiz/Predict_Credit_Risk/blob/main/Images/example_get_dummies_part_1.png) 

The following data frame, named *preview_get_dummies*, displays two non-numeric columns.

Then apply the `get_dummies()` code:

```python
pd.get_dummies(preview_get_dummies)
```

![Get_Dummies() Part 2](https://github.com/samuelroiz/Predict_Credit_Risk/blob/main/Images/example_get_dummies_part_2.png)

Now, the *preview_get_dummies* data frame has numeric columns, which means it meets the standards of machine learning models.

### Train and Test Data

#### How does train and test work and what is it doing to the data?

### Standard Scaler Section

#### How does the Standard Scaler work and what is it doing to the data?

Standard Scaler uses the formula:

```plaintext
z = (x - u) / s
```

where `z` is the scaled data, `x` is the data to be scaled, `u` is the average of the training samples, and `s` is the standard deviation of the training samples. The average or mean is calculated by summing all data points and dividing by the number of data points. In this scenario, `u` will sum all the training samples and divide by the number of these samples. The standard deviation formula involves placing the given values in one column, squaring each value, and then placing them in a second column. Find the sum of all values in the first column and square it, dividing this number by the number of data points in the first column, and call this `i`. Find the sum of the values in the second column, subtract `i` from it, and then divide the result by the number of data points minus one. This value leads to the `variance` of the sample and data, which is then square-rooted to give the standard deviation.

#### Example of Standard Scaler

To demonstrate the algorithm and how it functions, consider the dataset `{1,2,3,4,5}`. This dataset consists of 5 one-dimensional data points, each with one feature. Apply the standard scaler to the data, and the dataset becomes `{-1.41, -0.71, 0, 0.71, 1.41}`.

This example takes all of the data points and converts them to a range closer to 0 to 1. The standard scaler helps prevent outliers and keeps the data closer to each other rather than creating gaps.

## About the Data

The census data provided depends on race, age, and gender for education. The following image displays a bar chart of education levels. In this data, the majority have a high school diploma.

![Count Plot on Education in Census](https://github.com/laquita44/college_universities/blob/main/sam_data/juypter_notebook/2021%20Images/Education/count_plot.png)

The following image displays the outcome after applying the formula. If the outcome is negative, it indicates no possibility. If it is positive, then there is a higher probability.

![Doctor Analysis after applying formula 2021 to 2017-2019](https://github.com/laquita44/college_universities/blob/main/sam_data/juypter_notebook/2021%20Images/Education/doctor_prob.png)

![Model Outcome for Doctor Degree](https://github.com/laquita44/college_universities/blob/main/sam_data/juypter_notebook/2021%20Images/Education/model_outcome_for_doctor_degree.png)

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/samuelroiz/1af49ec9eea365bc845ba04c5071a976) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

- **Samuel Roiz** - *Data cleaning, Analyzed Data, Model* - [Profile](https://github.com/samuelroiz)
- **LaQuita Williams** - *Model* - [GitHub](https://github.com/laquita44)
- **Leo Lima** -

 *Data cleaned, API Keys, Model* - [GitHub](https://github.com/Leolima539)
- **Kevin Perez** - *Model, Data cleaned* - [GitHub](https://github.com/KevinKVNPR)

See also the list of [contributors](https://github.com/samuelroiz) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://gist.github.com/samuelroiz/1af49ec9eea365bc845ba04c5071a976) file for details.

## Acknowledgments

- Education
- Government Education
- Census
- USC Data Visualization
- CSUN Mathematics
