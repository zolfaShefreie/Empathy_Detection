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

## Results
<table>
  <tr>
     <td>
      Transformers
    </td>
    <td>
      Result
    </td>
  </tr>
  <tr>
    <td>
      GPT-2
    </td>
    <td>
      <img width="244" alt="image" src="https://user-images.githubusercontent.com/44172962/236611349-90cf8e91-7a41-4fb0-99f6-2f7d08e960d5.png">
    </td>
  </tr>
    <tr>
    <td>
      DialoGPT
    </td>
    <td>
      <img width="245" alt="image" src="https://user-images.githubusercontent.com/44172962/236611411-169628a7-149a-4d98-b4e7-4aed9eb822a9.png">
    </td>
  </tr>
    <tr>
    <td>
      Roberta
    </td>
    <td>
      <img width="246" alt="image" src="https://user-images.githubusercontent.com/44172962/236611439-53654e64-5042-45e7-8b3b-1e20b0e67ad5.png">
    </td>
  </tr>
</table>
