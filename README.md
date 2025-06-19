# Language-translation-model--Deploy-using-Hugging-Face 


Project Overview 

            * This project focuses on building a Neural Machine Translation (NMT) application to translate English sentences into Tamil using a fine-tuned transformer model.
            
            *The model is based on the Helsinki-NLP/opus-mt-en-dra architecture and was fine-tuned on a custom dataset to improve translation quality for domain-specific usage and enhanced linguistic fluency.

            *The final model is deployed using a Gradio web application, which is hosted on Hugging Face Spaces for easy user interaction and public access.

⚙️ Project Steps

    1)Model Selection: 

            * Used Helsinki-NLP/opus-mt-en-dra from Hugging Face for translation. 

    2)Data Preparation: 

            * Dataset formatted with columns: translation → {en: English text, ta: Tamil text}. 

            * Tokenization and preprocessing applied. 

    3) Model Fine-Tuning: 

            * Leveraged Seq2SeqTrainer from Hugging Face's Transformers library. 

            * Training included metrics like sacreBLEU to monitor translation quality. 

    4) Model Evaluation: 

            * BLEU scores tracked across epochs to assess translation improvement. 

            * Final BLEU score achieved: ~6.18, showing basic translation capabilities (can be improved with more data). 

    5) Model Saving:

            * Fine-tuned model artifacts (config, tokenizer, model weights) were saved and uploaded to Hugging Face. 

    6) Deployment:

            * Gradio-based web UI created for real-time user translation. 

            * Hosted in Hugging Face Spaces with interactive textbox input and output. 

📦 Dependencies:

    The following libraries are required to run the project and web app: 

               * transformers, gradio, torch, sentencepiece, numpy, evaluate. 

🚀 How to Use the App 

    1) Visit the Hugging Face Space. 
    
    2) Enter any English sentence in the input box. 

    3) Click “Submit” to get the Tamil translation.  

    Example:
    
    Input: "How are you?"

    Output: "நீ எப்படி இருக்கிறாய்?"

✅ Conclusion

      This project successfully demonstrates how to fine-tune a multilingual translation model and deploy it for interactive use. 
      While initial BLEU scores are modest, this project serves as a strong foundation for more advanced translation systems. 
      
Future improvements could include: 

    * Training with a larger, domain-specific corpus. 

    * Hyperparameter tuning and additional epochs. 

    * Adding post-processing or grammar correction layers. 

NOTE: Copy of language translation.ipynb file cannot view directly on github. If want to view the file,  can download and view the file.....
