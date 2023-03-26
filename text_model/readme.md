# Empathy detection on text level
Text is given to the transformer-based model to predict one of the outputs of "empathy-seeker", "empathy-provider" and "none". [seeker_provider_empathy dataset](https://github.com/zolfaShefreie/Empathy_Detection/tree/main/datasets/seeker_provider_empathy) is used for training models using pytorch.
## Steps
- preprocessing </br>
  - delete punctuation marks form text
  - using "Hugging Face" tokenizer to tokenize texts
  - convert to pytorch tensor
  - convert labels to one-hot format
- create dataloader
- train transformer-based models</br>
below transformers/language models is used to create empathy classifier:
  - Bert
  - Roberta
  - Albert
  - XLNet
  - DistilBert
  - Electra
  - Deberta
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
      Bert
    </td>
    <td>
      <img width="245" alt="image" src="https://user-images.githubusercontent.com/44172962/227760585-372ae2ea-e399-433b-9b09-610021b1bcf3.png">
    </td>
  </tr>
    <tr>
    <td>
      Roberta
    </td>
    <td>
      <img width="244" alt="image" src="https://user-images.githubusercontent.com/44172962/227760551-351a49c5-80ea-433b-b872-8cea55cae6d9.png">
    </td>
  </tr>
    <tr>
    <td>
      Albert
    </td>
    <td>
      <img width="245" alt="image" src="https://user-images.githubusercontent.com/44172962/227760623-fb16cdd2-83ec-408d-8f48-86f118d2f13d.png">
    </td>
  </tr>
    <tr>
    <td>
      XLNet
    </td>
    <td>
    <img width="245" alt="image" src="https://user-images.githubusercontent.com/44172962/227760253-5450e352-1726-4cb6-b6a8-ce28e3af9aea.png">
    </td>
  </tr>
   </tr>
    <tr>
    <td>
      DistilBert
    </td>
    <td>
    <img width="244" alt="image" src="https://user-images.githubusercontent.com/44172962/227760312-81ee6f7c-c626-41ab-ad85-72552515b9a9.png">
    </td>
  </tr>
    </tr>
    <tr>
    <td>
      Electra
    </td>
    <td>
    <img width="246" alt="image" src="https://user-images.githubusercontent.com/44172962/227760377-bd5ccfd8-5eed-42df-92f4-db7d2b3d7d7c.png">
    </td>
  </tr>
    </tr>
    <tr>
    <td>
      Deberta
    </td>
    <td>
      <img width="246" alt="image" src="https://user-images.githubusercontent.com/44172962/227760410-3a3622f9-7169-4e07-bb4a-610c87a3dc12.png">
    </td>
  </tr>
</table>
