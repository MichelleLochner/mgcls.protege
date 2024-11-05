## hyperparameters_experiment1.csv

This corresponds to section A1 in the appendix. The columns refer to the different hyperparameter values described in the appendix. The `loss` refers to the training loss. `validation_fraction` is non-zero if a validation set was used, reducing the amount of available data for training. `recall_mean` and related columns contain statistics about the performance running Protege 50 times with standard settings. Note that in this early experiment, we still selected the initial sources for labelling randomly which is the main source of the high variance.

## hyperparameters_experiment2.csv

Experiment corresponding to section A2 where only BYOL hyperparameters are varied. The column names refer to hyperparameters described in the text. The data are sorted by validation loss.

## hyperparameters_experiment3.csv

Experiment corresponding to section A3 where a few BYOL hyperparameter configurations are selected (indicated by `features_filename`) and passed through various configurations of Astronomaly. The column names refer to hyperparameters described in the text. The data are sorted by validation loss.