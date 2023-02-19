FROM python:3.6

WORKDIR /app

COPY ./SA_model_DEMO_AVG ./SA_model_DEMO_AVG

RUN pip install flask scikit-learn

CMD ["cd", "./SA_model_DEMO_AVG"]

CMD ["python", "SA_demo_AVG_final.py", "&", "sleep", "4", "|", "if", "grep", "-q", "'68.89 %'", ";", "then", "echo",
    "'Test1 passed'", ";", "else", "exit", "1", ";", "fi"]
    
CMD ["python", "SA_demo_AVG_final.py", "&", "sleep", "4", "|", "if", "grep", "-q", "'68.89 %'", ";", "then", "echo",
    "'Test1 passed'", ";", "else", "exit", "1", ";", "fi"]
    
    
