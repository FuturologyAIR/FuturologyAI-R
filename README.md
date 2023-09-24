# FuturologyAI-R

The Futurism Project envisions a future where AI-powered cities, airspace, and underwater arenas redefine our way of life. They emphasize the importance of communication in all aspects of society and highlight the effectiveness of sign language in bridging communication gaps.

In regions where language barriers exist, sign language can play a crucial role in conveying messages and building connections, especially in the context of tourism, travel, and underwater activities like scuba diving. Sign language is also essential for individuals with mental or physical disabilities to communicate with each other.

To address these communication challenges, the project aims to create a virtual chat assistant powered by GPT, incorporating various sign languages. This chat assistant will empower people, regardless of their health condition, to interact with others and perform daily tasks effectively, fostering inclusivity in society. The product will be a compact hardware device equipped with signal indicators and virtual try-on features.

One practical use case for this virtual chat assistant is to monitor air pollution levels and provide information through sign language, as detailed in the provided Lite paper and White paper, which address the significant issue of air pollution in society. Overall, the project aims to leverage AI and sign language to enhance communication, accessibility, and well-being for all individuals in the future.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation



### Prerequisites

Using the Hugging Face and Streamlit, the code for a basic chat ai assistant features is as follows ...

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
