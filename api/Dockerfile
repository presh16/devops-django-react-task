FROM python:3.6
WORKDIR /app
COPY . .
RUN pip install virtualenv 
RUN virtualenv env
RUN /bin/bash -c "source env/bin/activate"
RUN pip install -r requirements.txt
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
