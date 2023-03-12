FROM python:3.6

WORKDIR /app

COPY ./SA_model_DEMO_AVG ./SA_model_DEMO_AVG

RUN pip install flask scikit-learn

CMD (cd ./SA_model_DEMO_AVG/ && (python SA_demo_AVG_final.py & sleep 10) | if grep -q "68.89 %" ; then echo 'Test1 passed' ; fi) & (sleep 4 && (curl http://127.0.0.1:5000/ | if grep -q "Введите" ; then echo 'Test2 passed'; else exit 1; fi))
    
    
