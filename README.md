# <p align=center> <a href="https://bongsikb.github.io/My-homepage/">🏡 Welcome to my home page 🏡</a>
<p align=center> It's a responsive website! ✨

## 📌 HTML & CSS

- `Flex box` 반응형
  - px & pt (절대단위)
  - `rem & em` (상대단위)
  - vw & vh (상대단위)
- Power of `<a>` tag
- Responsible Nav bar
  - `🍔 Hamburger Menu`
    - <a href="https://github.com/BongsikB/my-homepage#-hamburger-menu--java-script">📎 Hamburger menu JS </a>
  - Sticky menu bar
- Overflow
- Span + text stroke
- Gradient background
  - <a href="https://cssgradient.io/">📎 Gradient backgroud maker</a>
- CSS animation
  - Spin animation
  - Zoom in animation

## 📌 Java Script

- responsive Nav bar JS
- `🍔 Hamburger Menu`
- ⚒️ Comment & like function `👩‍💻In progress`

 <hr>

## 🔁 Flex box | 반응형 사이트 만들기

<a href="https://developer.mozilla.org/ko/docs/Web/CSS/flex">📎 Flex box MDN</a> 

스크린 리더의 사이즈에 맞춰 변화하는 반응형 사이트를 구축하였습니다.<br>
`disply: flex` 과 `rem` 를 사용하는 것이 중요합니다. <br>

<a href="https://www.daleseo.com/css-em-rem/">📎 단위설명 글 인용 </a> <br>

px과 pt는 절대 단위입니다. 화면의 사이즈가 변화하여도 값이 고정되어있기 때문에 반응형이 적용되지 않는 것을 확인하실 수 있습니다. <br>
이럴때 필요한 것은 `상대단위 : em, rem, % ,vh, vw ... ` 입니다.

> 아래 두가지 화면 사이즈에서 보여지는 저의 홈페이지 이미지 입니다. <br> `rem` 단위 사용을 추천합니다.

## 💡 Viewport

```
vw/vh: viewport width/height;
```

- 뷰포트는 현재 보고있는 컴퓨터그래픽스의 영역
- 뷰포트의 크기는 화면 크기에 따라 다름

### `vh : view height`

- 뷰 포트 높이에 근거 하여 작용
- 1vh는 view height의 1%

### `vw : view width`

- 뷰 포트 너비에 근거 하여 작용
- 1vh는 view width의 1%

### `rem` 👍

- `r`oot 속성값에 기반
- 상대단위
- 초심자에게 추천하는 단위
- 유지보수가 쉬움

```css
1rem = 16px
```

### `em`

- 상위 요소 속성값에 영향받음
- 상대단위
- 유지보수가 어려움

```css
body {
  max-width: 100vw; ✨
}

.main-page {
  display: flex;
  height: 45rem;
  overflow: hidden;
  flex-wrap: nowrap;
  align-content: normal;
  justify-content: space-around;
  align-items: center;
}
```

### 미디어 쿼리

미디어 쿼리를 사용하여 nav바의 사이즈와 형태를 설정하였습니다.

<a href="https://developer.mozilla.org/ko/docs/Learn/CSS/CSS_layout/Media_queries">📎 미디어쿼리 MDN</a>

```css
/*Simplest media query syntax*/
@media media-type and (media-feature-rule) {
  /* CSS rules go here */
}
```

```css
@media screen and (max-width: 768px) {
  /* screen 768px 이하(좁을)일 때*/
  .nav-links {
    width: 60%;
  }
}
```

## 🍔 Hamburger menu : html & css

세가지의 선이 햄버거와 비슷하여 붙은 이름입니다. <br>
html과 css는 생각보다 간단합니다.

```html
<div class="burger">
  <div class="line1"></div>
  <div class="line2"></div>
  <div class="line3"></div>
</div>
```

```css
.burger {
  display: none;
  cursor: pointer;
}
.burger div {
  width: 25px;
  height: 2px;
  background-color: black;
  margin: 5px;
  transition: all 0.3s ease;
}
```

## Sticky Nav

```css
position: sticky; ✨
top: 0; ✨
```

## Power of `<a>` tag

```html
<!-- 어디로든 문, <a> 태그-->
<a href="#"></a>
<!-- e.g. -->
<a href="#"> <img /> </a> 👍
```

## 🌈 Gradient background

매번 그라디언트 배경을 코드로 만든다는것 어렵기 때문에 <a href="https://cssgradient.io/">Gradient backgroud maker</a>를 사용합시다.

```css
background: linear-gradient(
  47deg,
  rgba(253, 248, 237, 1) 0%,
  rgba(253, 248, 237, 1) 50%,
  rgba(69, 219, 252, 1) 100%
);
```

## 🔄 Spin animate

```css
#circle {
  width: 12rem;
  animation: spin 10s infinite;
}

@keyframes spin {
  100% {
    transform: rotate(360deg);
  }
}
```

### Text stroke | Extra Tricks

```html
<h1>
  <!-- 문장의 특정 단어에 효과를 주고 싶다면 span을 사용합니다 -->
  console&#46;log<br />
  ("<span id="strok-t">해</span>답을 찾는<br />
  프론트엔드 개발자")<br />
  이다빈<span id="strok-t">입니다&#46;</span>
</h1>
```

## 🔍 Zoom in animation

```css
/*부모 요소에 overflow hidden을 넣어 줌이 될 때 영역 밖으로 나오지 않게 설정*/
.proj-thn1 {
  overflow: hidden;
}

#thumb {
  filter: grayscale(100%);
  transition: all 1.2s ease-in-out;
}
/* 호버되었을 때 filter 흑백에서 컬러로 전환*/
#thumb:hover {
  filter: grayscale(0%);
  transform: scale(1.1);
  /*스케일이 설정한 s초 동안 1.1배 확대 됨*/
}
```

```css
/* 스트로크의 두께, 색상을 지정합니다.*/
#strok-t {
  -webkit-text-stroke: 0.1rem black;
  -webkit-text-fill-color: transparent;
  color: rgb(0, 0, 0, 0);
}
```

<hr>

# 📌 Java Script

## 🍔 Hamburger menu : Java script

```java script
  const navSlide = () => {
  const burger = document.querySelector(".burger");
  //일치하는 element return
  const nav = document.querySelector(".nav-links");
  const navLinks = document.querySelectorAll(".nav-links li");
  //individual link import here
  //toggle nav
  burger.addEventListener("click", () => {
    nav.classList.toggle("nav-active");
    //.nav-active {transform: translateX(0%);}
    //X좌표값 0% 이동
    //Over flow hidden 해제시 오른쪽에 대기중임을 확인할 수 있음

    //Animate links
    navLinks.forEach((link, index) => {
      //list idex transform css @keyframes navlikfade
      //index for each list animation
      if (link.style.animation) {
        link.style.animation = ""; //'' > nothing
      } else {
        link.style.animation = `navLinkFade 0.5s ease forwards ${
          index / 7 + 0.3
        }s`;
        //`navLinkFade 0.5s` 우리가 이미 만들어놓은 기능을 불러옴
        //${} interpolate index % 7 delay
        // n + n을 추가하여 add initial delay
      }
    });
    //burger Animation
    burger.classList.toggle("toggle");
  });
};

navSlide();

```

```java script
//Comment function
console.log(comment function)
// 👩‍💻In progress
```

<hr>
출처:

- https://developer.mozilla.org/en-US/docs/Web/CSS/Viewport_concepts
- https://www.daleseo.com/css-em-rem/
- https://45royale.com/blog/convert-pixels-to-rems/
