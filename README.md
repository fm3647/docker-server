# 훈민정음 커뮤니티 
### Hun-Min-Jeong-Eum Project
- server: Docker 
- backend: Django(python) 
- frontend: Vue

***

## 설치가이드

### Backend프로젝트
```commandline
cd backend
```
### Django 프로젝트를 생성
```commandline
:: ./backend
django-admin startproject config .
django-admin startapp 앱 이름
```

### Django admin에 스타일 적용안되는 문제
```pycon
STATIC_URL = 'static/'
STATIC_ROOT = os.path.join(BASE_DIR, 'static')
```
```commandline
:: ./backend
python manage.py collectstatic
```

### Docker로 Builld
```commandline
:: ./
docker-compose up -d --build
```

### migrate 명령어

```commandline
:: ./
python3 manage.py makemigrations
python3 manage.py migrate
```

### 관리자 생성
```commandline
:: ./backend
python3 manage.py createsuperuser
```
