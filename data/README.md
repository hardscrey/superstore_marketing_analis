# Скачать файл Sample_Superstore.csv
[Kaggle Dataset(сайт)](https://www.kaggle.com/datasets/shubhammeshram579/bank-customer-churn-prediction](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)) / [Kaggle Dataset(github)](data/Sample_Superstore.csv)
# Использовать выгрузку с kaggle(необходимо наличие токена):
    !pip install kaggle
    os.environ['KAGGLE_CONFIG_DIR'] = '/content/drive/MyDrive/kaggle'
    ! kaggle datasets download vivek468/superstore-dataset-final
    file_path = '/content/superstore-dataset-final.zip'
    with zipfile.ZipFile(file_path, 'r') as zip_ref:
        zip_ref.extractall('/content')
    df = pd.read_csv('Sample - Superstore.csv')
