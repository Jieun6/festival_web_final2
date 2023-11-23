# README.md

## 실행순서

### `npm install`

'npm install' 명령을 통해 package.json을 참조하여 필요한 라이브러리를 node_modules디렉토리에 설치합니다.

### `npm start`

`npm start` 명령을 통해 프로젝트를 'http://localhost:3000'의 주소로 실행합니다.

    npm install
    npm start

## 프로젝트 구성

### 메인페이지

메인페이지는 'http://localhost:3000/'으로 라우팅되어 있습니다.
메인페이지에서는 오늘 진행중인 축제정보와 인기있는 축제정보를 확인할 수 있습니다.
또한 검색기능을 통해 축제를 검색하거나 원하는 축제정보를 바로 확인할 수 있습니다.

### 지역축제페이지

지역축제 페이지는 'http://localhost:3000/CountryDetail'으로 라우팅되어 있습니다.
지역축제 페이지에서는 지역별로 분류된 다양한 축제정보를 확인할 수 있습니다.
또한 지역별로 진행되는 축제 중에서도 인기있는 축제들과 진행중인 축제를 확인할 수 있습니다.
주어진 캘린더를 통해 원하는 날짜에 진행중인 지역축제를 확인할 수 있습니다.

### 축제 상세페이지

축제 상세페이지는 'http://localhost:3000/festival_detail/축제ID'로 라우팅되어 있습니다.
메인페이지/지역축제페이지/검색페이지/테마페이지 등에서 하나의 축제를 클릭하면 출력되는 페이지입니다.
해당하는 축제에 대한 세부적인 정보외에도 이미지정보와 카카오맵을 통한 지리정보를 확인할 수 있습니다.

### 검색페이지

축제 상세페이지는 'http://localhost:3000/SearchList'로 라우팅되어 있습니다.
검색페이지에서는 검색어를 통해 해당하는 축제정보를 확인할 수 있습니다.
검색결과로 나온 축제들은 지역별로 필터링이 가능합니다.

### 테마페이지

축제  테마 페이지는 'http://localhost:3000/tabPrint'로 라우팅되어 있습니다.
테마 페이지에서는 사용자가 관심있는 테마별로 축제 추천 서비스를 받을 수 있습니다.

구현 세부사항

탭에 적힌 각 주제에 알맞는 데이터들을 출력하여 추천해주는 서비스입니다. 
탭 종류: 야경, 새해, 먹거리, 사계절(봄, 여름, 가을, 겨울)
탭 내용: 주제와 관련된 해시태그
기능: 해시태그와 축제 이름이 겹치는 데이터들을 출력 

데이터 출력: 마우스 포인터가 올라가면 세부위치 정보가 포스터 위에 오버레이되며 포스터를 클릭하면 해당 축제의 상세 정보 페이지로 이동

