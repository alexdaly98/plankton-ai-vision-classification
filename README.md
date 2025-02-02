# Plankton_classification_teamA001(Les Jongleurs) - Adrien Antonov, Alexandre Daly, Maxence Duplech, Nicolas Petitmangin

## Requirements

Before running any code, make sure to install all the dependancies by running
```
pip3 install -r requirements.txt
```

## Train a model

The folowing command is training the best model that you propose with the training set images given in the path PATH_TO_TRAINING_SET
```
python3 main.py train PATH_TO_TRAINING_SET
```

All training parameters (image_transform, image_transform_params, batch_size, model, optimizer, f_loss, nb_epochs and training_description) can be defined at the beginning of the " if __name__=="__main__" " in main.py

## Test a model

The folowing command is loading the model whose checkpoint fullpath is PATH_TO_CHECKPOINT, testing the model on the images provided in PATH_TO_TEST_SET and outputting the label csv file ready for submission - csv is stored at the root of the project once generated
```
python3 main.py test PATH_TO_CHECKPOINT PATH_TO_TEST_SET
```
Our best model is with PATH_TO_CHECKPOINT = "logs/resnet50_finetuning_nonweightedloss_batch128_Adam_2/best_model.pt" and the parameters (mentioned in "Train a model" section) given in the last commit



