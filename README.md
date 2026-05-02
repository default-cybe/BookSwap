<div align="center">
      <h1> <img src="https://raw.githubusercontent.com/default-cybe/BookSwap/main/static/img/BookSwap.png" width="80px"> <img src="https://indrashiluniversity.edu.in/images/IIF-SSIP%20Logo%20holo.png" width="80px"><br/>BookSwap</h1>
     </div>
<p align="center"> <a href="https://github.com/default-cybe" target="_blank"><img alt="" src="https://img.shields.io/badge/Website-EA4C89?style=normal&logo=dribbble&logoColor=white" style="vertical-align:center" /></a> <a href="https://twitter.com/default_yt_" target="_blank"><img alt="" src="https://img.shields.io/badge/Twitter-1DA1F2?style=normal&logo=twitter&logoColor=white" style="vertical-align:center" /></a> <a href="https://www.instagram.com/kaivalya_ahir" target="_blank"><img alt="" src="https://img.shields.io/badge/Instagram-E4405F?style=normal&logo=instagram&logoColor=white" style="vertical-align:center" /></a> <a href="https://www.linkedin.com/in/kaivalya-ahir/" target="_blank"><img alt="" src="https://img.shields.io/badge/LinkedIn-0077B5?style=normal&logo=linkedin&logoColor=white" style="vertical-align:center" /></a> </p>

# Description
BookSwap is a book-sharing web app written in Python with Django. You list the books you own, browse or search what everyone else has put up, and request to borrow something you want. When two people agree on a swap, a simple courier flow helps them arrange the hand-off.

It started life as our entry for the Student Start-up and Innovation Policy (SSIP) national hackathon. I've kept it around since as a portfolio piece.

# Tech Used
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![Bootstrap](https://img.shields.io/badge/bootstrap-%23563D7C.svg?style=for-the-badge&logo=bootstrap&logoColor=white)

# Prerequisites

You'll want Python 3 and pip, Git, and SQLite 3 installed before you start.

# Getting Started

Clone the repo and hop into the directory:

```bash
git clone https://github.com/default-cybe/BookSwap.git
cd BookSwap
```

Set up a virtual environment and activate it:

```bash
python -m venv venv
source venv/bin/activate      # on Windows: venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Copy the example env file and tweak the values for your setup:

```bash
cp .env.example .env
```

At the very least you'll need to set `DJANGO_SECRET_KEY` in `.env`. Django can generate one for you:

```bash
python -c "from django.core.management.utils import get_random_secret_key; print(get_random_secret_key())"
```

Run the migrations and start the dev server:

```bash
python manage.py migrate
python manage.py runserver
```

That's it. The app should be up at http://127.0.0.1:8000/.
