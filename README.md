## 하이퍼 텍스트 마크업 언어 :  페이지 표시 마크업 언어


### <00_html.html>
- ! + tab : html 자동 완성
- 각각 opening tag, closing tag 의미 : <p>My cat is very grumpy</p>
- Attribute : a 태그 - 주소가 있어야 함 
- `<! -- <태그명 속성명1 = "속성값", 속성명2 = "속성값2"> 내용 </태그명> -->`

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>html</title>   
    </head>
    <body>
    
    </body>
</html>
```

- <strong>글자</strong> : 볼드 처리
- <ul></ul> : 순서가 있는  / <ol></ol> : 순서가 없는
- <a href="https://google.com">google</a> :  "안에 있는 주소로 이동"
- <img src="./hello.jpg" alt=""> : "이미지 보여줌" / 이미지는 닫는 태그 없음 !
- radio : 여러가지 선택지 중 한가지 고를 때 사용

### 01_form.html
```
    <form action="">
        <label for="title">Name: </label>
        <input type="text" id="title" name="title">
        <br>
        <label for="number">Age: </label>
        <input type="number" id="age" name="age"> 
        <br>
        <label for="email">email: </label>
        <input type="email" id="email" name="email">
        <input type="submit">
        <input type="color">
        <input type="button">
        <input type="checkbox" value="1">
        <input type="checkbox" value="2">
        <input type="checkbox" value="3">
        <input type="radio" value="1" name="num">     # num을 붙이면 세개 중 하나 선택 가능
        <input type="radio" value="2" name="num">
        <input type="radio" value="3" name="num">
    </form>  
```

```
<form action="">
        <div>
            <label for="name">Name: </label>
            <input type="text" name= "name" id="name">
        </div>
        <div>
            <label for="date"></label>
            <input type="date" name= "date" id="date">
        </div>
        <hr>
            <h3>샌드위치 선택</h3>
            <input type="radio" name="menu" value="egg">     # radio : 한가지 선택할 때 사용
            <label for="">에그마요</label>
            <input type="radio" name="menu" value="blt">
            <label for="">BLT</label>
        <hr>
                <h3>빵 사이즈</h3>
                <input type="number" min="15" max="30" step="15">

        <hr>
                <h3>빵 종류</h3>
                <select name="bread" id="">
                    <option value="honey">허니오트</option>
                    <option value="flat">플랫브래드</option>
                </select>

        <hr>
                <h3>야채</h3>
                <input type="checkbox" id="1" name="cu">
                <label for="1">오이</label>
                <input type="checkbox" id="2" name="to">
                <label for="2">토마토</label>
        <input type="submit">
    </form>
```

### 03_
- css 불러오는 방법 : 3가지

- 1) <h1 style="color: red">hello</h1>
- 2) <h2>world</h2>  head에서 스타일로 컬러 지정
- 3) <h3>hi</h3> head에서 <link rel="stylesheet" href="mycss.css">  
          

- class="b" : 여러개의 값을 불러올 때 
- id : id의 우선 순위가 더 높음.


- ol > li.a {
    font-size: 10pt;   # 지정해서 폰트 사이즈 정해줌.
}

#### 
- copy selectors

- div {
    display: inline;  # inline은 자기가 가진 영역만큼만 데이터를 가짐 
}                        
-  <div>hello</div>     # div 블록 자체에 대한 데이터를 가짐 
    <p>hello</p>                   



#### 
- contencs : 제일 안쪽
- border : 테두리
- padding : 컨텐츠와 테두리의 중간
- margin : 액자와 액자 사이 공간 


####
```
#pond {
  display: flex; 

justify-content:flex-end;    # 오른쪽 정렬
justify-content:space-between; # 요소들을 동일한 간격을 둠.
justify-content:space-around; # 요소들 주위에 동일한 간격
}


align-items: flex-start: 요소들을 컨테이너의 꼭대기로 정렬합니다.
align-items:flex-end: 요소들을 컨테이너의 바닥으로 정렬합니다.
align-items:center: 요소들을 컨테이너의 세로선 상의 가운데로 정렬합니다.
align-items:baseline: 요소들을 컨테이너의 시작 위치에 정렬합니다.
align-items:stretch: 요소들을 컨테이너에 맞도록 늘립니다.
```

###
- 메인축 : 왼 -> 오
- 보조축 : 위 -> 아래

row: 요소들을 텍스트의 방향과 동일하게 정렬합니다.
row-reverse: 요소들을 텍스트의 반대 방향으로 정렬합니다.
column: 요소들을 위에서 아래로 정렬합니다.
column-reverse: 요소들을 아래에서 위로 정렬합니다.

order : 1 오른쪽정렬
order : -1 왼쪽 정렬

### 04_bootstrap.html

#### 0. 
- head 끝나기 전 : <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">

- body 끝나기 전 : 자바 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>


- 색깔 지정 : text-danger, text-warning, text-primary 등등 
    - 배경 색 지정 : bg-primary
- 명도 조절 : text-opacity-50
- 테두리 설정 : border
    - border-dark 
    - border-3 
    - rounded (모서리 둥글게) 

- grid 크기 지정 : 모니터에 보여지는 
xs
<576px	sm
≥576px	md
≥768px	lg
≥992px	xl
≥1200px	xxl


#### 99_practice
- 부트 스트랩 불러오기 (download)
- navbar : 상단 버튼 
- card : 
