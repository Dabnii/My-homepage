# <p align=center> <a href="https://dabnii.github.io/My-homepage/">π‘ Welcome to my home page π‘</a>
<p align=center> It's a responsive website! β¨

## π HTML & CSS

- `Flex box` λ°μν
  - px & pt (μ λλ¨μ)
  - `rem & em` (μλλ¨μ)
  - vw & vh (μλλ¨μ)
- Power of `<a>` tag
- Responsible Nav bar
  - `π Hamburger Menu`
    - <a href="https://github.com/BongsikB/my-homepage#-hamburger-menu--java-script">π Hamburger menu JS </a>
  - Sticky menu bar
- Overflow
- Span + text stroke
- Gradient background
  - <a href="https://cssgradient.io/">π Gradient backgroud maker</a>
- CSS animation
  - Spin animation
  - Zoom in animation

## π Java Script

- responsive Nav bar JS
- `π Hamburger Menu`
- βοΈ Comment & like function `π©βπ»In progress`

 <hr>

## π Flex box | λ°μν μ¬μ΄νΈ λ§λ€κΈ°

<a href="https://developer.mozilla.org/ko/docs/Web/CSS/flex">π Flex box MDN</a> 

μ€ν¬λ¦° λ¦¬λμ μ¬μ΄μ¦μ λ§μΆ° λ³ννλ λ°μν μ¬μ΄νΈλ₯Ό κ΅¬μΆνμμ΅λλ€.<br>
`disply: flex` κ³Ό `rem` λ₯Ό μ¬μ©νλ κ²μ΄ μ€μν©λλ€. <br>

<a href="https://www.daleseo.com/css-em-rem/">π λ¨μμ€λͺ κΈ μΈμ© </a> <br>

pxκ³Ό ptλ μ λ λ¨μμλλ€. νλ©΄μ μ¬μ΄μ¦κ° λ³ννμ¬λ κ°μ΄ κ³ μ λμ΄μκΈ° λλ¬Έμ λ°μνμ΄ μ μ©λμ§ μλ κ²μ νμΈνμ€ μ μμ΅λλ€. <br>
μ΄λ΄λ νμν κ²μ `μλλ¨μ : em, rem, % ,vh, vw ... ` μλλ€.

> μλ λκ°μ§ νλ©΄ μ¬μ΄μ¦μμ λ³΄μ¬μ§λ μ μ ννμ΄μ§ μ΄λ―Έμ§ μλλ€. <br> `rem` λ¨μ μ¬μ©μ μΆμ²ν©λλ€.

## π‘ Viewport

```
vw/vh: viewport width/height;
```

- λ·°ν¬νΈλ νμ¬ λ³΄κ³ μλ μ»΄ν¨ν°κ·Έλν½μ€μ μμ­
- λ·°ν¬νΈμ ν¬κΈ°λ νλ©΄ ν¬κΈ°μ λ°λΌ λ€λ¦

### `vh : view height`

- λ·° ν¬νΈ λμ΄μ κ·Όκ±° νμ¬ μμ©
- 1vhλ view heightμ 1%

### `vw : view width`

- λ·° ν¬νΈ λλΉμ κ·Όκ±° νμ¬ μμ©
- 1vhλ view widthμ 1%

### `rem` π

- `r`oot μμ±κ°μ κΈ°λ°
- μλλ¨μ
- μ΄μ¬μμκ² μΆμ²νλ λ¨μ
- μ μ§λ³΄μκ° μ¬μ

```css
1rem = 16px
```

### `em`

- μμ μμ μμ±κ°μ μν₯λ°μ
- μλλ¨μ
- μ μ§λ³΄μκ° μ΄λ €μ

```css
body {
  max-width: 100vw; β¨
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

### λ―Έλμ΄ μΏΌλ¦¬

λ―Έλμ΄ μΏΌλ¦¬λ₯Ό μ¬μ©νμ¬ navλ°μ μ¬μ΄μ¦μ ννλ₯Ό μ€μ νμμ΅λλ€.

<a href="https://developer.mozilla.org/ko/docs/Learn/CSS/CSS_layout/Media_queries">π λ―Έλμ΄μΏΌλ¦¬ MDN</a>

```css
/*Simplest media query syntax*/
@media media-type and (media-feature-rule) {
  /* CSS rules go here */
}
```

```css
@media screen and (max-width: 768px) {
  /* screen 768px μ΄ν(μ’μ)μΌ λ*/
  .nav-links {
    width: 60%;
  }
}
```

## π Hamburger menu : html & css

μΈκ°μ§μ μ μ΄ νλ²κ±°μ λΉμ·νμ¬ λΆμ μ΄λ¦μλλ€. <br>
htmlκ³Ό cssλ μκ°λ³΄λ€ κ°λ¨ν©λλ€.

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
position: sticky; β¨
top: 0; β¨
```

## Power of `<a>` tag

```html
<!-- μ΄λλ‘λ  λ¬Έ, <a> νκ·Έ-->
<a href="#"></a>
<!-- e.g. -->
<a href="#"> <img /> </a> π
```

## π Gradient background

λ§€λ² κ·ΈλΌλμΈνΈ λ°°κ²½μ μ½λλ‘ λ§λ λ€λκ² μ΄λ ΅κΈ° λλ¬Έμ <a href="https://cssgradient.io/">Gradient backgroud maker</a>λ₯Ό μ¬μ©ν©μλ€.

```css
background: linear-gradient(
  47deg,
  rgba(253, 248, 237, 1) 0%,
  rgba(253, 248, 237, 1) 50%,
  rgba(69, 219, 252, 1) 100%
);
```

## π Spin animate

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
  <!-- λ¬Έμ₯μ νΉμ  λ¨μ΄μ ν¨κ³Όλ₯Ό μ£Όκ³  μΆλ€λ©΄ spanμ μ¬μ©ν©λλ€ -->
  console&#46;log<br />
  ("<span id="strok-t">ν΄</span>λ΅μ μ°Ύλ<br />
  νλ‘ νΈμλ κ°λ°μ")<br />
  μ΄λ€λΉ<span id="strok-t">μλλ€&#46;</span>
</h1>
```

## π Zoom in animation

```css
/*λΆλͺ¨ μμμ overflow hiddenμ λ£μ΄ μ€μ΄ λ  λ μμ­ λ°μΌλ‘ λμ€μ§ μκ² μ€μ */
.proj-thn1 {
  overflow: hidden;
}

#thumb {
  filter: grayscale(100%);
  transition: all 1.2s ease-in-out;
}
/* νΈλ²λμμ λ filter νλ°±μμ μ»¬λ¬λ‘ μ ν*/
#thumb:hover {
  filter: grayscale(0%);
  transform: scale(1.1);
  /*μ€μΌμΌμ΄ μ€μ ν sμ΄ λμ 1.1λ°° νλ λ¨*/
}
```

```css
/* μ€νΈλ‘ν¬μ λκ», μμμ μ§μ ν©λλ€.*/
#strok-t {
  -webkit-text-stroke: 0.1rem black;
  -webkit-text-fill-color: transparent;
  color: rgb(0, 0, 0, 0);
}
```

<hr>

# π Java Script

## π Hamburger menu : Java script

```java script
  const navSlide = () => {
  const burger = document.querySelector(".burger");
  //μΌμΉνλ element return
  const nav = document.querySelector(".nav-links");
  const navLinks = document.querySelectorAll(".nav-links li");
  //individual link import here
  //toggle nav
  burger.addEventListener("click", () => {
    nav.classList.toggle("nav-active");
    //.nav-active {transform: translateX(0%);}
    //Xμ’νκ° 0% μ΄λ
    //Over flow hidden ν΄μ μ μ€λ₯Έμͺ½μ λκΈ°μ€μμ νμΈν  μ μμ

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
        //`navLinkFade 0.5s` μ°λ¦¬κ° μ΄λ―Έ λ§λ€μ΄λμ κΈ°λ₯μ λΆλ¬μ΄
        //${} interpolate index % 7 delay
        // n + nμ μΆκ°νμ¬ add initial delay
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
// π©βπ»In progress
```

<hr>
μΆμ²:

- https://developer.mozilla.org/en-US/docs/Web/CSS/Viewport_concepts
- https://www.daleseo.com/css-em-rem/
- https://45royale.com/blog/convert-pixels-to-rems/
