# USing Official Image
FROM python:3.10-slim 

#Set-Working Directory 
WORKDIR /app

#Copy requirements file first to leverage Docker cache
COPY requirements.txt .

#Install Pyrthone Dependencies
RUN pip install --no-cache-dir -r requirements.txt

#Copy app source code
COPY . .

#EXpose the Flask default Port
EXPOSE 5000

#RUn app
CMD ["python", "app.py"]




