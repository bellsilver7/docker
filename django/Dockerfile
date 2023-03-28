# 이미지와 버전 명시
FROM python:3.11

# 프로젝트 경로 설정
WORKDIR /app

# 장고 모듈 설치
RUN pip install django

# 패키지 관리 파일 생성
RUN pip freeze > requirements.txt

# 장고 프로젝트 생성
RUN django-admin startproject config .

# 포트 설정
EXPOSE 8000

# 서버 실행
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]