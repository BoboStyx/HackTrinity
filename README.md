# Verdict Predict #
Lawyers often spend a significant amount of time conducting research to find precedents and relevant case law to support their arguments. Verdict Predict aims to streamline this process, enabling lawyers to compare their arguments to similar past cases quickly. We also trained an AI model to predict the outcome of the case counteracting tunnel vision. In the end they user will get similar cases and a prediction for the verdict as an outcome.

Model inference code located in 
[link](https://github.com/SamManoli975/HackTrinity/tree/main/APIs/HackTrinity)
![image](https://github.com/user-attachments/assets/d3723250-92f7-4a40-b8ff-06be985e497e)
We trained a bert model based on the [US Class Action Dataset](https://huggingface.co/datasets/darrow-ai/USClassActions/viewer/default/train?p=2&row=203) trained using BCE loss function
## Technical Architecture ##
![image](https://github.com/user-attachments/assets/9f9594ed-eddb-4443-bc89-7fc3c85d3c35)
We then encoded each legal case in the dataset using a transformer encoder. This allows us to retrieve similar cases by calculated the cosine similarity of the search case and the cases located in the dataset 


### Example Code Snippet
```npm start ```
```python APIs/HackTrinity/restAPI.py  ```
