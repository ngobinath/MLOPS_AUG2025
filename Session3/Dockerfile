FROM python:3.9-slim

WORKDIR /app
# Update system packages to reduce vulnerabilities
RUN apt-get update && apt-get upgrade -y && apt-get clean
RUN pip install --no-cache-dir pandas numpy matplotlib seaborn scikit-learn joblib jupyter

COPY train.py .
CMD [ "python", "train.py" ]
