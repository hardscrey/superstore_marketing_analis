https://www.kaggle.com/datasets/vivek468/superstore-dataset-final
!pip install kaggle

os.environ['KAGGLE_CONFIG_DIR'] = '/content/drive/MyDrive/kaggle'

! kaggle datasets download vivek468/superstore-dataset-final

from google.colab import drive
drive.mount('/content/drive')

file_path = '/content/superstore-dataset-final.zip'

with zipfile.ZipFile(file_path, 'r') as zip_ref:
    zip_ref.extractall('/content')
