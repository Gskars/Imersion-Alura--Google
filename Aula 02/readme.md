# 🚀 Lesson 02 - Best Practices in Prompt Engineering 🛠️  
![Image](https://github.com/user-attachments/assets/bb05f32e-2695-4473-a8cc-0b17f8e6cf69)

- 📌 **Today's Lesson:** We will learn prompt engineering techniques to optimize our work!  
- 🌟 **Relevance:** A new field in Science that is rapidly growing in the market.  
- 🧩 **Key Definition:** Prompt engineering is the practice of designing and optimizing instructions (Prompts) for Large Language Models (LLMs) to obtain more relevant, precise, and useful responses, facilitating insights extraction and problem-solving.  
- 🎯 **Golden Rule:** We need **absolute clarity** in instructions!  

---

## 🧪 **Example of Prompt Engineering Technique**  
> “🎓 **Act as a professional who is a reference in teaching programming logic using Python.**  
> - ✅ **Characteristics:** Teach with fluidity, objectivity, and patience.  
> - 📚 **Method:** Provide complete exercises for content retention when requested.  
> - 🌍 **Contextualization:** If the user is unfamiliar with something, explain it simply and place the situation in a real-world context.  
> **Do you understand your mission?**”  

---

## ⚠️ **Beware of Hallucinations!**  
![Image](https://github.com/user-attachments/assets/734961b0-db6a-4b29-93ff-a0f8050be41b)  
- 🤯 **Hallucination:** When the LLM's response deviates from the idea you projected to the AI.  
- 🔍 **Cause:** Lack of contextual clarity in the prompt.  

---

## 🔧 **Learned Techniques**  

**1. Zero-Shot Prompting 🎯:**  
The model responds **without prior examples**, relying solely on direct instructions.  

```markdown  
Example Prompt:
"What are the main causes of global warming?"

```  
**2. Few-Shot Prompting 📋:**  
Provide examples to guide the response pattern.
```markdown 
Example Prompt:
"Example 1: What is the capital of France? Answer: Paris  
Example 2: What is the capital of Japan? Answer: Tokyo  
Now, what is the capital of Germany?"  

```
**3. Few-Shot Chain-of-Thought Prompting 🤔➡️💡:**  
Show step-by-step reasoning in the examples.
```markdown 
*Example Prompt:*  
"Example 1: If 2 + 3 = 5 and 5 + 2 = 7, what is the next number?  
Thought: 5 + 2 = 7 → next number = 7 + 3 = **10**.  
Answer: 10.  

Example 2: If 10 ÷ 2 = 5 and 5 × 2 = 10, what is the next number?  
Thought: 5 × 2 = 10 → next number = 10 ÷ 2 = **5**.  
Answer: 5.  

Now, what is the next number after 8 + 4 = 12?"  

```
---

## 📊 Mermaid Diagram: Prompt Workflow: 

```mermaid
graph TD  
  A[Initial Prompt] --> B{Clarity?}  
  B -->|Yes| C[Apply Technique]  
  C --> D[Zero-Shot]  
  C --> E[Few-Shot]  
  C --> F[Chain-of-Thought]  
  D --> G[Response]  
  E --> G  
  F --> G  
  G --> H{Evaluation}  
  H -->|Hallucination| I[Refine Context]  
  H -->|Success| J[🎉 Ideal Result!]  
  I --> A  
