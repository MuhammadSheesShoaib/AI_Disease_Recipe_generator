# Disease-Specific Recipe Generator 🍲

This project is an AI-powered Recipe Generator built to help people with specific health conditions.  
Given a disease (like diabetes, heart disease, obesity, etc.), the model generates a **tasty and healthy recipe**, along with:
- Ingredients
- Step-by-step instructions
- Tips for healthy eating
- Foods to avoid

---

## Why This Project? 🎯

Healthy eating is crucial for managing diseases, but it’s often hard to find recipes tailored for specific medical conditions.  
I wanted to build a smart system that can instantly generate disease-safe recipes while also guiding the user about important food restrictions.

---

## How I Built This Project 🛠️

- **Dataset Categories**:  
  - I curated a custom dataset containing 12 disease categories:
    - Celiac Disease
    - Chronic Kidney Disease
    - Diabetes
    - Egg Allergy
    - Fatty Liver
    - Heart Disease
    - High Blood Pressure
    - High Cholesterol
    - Liver Disease
    - Milk Allergy
    - Obesity
    - Wheat Allergy
  
- **Model Training**:  
  - Fine-tuned a mistralai/Mistral-7B-v0.1 model on disease-specific recipe instructions.
  - The training was done over multiple steps to ensure quality and relevance.

## Dataset 📚

- The dataset used for training is **custom-built**.
- I manually **collected authentic data from trusted resources on the web** about dietary guidelines for different diseases.
- After collecting the data, I used the **Mistral 7B model** via **Together AI API** to **generate conversational recipe responses**.
- The collected data was used as **instructions** for the Mistral model to create natural, user-friendly, and medically accurate recipe responses.
- The final conversational dataset is available inside the `/Disease_Recipe_Data/` folder.
- Alternatively, you can load dataset directly: load_dataset("Shees7/Disease-recipes-conversational-data")
