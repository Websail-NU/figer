Fine-Grained Entity Recognizer
=============================

This distribution contains the source code for the experiments presented in the following research publication:

    Xiao Ling and Daniel S. Weld (2012). 
    "Fine-Grained Entity Recognition", 
    in Proceedings OF THE TWENTY-SIXTH AAAI CONFERENCE ON ARTIFICIAL INTELLIGENCE (AAAI), 2012.

# Download the model file

One can test the trained model on the evaluation data or new data as they wish. 

Run `./downloadModel.sh` to download the [Model](https://drive.google.com/open?id=0B52yRXcdpG6MWlVXaTFXWVZQYjg) and save it at the root directory. 

A better [model](https://drive.google.com/open?id=0B52yRXcdpG6Mbm1TdHhYdVBmSnM) has been trained and can be fetched by `./downloadModel.sh new`. Change the config value accordingly.

## Replicate the experiments

To run the experiments in the AAAI-12 paper, you can proceed as follows:

    $ ./run.sh "aaai/exp.conf" &> aaai/exp.log

## Run FIGER on new data

To make predictions on new data, please see `package edu.washington.cs.figer.FigerSystem` for example code or run:

    $ sbt "runMain edu.washington.cs.figer.FigerSystem <text_file>"

# Training Data

The training data `train.tar.gz` is serialized in [Protocol Buffer](http://code.google.com/p/protobuf/). Please see `entity.proto` in the code package for the definitions.

Download [link](https://drive.google.com/open?id=0B52yRXcdpG6MdkNEaE5IVzkxR0k)

