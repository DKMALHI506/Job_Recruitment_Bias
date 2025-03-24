# Job_Recruitment_Bias

# Job Recruitment AI Bias Project

## What’s This About?
I built an AI model to predict who gets "hired" based on the UCI Adult Income dataset.
The idea was to see if it’s fair does it favor men over women or certain races?
I used Random Forest and SHAP to dig into it, then tried fixing any bias I found. 
It’s a cool mix of coding and real-world impact!

## Files
Recruitment_bias.ipynb`: The main code loads data, trains the model, checks bias, and plots stuff.
Adult.data`: The dataset I used (from UCI).
Requirements.txt`: Libraries  need to run it.
Bias_plot.png`: A bar chart I saved showing hire rates before and after my fix.

## How to Run It
1. Install stuff from `requirements.txt` (`pip install -r requirements.txt`).
2. Open `recruitment_bias.ipynb` in Jupyter Notebook.
3. Make sure `adult.data` is in the same folder.
4. Run all cells takes a few minutes, especially the SHAP part!

## What I Got
- Model accuracy: 0.8456183003646812% at first.
- Found males were “hired” more (1.4x vs females) yikes!
- After dropping ‘sex’ from the data, bias dropped to 1.1x, accuracy still ~83%.
- SHAP showed education and gender were big drivers—check the plot in the notebook.

![image](https://github.com/user-attachments/assets/3889e190-a840-4756-865e-6935ee5b5eb7)


## Why It Matters
This ties into AI fairness, which is huge for jobs and society.
I learned a ton about how models can mess up without us noticing perfect for the PSL Master’s vibe.
