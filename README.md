# FuturologyAI-R

The Futurism Project envisions a future where AI-powered cities, airspace, and underwater arenas redefine our way of life. They emphasize the importance of communication in all aspects of society and highlight the effectiveness of sign language in bridging communication gaps.

In regions where language barriers exist, sign language can play a crucial role in conveying messages and building connections, especially in the context of tourism, travel, and underwater activities like scuba diving. Sign language is also essential for individuals with mental or physical disabilities to communicate with each other.

To address these communication challenges, the project aims to create a virtual chat assistant powered by GPT, incorporating various sign languages. This chat assistant will empower people, regardless of their health condition, to interact with others and perform daily tasks effectively, fostering inclusivity in society. The product will be a compact hardware device equipped with signal indicators and virtual try-on features.

One practical use case for this virtual chat assistant is to monitor air pollution levels and provide information through sign language, as detailed in the provided Lite paper and White paper, which address the significant issue of air pollution in society. Overall, the project aims to leverage AI and sign language to enhance communication, accessibility, and well-being for all individuals in the future.

*** Note : The full installation package of the exact entire AI, virtual chat assistant with basic sentiment analysis features will only be provided after being shortlisted to the final judginng round/s. 

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

Clone the repository.git clone https://github.com/FuturologyAIR/FuturologyAI-R.git

1.Navigate to the project directory.

cd your-project

Install dependencies.

# Use the appropriate package manager for your project, e.g., pip or npm
pip install -r requirements.txt


Additional setup steps, if necessary.
Usage

# Example usage
python your_script.py

Others whom wish to contribute to our project by providing us some tips, share with us on 
how we can seek improvement for the next judging round. 

There is no license for this as we are temporary hosting this here...

### Prerequisites

Using the Hugging Face and Streamlit, the code for a basic sentiment analysis features is as follows ...

The air pollution datasets are for deep learning frameworks and not for NLP, have to be separately processed. 

Require a GPU/ Cloud services to do up this air pollution datasets. 

Need more stakeholders like the members of public onboard this mission as well...

Based on this basic sentiment analysis features, we can setup the news from the reporting chat 
agent and/or virtual chat assistant embedded. 

```
// E.g The gates of heaven have been opened (POSITIVE: 0.999289870262146)
// E.g The gates of hell have been opened (NEGATIVE: 0.91)

import streamlit as st
from transformers import pipeline

model = pipeline("sentiment-analysis")

def main():
    st.title("Hugging Face Model Demo")

    # Create an input text box
    input_text = st.text_input("Enter your text", "")

    # Create a button to trigger model inference
    if st.button("Analyze"):
        
        # Perform inference using the loaded model
        result = model(input_text)
        st.write("Prediction:", result[0]['label'], "| Score:", result[0]['score'])

if __name__ == "__main__":
    main()
```
