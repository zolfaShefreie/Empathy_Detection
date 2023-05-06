# Converation Level Empathy Detection
Conversation is given to the transformer-based model to predict one of the outputs of "empathetic" and "not_empathetic". [conversation_empathy dataset](https://github.com/zolfaShefreie/Empathy_Detection/tree/main/datasets/conversation_empathy) is used for training models using pytorch.

## Steps
- preprocessing </br>
  - merge utterances of one converation
  - delete punctuation marks form text
  - add special tokens for "start of utterance" and "end of utterance"
  - using "Hugging Face" tokenizer to tokenize texts
  - convert to pytorch tensor
- create dataloader
- train transformer-based models</br>
below transformers/language models is used to create empathy classifier:
  - GPT-2
  - DialoGPT
  - Roberta
- evaluate
