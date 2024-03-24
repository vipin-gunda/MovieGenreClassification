# MovieGenreClassification

## Set Up .gitignore
Maintain a .gitignore file that ignores the following:
- data/

## Set Up Data Folder
Create a folder called `data` in the root directory of the project. This folder will contain the data files for the project.

You can download the data from: https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

Make sure you rename the unzipped folder as **movies***. The directory should look like this: 
```
  \data
    \movies
      credits.csv
      keywords.csv
      links.csv
      links_small.csv
      movies_metadata.csv
      ratings.csv
      ratings_small.csv
```


## data_exploration.ipynb
This is a jupyter notebook that contains the data extraction process along with some minor data cleaning. It also contains exploratory data analysis and visualizations. The way the notebook processes different columns and fields in the metadata csv is useful for defining inputs/outputs of future models. 


## transformer.ipynb
This is a jupyter notebook that contains the transformer model. The model predicts the genre of a movie based on the movie's title and overview. The model is trained using the `transformers` library and the `Albert-Base-V2` model. This model was chosen because it is a smaller Transformer (~12 million parameters) so it was used to make training as quick as possible. The notebook also contains code to save the model and load it for future use. 

*Note: The ipynb may not work on your local machine due to the hardware requirements of the Transformers library. However, it should work smoothly on Google Colab.*