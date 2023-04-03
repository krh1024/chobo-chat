<h1>라라벨 + 이너시아 뷰 스타터</h1>

1. 아파치서버를 사용할 때, 라라벨은 반드시 sudo a2enmod rewrite 로 짧은 주소를 설정해줘야 한다.
2. npm run watch 를 해줘야 vue가 수정되는걸 웹으로 확인할 수 있다.
3. 이 문서는 본인이 직접 작성하였다.

<h2>설치방법</h2>

<ol>
    <li> git pull origin https://github.com/krh1024/laravel8_vue3.git</li>
    <li> composer install</li>
    <li> npm install</li>
    <li> cp .env.example .env  -> 치고나서 .env 에 DB 넣어줘야함</li>
    <li> storage 폴더 권한 설정해줘야함(777)</li>
    <li> php artisan key:generate</li>
    <li> php artisan migrate</li>
    <li> 접속!</li>
<ol>

<h2>이너시아 없다고 할 때, vite 모듈이 없다고 할 때</h2>
<p>이 때는 라라벨이 8인데 jetstream 의 버전이 라라벨 9로 맞춰서 설치될 때이다.</p>
<ol>
    <li> composer require laravel/jetstream:2.7.0</li>
    <li> php artisan jetstream:install inertia</li>
    <li> php artisan migrate</li>
    <li> npm install && npm run watch</li>        
</ol>
