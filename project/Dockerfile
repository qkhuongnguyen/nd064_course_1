FROM python:3.8
EXPOSE 3111

WORKDIR /app
COPY techtrends /app
COPY techtrends/requirements.txt /app
COPY techtrends/init_db.py /app
RUN pip install -r requirements.txt
RUN python init_db.py
CMD [ "python", "app.py" ]
