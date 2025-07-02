# iSmishU

**iSmishU** is a smishing detection system specifically designed for **Taglish** (a mix of Tagalog and English). It leverages **XLM-RoBERTa**, a powerful multilingual language model, to analyze message content and classify it as either *Smishing* or *Ham* (legitimate). To enhance detection capabilities, the system integrates **text classification** using a fine-tuned XLM-RoBERTa model with **URL analysis** through the [VirusTotal API](https://www.virustotal.com/).

## Key Features
- **Multilingual Support**: Utilizes XLM-RoBERTa to understand and process mixed Tagalog-English (Taglish) messages.
- **Layer Freezing Strategy**: Fine-tuning is performed by freezing alternate layers of the model to prevent overfitting and improve generalization.
- **URL Scanning**: Incorporates VirusTotal API to analyze links found in messages and provide additional signals for smishing detection.

## Dataset Disclaimer
Due to privacy concerns, the dataset used for training and testing is **not included** in this repository. The dataset contains real messages voluntarily shared by users, which include both legitimate and smishing samples. However, the provided code is fully functional and ready to use with your own Taglish dataset.

## Instructions for Use

1. **Use Google Colab**:
   - Recommended for faster training, easy dataset upload, and seamless model saving.
  
2. **Update Data Paths**:
   - Replace all placeholder paths marked with `#change datapath` in the code with the appropriate paths to your own dataset and model directories.

3. **Set Up VirusTotal API**:
   - Obtain your own API key from [VirusTotal](https://www.virustotal.com/) and update it in the designated part of the code.

## Notes

- **Read the Code Carefully**: Ensure you review the codebase to locate and modify all necessary paths and configuration variables.
- **Refer to the Documentation**: For a detailed explanation of the system, please read the included `iSmishU Documentation.pdf`.

