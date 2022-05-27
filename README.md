# 설치가이드

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
