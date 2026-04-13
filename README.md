# Project 3 - Classification of Dermal Medical Imaging
## Software 

Primary Software: Jupyter Notebook  
  
Add-on Packages: 
- os  
- numpy  
- pandas  
- matplotlib.pyplot  
- seaborn
- Image (from PIL)
- StratifiedKFold (from sklearn.model_selection)
- StandardScaler, OneHotEncoder, LabelEncoder (from sklearn.preprocessing)
- compute_class_weight (from sklearn.utils.class_weight)
- classification_report, confusion_matrix, f1_score (from sklearn.metrics)
- RandomForestClassifier (from sklearn.ensemble)
- tensorflow  
- keras (from tensorflow)
- layers (from tensorflow.keras)
- MobileNetV2 (from tensorflow.keras.applications)
- preprocess_input (tensorflow.keras.applications.mobilenet_v2)
- image (from tensorflow.keras.preprocessing)
- EarlyStopping (from tensorflow.keras.callbacks)
- ResNet50 (from tensorflow.keras.applications)
- preprocess_input (from tensorflow.keras.applications.resnet50)  

Platform: macOS

## Documentation Map

```
data/
└── metadata

outputs/
├── EDA/
│   ├── age-distribution.png
│   ├── age_vs_dx_heatmap.png
│   ├── class_distribution.png
│   ├── localization_distribution.png
│   ├── localization_vs_dx_heatmap.png
│   ├── sex_distribution.png
│   └── sex_vs_dx_heatmap.png
├── classification_reports 
│   ├── image_only_classification_report.png
│   ├── mobilenet_image_only_5fold_summary.png
│   ├── mobilenet_multimodal_5fold_summary.png
│   ├── multimodal_classification_report.png
│   ├── resnet_image_only_5fold_summary.png
│   └── resnet_multimodal_5fold_summary.png
└── confusion_matrices 
│   ├── image_only_confusion_matrix.png  
│   ├── mobilenet_image_only_confusion_matrix_5fold_average.png
│   ├── mobilenet_multimodal_confusion_matrix_5fold_average.png
│   ├── multimodal_confusion_matrix.png
│   ├── resnet_image_only_confusion_matrix_5fold_average.png
│   └── resnet_multimodal_confusion_matrix_5fold_average.png

scripts/
├── eda.ipynb
├── mobilenetv2_modeling_and_analysis.ipynb
└── resnet_model_and_analysis.ipynb

.gitignore
LICENSE
README.md
```

## Instructions for Reproduction  

### i.) Pulling the Data  
- The data was obtained a dataset from the Harvard Dataverse called “The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions.” The dataset includes two zip files: HAM10000_images_part_1.zip and HAM10000_images_part_2.zip. These two files were unzipped and combined to create one large file which we used for our models. Each file had roughly 5,000 jpegs so the large combined file has over 10,000 jpegs. Due to the size of the combined file, the dataset is too large to upload onto github. Once the large file is created, the data can be stored locally and used to run the models. We also uploaded the metadata file to use for a multimodal model. The link to these files can be found here: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T

## Note

The dataset in which we used for this project includes it's own license concerning the contents of the data. The license can be found here: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T&version=4.0&selectTab=termsTab
