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