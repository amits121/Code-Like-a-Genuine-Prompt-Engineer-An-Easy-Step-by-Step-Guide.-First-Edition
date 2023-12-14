 🚀 **Become Unstoppable**
## 🛠️ *Code Like a Genuine Prompt Engineer*: An Easy Step-by-Step Guide.
### 🔗 Learn to Integrate the LangChain Framework with Vector Database.




  ![Become Unstoppable (400 x 500 px)](https://github.com/ChatGPTHero/Code-Like-a-Genuine-Prompt-Engineer-An-Easy-Step-by-Step-Guide.-First-Edition/assets/146596849/776d17e5-63ef-4bca-a0b4-94fbb6dc4843)

📔 **This is the code repository for the Book Become Unstoppable** 
An easy step-by-step guide to coding like a genuine Prompt Engineer. Master the seamless integration of the LangChain Framework with Vector Database. 
📘 **First Edition** by **Amit Sarkar**


## 📘 **What is this book all about?**

**This book offers more than just knowledge; it holds the power to transform you.** As you delve into its pages, you'll unlock insights that propel you into the ranks of the world's top candidates. It's not merely about learning; it's about undergoing a profound evolution that sets you apart.

**Key takeaways:**  
- **Transformative Insights:** Propel yourself into the world's top echelon of candidates.
- **From Questions to Prompts:** Learn to swiftly transition from business queries to high-performance prompts for ChatGPT in production.
- **Master Prompt Engineering:** Harness various techniques with Python and Jupyter notebooks.
- **Leverage Powerful Tools:** Dive deep into the features and APIs of ChatGPT, LangChain, and Pinecone Vector Database.

## 📘 Topics Covered in This Book

**- Open AI and its APIs**  
**- Prompt Engineering:**  
  From basics to a deep dive, including detailed discussions from some relevant research papers.

**- Integrating ChatGPT using code:**  
  Practical implementation from the official OpenAI cookbook. Step-by-step instructions on various libraries, packages, APIs, and functions.

**- LangChain:**  
  A comprehensive exploration of the intuitive open-source framework. Learn how to integrate LLMs with the LangChain Framework using `PromptTemplates` and `.chains`.

**- Retrieval, Text Embeddings, and Vector Stores:**  
  Understand and implement the integration of LLMs using LangChain.

  ## 📜 **Research Papers**
To download all the relevant research papers discussed in the code, please visit [ChatGPT Hero Research Papers](https://www.chatgpthero.io/book-research-papers/).

## 📁 **Instructions and Navigations**
All of the code is organized into folders. 

**Before you begin two most important points to note**
Why You May Encounter Variations in Output When Running the Same Code from this Book in Jupy-ter Notebook: When using the OpenAI API to run a model, you often receive similar but slightly different results due to the inherent stochasticity or randomness in the generation process. OpenAI's language models, like GPT-3 and GPT-4, employ a technique called "sampling" to generate text. During sampling, the model considers multiple possible next words or tokens at each step and selects one based on probabilities. This probabilistic nature means that even with the same prompt, minor variations in the initial conditions, such as the internal model state or the random seed, can lead to different choices being made at each step of text gen-eration.
As a result, when you run the same prompt multiple times, you're likely to receive variations in the generated text. This can be beneficial because it allows for diversity in responses and can help you explore different an-gles or ideas related to your query. However, it's essential to be aware of this variability, and all the codes dis-cussed in this book may give you slightly different output than the output you obtain when you run them. You can control the level of randomness or creativity by adjusting parameters like the "temperature" in the API re-quest, where higher values lead to more randomness, and lower values produce more deterministic outputs. 

**OpenAI released version 1.0:** On November 8, 2023, OpenAI released version 1.0. However, most of the codes on GitHub (I will show you how to access vast repositories of code on GitHub in advanced lessons) are still running on old versions. For a beginner, migrating all the codes to the new version would be extremely hard. Please follow all my codes on this Github repository and I will update codes on a regular basis. Also please join our Discord  Channel  where I will give you all updates on regular basis.  Please visit https://www.chatgpthero.io/ for all the links provided in this book.  For more information about the OpenAI latest version please visit https://github.com/openai/openai-python/discussions/742.




**Sample Code:**
```python
!pip install openai 
from openai import OpenAI

# Replace 'YOUR_API_KEY' with your actual API key from OpenAI

client = OpenAI(
    api_key = 'your api key', )
# Chain of thought prompting
chain_of_thought = (
    "Prompt 1: The shopkeeper starts with 50 apples.\n"
    "Prompt 2: In the morning, he sells 20 apples.\n"
    "Prompt 3: In the afternoon, he sells 15 more apples.\n"
    "Prompt 4: How many apples does he have left at the end of the day?"
)

# Make the API call to GPT-3.5 to get a response
response = client.completions.create(
        model="text-davinci-002",
        prompt=chain_of_thought,
        temperature=0.7,
        max_tokens=100,
        #stop=["\n"]
    )
print(response.choices[0].text.strip())
## 🛠️ **Software and Hardware List**
For executing the code, you can either use **Google Colab** or install **Anaconda** to run the codes on Jupyter notebooks.
