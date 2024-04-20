Here's the corrected README file:

---

# Music Genre Classifier

This repository contains a Music Genre Classifier built using the GTZAN dataset. The dataset can be downloaded from [Kaggle](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification?resource=download).

## Dataset
The GTZAN dataset is used for this classification task. It consists of 1000 audio tracks each 30 seconds long, sampled at 22050Hz, and each belonging to one of 10 genres:
- Blues
- Classical
- Country
- Disco
- Hip-Hop
- Jazz
- Metal
- Pop
- Reggae
- Rock

## Usage
1. Extract the dataset into the `data` folder.
2. If using Google Colab, mount your drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
3. Run the `music_genre_classifier.ipynb` Jupyter Notebook to train and test the classifier.
4. To save the model in `.h5` format, use the following steps in your notebook:
   ```python
   import os
   import tensorflow as tf
   from tensorflow import keras
   import tensorflow.keras.models as models

   # Save the model in HDF5 format
   models.save_model(model, '/content/drive/MyDrive/saved_models/music_cnn.h5')
   ```

## Requirements
- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Librosa

## Usage Example
```bash
jupyter notebook music_genre_classifier.ipynb
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README further with additional information about your classifier, how to interpret the results, or any other details you find relevant for users of your repository.
