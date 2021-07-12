# NN

### Authors
- Mihajlo Perendija @mihajlo-perendija
- Petar Bašić @coperope

### Original data
Project is inspired by DCASE challange http://dcase.community/challenge2019/task-sound-event-detection-in-domestic-environments
Original dataset for this project can be found at http://nlp.cs.aueb.gr/software_and_datasets/EURLEX57K/index.html

### Code organization
As this is mainly a research project, there is no final runnable code ready. 

Code is organized in multiple colab notebooks:

- initial_experiments_mfcc_creation -> holds code with initial data exploration, creation of MFCC values for audio samples (vectorization) and models for sound detection task (basic NN, GRU + NN, CNN + NN) + some experiments with splitting sequences. 
- seq_to_seq_prepare_initial_test -> holds code for preparing data for seq_to_seq model (creates output/target sequences) and initial experiments with seq_to_seq model (for sound event detection task). 
- seqtoseq_testing -> code with further seq_to_seq model experiments, advanced evaluation with sed_eval library & creation and evaluation of ansabmle model
- CNN_splitted_sequences -> holds code for creation and evaluation of CNN based model for sound **event** detection. 
- Sequence_to_seq_beg_end_pred -> holds code with initial experiments on using seq_to_x2seq model to predict beginning and end of sound in an audio sample (separately)
- Sequence_to_seq_beg_end_improved -> Various further experiments with previous model architecture. 
- seq_to_seq_beg_end_splitting_plus_gradients -> Further experiments on previous model with splitted sequences + trial of using only gradients for event detection. 

All colabs expect code, data, pre-trained models & prepared (vectorized) data to be uploaded on google drive.

Original code can be found in:
- https://drive.google.com/drive/folders/1BoAbyzIohZp1GitEOGa64edf5lh_eJBq?usp=sharing
- https://drive.google.com/drive/folders/1giEv38zsG9lU8P_aLPmUW87DQJhTX-E4?usp=sharing
