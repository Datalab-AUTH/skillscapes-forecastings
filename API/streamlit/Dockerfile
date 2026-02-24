FROM python:3.14-alpine
WORKDIR /app
COPY requirements.txt /app/
RUN pip install -r /app/requirements.txt
COPY ./*.py /app
CMD streamlit run app.py --server.port=8501 --server.address=0.0.0.0 --server.enableCORS=false --server.enableXsrfProtection=false
