# README

안녕하세요 2020 동의대학교 김성희 교수님이 Ruby On Rails 강의 자료에 사용한 코드 입니다.

# 사용 환경
- 구름IDE
- Ubuntu 14.04 LTS, 
- Ruby 2.4.0
- rvm 1.29.1
- Rails 5.2.3
- Sinatra 1.4.7

# 배포 환경
- Heroku

# 사용한 RDBMS
- postgresql
-------------------------------------------------------------------------
# 폴더 별 강의 주차 참고자료(2주차 부터 진행됩니다.)

## 2주차, 3주차
    app
    ㄴ controllers 
          ㄴ application_controller.rb
          ㄴ tests_controller.rb
    ㄴ models 
          ㄴ test.rb 
    ㄴ views 
          ㄴ tests 
              ㄴ _form.html.erb 
              ㄴ _test.json.jbuilder 
              ㄴ edit.html.erb 
              ㄴ index.html.erb 
              ㄴ index.json.jbuilder 
              ㄴ new.html.erb 
              ㄴ show.html.erb 
              ㄴ show.json.jbuilder 
    ㄴ config
          ㄴ database.yml
          ㄴ routes.rb
    Gemfile
    
## 2주차 터미널 명령어 모음

### postgresql 설치 이후 구름IDE를 실행 할때마다 입력해야할 문구(postgresql 서버를 실행해야 합니다.)
<pre><code>
sudo service postgresql start
</code></pre>

### postgresql 환경 구축
<pre><code>
sudo apt-get update && sudo apt-get install -y libpq-dev
</code></pre>

### postgresql 설치
<pre><code>
sudo apt update && sudo apt install postgresql postgresql-contrib
</code></pre>

### postgresql 콘솔창 실행
<pre><code>
sudo -u postgres psql
</code></pre>

### postgresql 사용자 비밀번호 변경
<pre><code>
alter user postgres with password 'postgres';
</code></pre>

### postgresql 콘솔창 종료
<pre><code>
\q
</code></pre>

### name, age 데이터를 가진 test라는 이름의 scaffold 생성
<pre><code>
rails g scaffold test name:string age:integer
</code></pre>

### 생성한 scaffold 확정 & 테이블 생성
<pre><code>
rake db:migrate
</code></pre>


## 3주차 터미널 명령어 모음

### 생성된 경로정보 확인 명령어
<pre><code>
rake routes
</code></pre>

### DB 조작 명령어 모음
<pre><code>
#확정되지 않은 migration 파일 확정(테이블 생성)
rake db:migrate

#모든 migration 파일 롤백 및 DB 삭제
rake db:drop

#새로운 db 생성(drop 이후 또는 db 종류를 변경하였을때 사용)
rake db:create

#모든 migration 파일만 롤백하고 다시 migration(drop과 다르게 변경된 migration을 반영하지 않고 단순히 db내용을 다 삭제후 migration 실행)
rake db:reset
</code></pre>
    
#### 4주차  
    app
    ㄴ controllers 
          ㄴ application_controller.rb
          ㄴ tests_controller.rb
    ㄴ models 
          ㄴ test.rb 
    ㄴ views 
          ㄴ tests 
              ㄴ _form.html.erb 
              ㄴ _test.json.jbuilder 
              ㄴ edit.html.erb 
              ㄴ index.html.erb 
              ㄴ index.json.jbuilder 
              ㄴ new.html.erb 
              ㄴ show.html.erb 
              ㄴ show.json.jbuilder 
    ㄴ config
          ㄴ database.yml
          ㄴ routes.rb
    Gemfile
    
    
      
   
  
