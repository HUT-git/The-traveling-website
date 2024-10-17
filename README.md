# The-traveling-website
Hello, This is a REadme file.
I am Tanmmay. hello ji

@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@500;600&family=Poppins:wght@400;500&display=swap");


:root {
  --header-height: 3.5rem;


  --title-color: hsl(0, 0%, 95%);
  --text-color: hsl(0, 0%, 70%);
  --text-color-light: hsl(0, 0%, 60%);
  --body-color: hsl(0, 0%, 0%);
  --container-color: hsl(0, 0%, 8%);



  --body-font: "Poppins", sans-serif;
  --second-font: "Montserrat", sans-serif;
  --biggest-font-size: 2.75rem;
  --h1-font-size: 1.5rem;
  --h2-font-size: 1.25rem;
  --h3-font-size: 1rem;
  --normal-font-size: .938rem;
  --small-font-size: .813rem;
  --smaller-font-size: .75rem;


  --font-regular: 400;
  --font-medium: 500;
  --font-semi-bold: 600;


  --z-tooltip: 10;
  --z-fixed: 100;
}



@media screen and (min-width: 1152px) {
  :root {
    --biggest-font-size: 5.5rem;
    --h1-font-size: 2.5rem;
    --h2-font-size: 1.5rem;
    --h3-font-size: 1.25rem;
    --normal-font-size: 1rem;
    --small-font-size: .875rem;
    --smaller-font-size: .813rem;
  }
}


* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

html {
  scroll-behavior: smooth;
}

body,
button,
input {
  font-family: var(--body-font);
  font-size: var(--normal-font-size);
  color: var(--text-color);
}

body {
  background-color: var(--body-color);
}

button,
input {
  outline: none;
  border: none;
}

h1,
h2,
h3,
h4 {
  color: var(--title-color);
  font-family: var(--second-font);
  font-weight: var(--font-semi-bold);
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}

img {
  display: block;
  max-width: 100%;
  height: auto;
}


.container {
  max-width: 1120px;
  margin-inline: 1.5rem;
}

.grid {
  display: grid;
  gap: 1.5rem;
}

.section {
  padding-block: 5rem 1rem;
}

.section__title {
  text-align: center;
  font-size: var(--h1-font-size);
  margin-bottom: 1.5rem;
}

.main {
  overflow: hidden;
}


.header {
  position: fixed;
  width: 100%;
  background-color: transparent;
  top: 0;
  left: 0;
  z-index: var(--z-fixed);
}

.nav {
  height: var(--header-height);
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.nav__logo {
  color: var(--title-color);
  font-family: var(--second-font);
  font-weight: var(--font-semi-bold);

}

.nav__toogle,
nav__close {
  display: flex;
  font-size: 1.25rem;
  color: var(--title-color);
  cursor: pointer;

}

@media screen and(max-width: 1023px) {
  .nav__menu {
    position: fixed;
    top: -100%;
    left: 0;
    background-color: hsla(0, 0%, 0%, .3);
    width: 100%;
    padding-block: 4rem;
    backdrop-filter: blur(24px);
    -webkit-backdrop-filter: blur(24px);
    transition: top .4s;
  }
}

.nav__list {
  text-align: center;
  display: flex;
  flex-direction: column;
  row-gap: 2.5rem;
}

.nav__link {
  color: var(--title-color);
  font-family: var(--second-font);
  font-weight: var(--font-medium);
}

.nav__close {
  position: absolute;
  top: 1rem;
  right: 1.5rem;

}

.show-menu {
  top: 0;
}

.blur-header::after {
  content: '';
  position: absolute;
  width: 1000%;
  height: 100%;
  background-color: hsla(0, 0%, 0%, .3);
  backdrop-filter: blur(24px);
  -webkit-backdrop-filter: blur(24px);
  top: 0;
  left: 0;
  z-index: -1;




}

.home {
  position: relative;
}

.home__bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 750px;
  object-position: center;
}

.home__shadow {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 800px;
  background: linear-gradient(180deg,
      hsla(0, 0%, 0%, 0) 58%,
      hsl(0, 0%, 0)78%);

}

.home__container {
  position: relative;
  padding-top: 3rem;
}

.home__data {
  text-align: center;

}

.home__subtitle {
  font-size: var(--h3-font-size);
  margin-bottom: .5rem;
}

.home__title {

  font-size: var(--biggest-font-size);
  margin-bottom: 1rem;
}

.home__description {
  margin-bottom: 2rem;
  color: var(--title-color);

}

.home__card {
  position: relative;
  overflow: hidden;

}

.home__card-img {
  transition: tranform .4s;

}

.home__card-shadow {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  background: linear-gradient(180deg,
      hsla(0, 0%, 0%, 0) 50%,
      hsl(0, 0%, 0%, 0)125%);

}

.home__card-title {
  position: absolute;
  left: 1rem;
  bottom: 1rem;
  font-size: var(--h3-font-size);
  z-index: 1;

}

.home__card:hover .home__card-img {
  transform: scale(1.2);
}

.button {
  background-color: hsla(0, 0%, 100%, .2);
  padding: 1.25rem 1.5rem;
  color: var(--title-color);
  display: inline-flex;
  align-items: center;
  column-gap: .5rem;
  font-family: var(--second-font);
  font-weight: var(--font-semi-bold);
  backdrop-filter: blur(24px);
  -webkit-backdrop-filter: blur(24px);
}

.button i {
  font-size: 1.25rem;
  transition: transform .4s;
  font-weight: initial;
}

.button:hover {
  transform: translateX(.25rem);
}

.about__container {
  row-gap: 3rem;

}

.about__data {
  text-align: center;

}

.about__description {
  margin-bottom: 2rem;
}

.about__image {
  position: relative;
  justify-self: center;
  overflow: hidden;
}

.about__img {
  width: 300px;
  transition: tranform .4s;


}

.about__shadow {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(180deg,
      hsla(0, 0%, 0%, 0)50%,
      hsl(0, 0%, 0%)125%);
}

.about__image:hover.about__img {
  transform: scale(1.2);
}

.popular__container {
  padding-top: 1.5rem;
  grid-template-columns: 240px;
  justify-content: center;
  row-gap: 2.rem;

}

.popular__image {
  position: relative;
  overflow: hidden;
  margin-bottom: 1rem;

}

.popular__img {
  transition: transform .4s;
}

.popular__shadow {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(180deg,
      hsla(0, 0%, 0%, 0)50%,
      hsl(0, 0%, 0%)125%);
}

.popular__title{
  font-size: var(--h3-font-size);
  margin-bottom: .5rem;
}
.popular__location{

  display: inline-flex;
  align-items: center;
  column-gap: .25rem;
  font-size: var(--small-font);
  font-family: var(--second-font);
  font-weight: 500;
}

.popular__image:hover .popular__img{
  transform: scale(1.2);
}


