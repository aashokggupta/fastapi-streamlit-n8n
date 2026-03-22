Steps to execue the project

1) Install n8n
Install Node.js: Download and install the LTS version from nodejs.org.
Install n8n: Open Command Prompt and run:
**npm install n8n -g**
Start n8n: Run the following command:
Bash : **n8n**
Access: **Open your browser to http://localhost:5678.**
2) Create venv with name mlflow-pipeline(optional)
3) Go to venv
4) Below command will install pandas library, streamlit, fastapi, mlflow, model library scikit-learn
**pip install pandas scikit-learn mlflow streamlit fastapi uvicorn**
5) Run this once pip insall completes **streamlit hello**
   Open Streamlit in browser : **http://localhost:8501/**
6) run generate_data.py
7) run train_model.py
8) run predict_api.py and test fastapi
   **python -m uvicorn predict_api:app --reload**
   **http://localhost:8000/predict?marketing_spend=4000&season=3&region=4**  
11) **streamlit run ./dashboard.py** and open streamlit
    **http://localhost:8501/**
12) Create workflow in n8n
    upload Sales Forecast AI Agent.json
    run webook **http://localhost:5678/webhook-test/sales-agent**
    execute all the workflows.

