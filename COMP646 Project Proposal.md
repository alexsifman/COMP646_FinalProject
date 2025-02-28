**COMP646 Project Proposal: Recipe Generator from Food Images**  
Project Group 25 \- Alejandro Sifuentes, Alma Torres, Kelly Zeng, Lan Shui

**The Problem and Solution**  
Cooking is an essential part of daily life, but it’s a skill that takes a long time to master. For beginner chefs like us college students, cooking is impossible without a recipe. However, we often see dishes online or in a restaurant that look so appetizing, but we fail to successfully recreate these dishes from just seeing them alone. This project aims to develop a deep learning system that generates a recipe based on an input image of any dish. We will utilize computer vision to identify the dish and detect ingredients, and we will leverage natural language processing to either retrieve existing recipes or generate a new one. By combining computer vision and natural language processing, this AI system can provide users with instant, personalized recipe recommendations based on visual input.

**Technologies and Tools (assisted by ChatGPT 4o)**

* Data: use [Recipe1M+](https://im2recipe.csail.mit.edu/) and [Food-101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) (publicly available) for food images and recipe text  
* Food Classification:  identify the dish category from an image using a CNN-based model like EfficientNet or ResNet to classify dishes in varying lighting, angles, and styles  
* Ingredient Detection: identify and recognize ingredients from food images using object detection models like YOLO and Faster R-CNN   
* Recipe Retrieval: find the closest matching recipe from an existing dataset based on image analysis through models like BERT and CLIP  
* Recipe Generation: generate a recipe with cooking steps based on detected ingredients and the dish name using NLP models like T5, BART, or GPT-4  
* Web App Interface: provide an interface for real-time image to recipe conversion 

**Roadmap (rough 8 week timeline)**

* Week 1-2: Data Collection, Preprocessing, Exploratory Data Analysis  
  * Obtain access to data, explore what has been done similarly by Recipe1M+ and Food-101, download data, clean and preprocess data, conduct exploratory data analysis to analyze patterns and understand the distribution of recipe and dish categories  
* Week 3-4: Food Classification and Ingredient Recognition  
  * Train a food classification and a ingredient detection model, evaluate model performance   
* Week 5-6: Recipe Retrieval/Generation  
  * Implement a recipe retrieval model and evaluate or train a recipe generation model and evaluate depending on which one works better for the project  
* Week 7-8: Optimization and Interface Deployment   
  * Fine-tune and optimize models for better accuracy and build an interactive interface if time permits  
  * Evaluate model based on dish and ingredient prediction accuracy and text generation metrics, such as BLEU, ROUGE, perplexity, and human evaluation