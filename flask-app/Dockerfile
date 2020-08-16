#Use Python Image
FROM python:latest

# Install apt dependencies
RUN apt update && apt install python3-pip
# Copy contents into image
Copy . .
# run pip dependencies
RUN pip3 install flask flask_sqlalchemy pymysql
# Expose correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT ["python3", "app.py"]
