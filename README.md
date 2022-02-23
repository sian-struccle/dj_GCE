# django + GCEプロジェクトの起動方法

## 前提条件
"""
1, python環境がある
2, docker環境がある
"""

## clone & cd
"""
git clone https://github.com/sian-struccle/dj_GCE.git
cd dj_GCE
"""

## Djangoアプリ起動（docker）
"""
docker-compose up -d --build
"""

## コンテナに入り、migrate
"""
docker-compose exec web sh
python manage.py migrate
"""

## superuser作成
"""
python manage.py createsuperuser
"""

