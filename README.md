# armrating

---
Project for armwrestling competitions

---
### Create VENV (Optional)
    virtualenv venv
####
    venv\Scripts\activate.bat
## Starting project with Docker
    cd docker
####
    docker-compose build
####
    docker-compose up back_end
####
####Project starts at 127.0.0.1:5000
## Starting project without Docker
    pip install -r requirements.txt
####
    python manage.py migrate
####
    python manage.py runserver
####Project starts at 127.0.0.1:8000