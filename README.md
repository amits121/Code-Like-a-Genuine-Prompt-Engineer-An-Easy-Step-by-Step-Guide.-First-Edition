 🚀 **Become Unstoppable**
## 🛠️ *Code Like a Genuine Prompt Engineer*: An Easy Step-by-Step Guide.
### 🔗 Learn to Integrate the LangChain Framework with Vector Database.
![Become Unstoppable (400 x 500 px)](https://github.com/amits121/Code-Like-a-Genuine-Prompt-Engineer-An-Easy-Step-by-Step-Guide./assets/9373813/cbb395c1-47a7-4bf7-a8ac-4d022223b94c)

📔 **This is the code repository for:** 
An in-depth, step-by-step guide to coding like a genuine Prompt Engineer. Master the seamless integration of the LangChain Framework with Vector Database.

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

**Sample Code:**
```python
import openai
# Replace 'YOUR_API_KEY' with your actual API key from OpenAI
openai.api_key = 'your openai key'

# Chain of thought prompting
chain_of_thought = (
    "Prompt 1: The shopkeeper starts with 50 apples.\n"
    "Prompt 2: In the morning, he sells 20 apples.\n"
    "Prompt 3: In the afternoon, he sells 15 more apples.\n"
    "Prompt 4: How many apples does he have left at the end of the day?"
)

# Make the API call to GPT-3.5 to get a response
response = openai.Completion.create(
        engine="text-davinci-002",
        prompt=chain_of_thought,
        temperature=0.7,
        max_tokens=100,
        #stop=["\n"]
    )
print(response.choices[0].text.strip())
## 🛠️ **Software and Hardware List**
For executing the code, you can either use **Google Colab** or install **Anaconda** to run the codes on Jupyter notebooks.
