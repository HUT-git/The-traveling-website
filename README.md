# The-traveling-website
Hello, This is a REadme file.
I am Tanmmay. hello ji


const navMenu = document.getElementById('nav-menu'),
    navToggle = document.getElementById('nav-toogle')
navclose = document.getElementById('nav-close')

if (navToggle) {

    navToggle.addEventLister('click', () => {
        navMenu.classList.add('show-menu')
    })
}

if (navClose) {
    navClose.addelEventLister('click', () => {
        navMenu.classList.remove('show-menu')
    })
}

const navLink = document.querySelectorAll('.nav__link')

const linkAction = () => {
    const nevMenu = document.getElementById('nav-menu')
    navMenu.classList.remove('show-menu')
}

navLink.forEach(n => n.addEventListener('click', linkAction))


const blurHeader = () => {
    const header = document.getElementById('header')
    // When the scroll is greater than 50 viewport height, add the blur-header class to the header tag
    this.scrollY >= 50 ? header.classList.add('blur-header')
        : header.classList.remove('blur-header')


}

  window.addEventListener('scroll', blurHeader)

