FROM python:3
WORKDIR /usr/src/app
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
RUN python -m spacy download en_core_web_sm
#RUN pip install ./en_core_web_sm-2.3.0.tar.gz
CMD ["python", "app.py"]