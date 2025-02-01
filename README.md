# 📜 AI-Driven Custom Storybook Creation

This project utilizes the **LLaMA 13B** language model and **Streamlit** to generate personalized stories based on user inputs. Users can select a genre, specify a theme, and describe characters to create a unique, AI-generated narrative. The project also evaluates the generated stories using the **ROUGE Score** to measure text summarization quality.

## 🚀 Features

✅ Personalized story generation based on user preferences (genre, theme, characters)  
✅ Uses **LLaMA 13B** for high-quality text generation  
✅ **Streamlit UI** for interactive and user-friendly experience  
✅ **ROUGE Score Evaluation** to assess text quality  
✅ Scalable and adaptable for various storytelling applications  

## 📌 Installation

1️⃣ Clone the repository:  
```bash
git clone https://github.com/Dhanushshruthi/story-generation.git
cd ai-storybook
```
2️⃣ Install dependencies:  
```bash
pip install torch transformers streamlit rouge_score
```
3️⃣ Run the Streamlit app:  
```bash
streamlit run app.py
```

## 🎭 How It Works

1️⃣ User selects **Genre** (Fantasy, Sci-Fi, Mystery, Adventure)  
2️⃣ User enters a **Theme** for the story  
3️⃣ User describes the **Main Characters**  
4️⃣ LLaMA 13B generates a **personalized story** based on the inputs  
5️⃣ The generated story is evaluated using **ROUGE Score**  

## 🎯 Example Prompt & Output

### **Input**  
```plaintext
Genre: Fantasy
Theme: A hidden kingdom beneath the ocean
Characters: A young prince who discovers his lost heritage
```
### **Generated Story**  
```plaintext
Once upon a time, beneath the vast ocean waves, there lay a kingdom untouched by time. 
A young prince, unaware of his royal blood, lived among the surface dwellers, until one day...
```

## 📊 ROUGE Score Evaluation

The **ROUGE Score** is used to compare the AI-generated story with reference texts:  
```python
from rouge_score import rouge_scorer

scorer = rouge_scorer.RougeScorer(['rouge1', 'rouge2', 'rougeL'], use_stemmer=True)
scores = scorer.score(reference_text, generated_story)
print(scores)
```

## 🛠 Tech Stack

- **Python**
- **Hugging Face Transformers**
- **LLaMA 13B**
- **Torch**
- **Streamlit**
- **ROUGE Score Evaluation**

## 🎯 Future Enhancements

🔹 Add voice narration for generated stories  
🔹 Enable real-time collaborative storytelling  
🔹 Implement multi-turn interactions with AI  

## 📜 License

This project is licensed under the MIT License.
