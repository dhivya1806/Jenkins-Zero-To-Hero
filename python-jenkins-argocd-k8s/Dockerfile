FROM python:3
RUN pip install django==3.2

COPY . .

RUN python python-jenkins-argocd-k8s/manage.py migrate
EXPOSE 8000
CMD ["python","python-jenkins-argocd-k8s/manage.py","runserver","0.0.0.0:8000"]


