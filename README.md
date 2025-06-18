# Django_2

## 초기 설정

```bash
# 1단계 -> Django 프로젝트 생성
django-admin.exe startproject myproject .

# 2단계 -> 어플리케이션 생성
python.exe ./manage.py startapp myapp

# 3단계 -> 애플리케이션 등록
settings.py의 INSTALLED_APPS에 'myapp' 추가

# 4단계 -> 모델 정의
myapp/models.py 에 테이블 생성

# 5단계 -> 데이터베이스 마이그레이션
python.exe ./manage.py makemigrations
python.exe ./manage.py migrate

# 6단계 -> 관리자 패널에 모델 등록
myapp/admin.py 에 admin.site.register([모델]) 추가

# 7단계 -> 수퍼 유저 생성
python manage.py createsuperuser

# 8단계 -> 서버 실행
python manage.py runserver

# 9단계 -> 관리자 화면에서 데이터 입력
localhost:8000/admin
```
