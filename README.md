A audio classifier model for a Kaggle competition | 11 March - 3 June

The bird-udd file was used for trianing the model and the submission file uses the pre-trined model from hugging face repository for competition's model evaluation. 

## Description
How do you protect an ecosystem you can’t fully see? One way is to listen.
This competition involves building models that automatically identify wildlife species from their vocalizations in audio recordings collected across the Pantanal wetlands. This work will support more reliable biodiversity monitoring in one of the world’s most diverse and threatened ecosystems.

Understanding how ecological communities respond to environmental change and restoration efforts is a central challenge in conservation science. The Pantanal — a wetland spanning 150,000+ km² across Brazil and neighboring countries — is home to over 650 bird species plus countless other animals, yet much of it remains unmonitored. Seasonal flooding, wildfires, agricultural expansion, and climate change make regular fieldwork challenging.

## Goal of the Competition
Conventional biodiversity monitoring across vast, remote regions is expensive and logistically demanding. To help address these challenges, a growing network of 1,000 acoustic recorders is being deployed across the Pantanal, running continuously to capture wildlife sounds across different habitats and seasons. Continuous audio recording allows researchers to capture multi-species soundscapes over extended periods, providing a community-level perspective on biodiversity dynamics. But the sheer volume of audio is too large to review manually, and labeled species data is limited.
This competition focuses on the development of machine learning models that identify wildlife species from passive acoustic monitoring (PAM). Proposed approaches should work across different habitats, withstand the constraints of messy, field-collected data, and support evidence-based conservation decisions. Successful solutions will help advance biodiversity monitoring in the last wild places on Earth, including research initiatives in the Pantanal wetlands of Brazil.
Listening carefully, and at scale, may be one of the most effective tools available to protect this landscape. 

## Evaluation
The evaluation metric for this contest is a version of macro-averaged ROC-AUC that skips classes that have no true positive labels.  

## Resources 
[Data](https://www.kaggle.com/competitions/birdclef-2026/data) 
[Trained-models](Katie090902/CNN_birdclassifier) 


## Result before submission 
The tradictional CNN architecture from efficientNet outperformed the hybrid model that included CNN and transformers 
diagnonsis: The number of epochs required to train a model with transformer is comparitively more than traditional CNN. 

## Result 
On submission the model scored a AUC score of 0.814 A huge room for improvement!
