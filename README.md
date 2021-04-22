## 0422
### css1

``` *{margin: 0px; padding: 0px;}
ul{list-style: none;} /* 리스트 앞에 .  제거*/
a{text-decoration: none;} /* 링크에 밑줄  제거*/
 
header{
    width: 800px; /*메인 이미지의 너비 사이즈와 같음*/
    height: 95px;
    background-color: #2d3a4b;
 
    /* header 안에 요소들을 모두 absolute 포지션으로 배치할 것이라서 */
    /* absolute 요소가 header의 좌상단을 기준으로 하려면 */
    /* header의 position이 relative 여야만 함 */
    position: relative;
}
 
/* 제목영역안에 있는 메인 로고 이미지 위치 지정 */
#logo{
    position: absolute;
    top: 30px;
    left: 30px;
 
}
 
/* 제목영역안에 오른쪽 상단에 top_menu 배치 */
#top_menu{
    position: absolute;
    top: 20px;
    right: 10px;
    color: white;
}
 
/* top_menu a의 글씨 하얀색으로 */
#top_menu a{color: white;}
 
/* 헤더 영역안에 네비게이션 메뉴 배치 */
nav{
    position: absolute;
    bottom: 10px;
    left: 220px;
    font-size: 16px;
}
 
nav li{
    display: inline;
    margin-left: 30px;
}
 
nav li a{color: white;}
 
#content #banner li{
    border-bottom: 1px solid gray;
    display: inline;
    
}

#content #banner li a{
    display: inline;
    text-align: center;
}
 
/* footer 영역 */
footer{
    width: 800px; /*헤더와 같은 사이즈*/
    height: 90px;
    margin-top: 20px;
    text-align: center;
    background-color: #f1f1f1;
}
 
/* 전체 페이지가 가운데로 오도록 */
#page{width: 820px; margin: 0px auto;}

```

### css2

```

@charset "EUC-KR";
*{margin: 0; padding: 0;}
ul{list-style: none;}
a{text-decoration: none;}
 
header{
    width: 100%;
    background-color: #2d3a4b;
    position: relative;
}
 
#log{
    padding-top: 30px;
    padding-left: 30px;
 
}
 
#top_menu{
    position: absolute;
    right: 10px;
    top: 20px;
    color: white;
}
#top_menu a{color: white;font-size: 14px;}
 
nav{
    border-top: 1px solid white;
    border-bottom: 1px solid white;
    margin-top: 10px;
}
 
nav li{
    line-height: 3em;
    border-bottom: 1px solid #223344;
}
 
nav li a{
    color: white;
    display: block;
    text-align: center;
}
 
nav li a:hover{
    background-color: white;
    color: black;
}
 
#content #main img{ width: 100%; border: 1px solid gray;}
 
#content #banner li{
    border-bottom: 1px solid gray;
}

#content #banner li a{
	width : 200px;
	height : 90px;
    display: flex;
    justify-content:space-between;
    text-align: center;
}
 
footer{padding: 0px 10px;}
footer img{width: 100%;}

```