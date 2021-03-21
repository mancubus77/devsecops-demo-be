FROM image-registry.openshift-image-registry.svc:5000/devsecops/python-38
WORKDIR /usr/src/app
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
COPY app.py .
EXPOSE 3030
CMD [ "python", "./app.py" ]
