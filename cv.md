# rsschool-cv


# Yauheniya Prymerava


### Contact information:
-----------------
+ **Phone:** +375(29)132 54 33
+ **E-mail:** minsk1901masha@gmail.com
+ **GitHub:** [feminochka](https://github.com/feminochka)
+ **Linkedin:** [Евгения Примерова](https://www.linkedin.com/in/%D0%B5%D0%B2%D0%B3%D0%B5%D0%BD%D0%B8%D1%8F-%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D0%BE%D0%B2%D0%B0-0166b5b4/)
+ **discord-nik:** feminochka#8881

### About me:
----------------
I like study and get new knowledges and sometimes change my life. Therefore I finished course Python and continue learning in RS School for grow like front-end developer. I had rich experience to work in big company with big projects like engineer. Also I like doing sport (gym, snowboard, ski) and travelling.

### Skills:
----------------
1. HTML (basic)
2. CSS (basic)
3. Python (basic)
4. JavaScript (beginner)
4. Django (basic)
5. SQLite(basic)
6. Editors: VSCode, PyCharm

### Code examples:
-----------------
- ***Python:***
```
def disemvowel(string_):
    vow = ["a", "e", "i", "o", "u"]
    new_string = []

    for i in string_: 
        if i.lower() not in vow:
            new_string.append(i)

    return "".join(new_string)
```
- ***JavaScript:***

```
const prev = document.getElementById('btn-prev'),
    next = document.getElementById('btn-next'),
    slides = document.querySelectorAll('.slide'),
    dots = document.querySelectorAll('.dot');
let index = 0;

const activeSlide = n =>{
    for (slide of slides){
        slide.classList.remove('active');}
    slides[n].classList.add('active');
}

const activeDot = n => {
    for (dot of dots) {
        dot.classList.remove('active');
    }
    dots[n].classList.add('active');
}

const nextSlide = () =>{
    if(index == slides.length - 1){
        index = 0;
        prepareCurrentSlide(index);
    }else{
        index++;
        prepareCurrentSlide(index);
    }
}

const prevSlide = () =>{
    if(index == 0){
        index = slides.length - 1;
        prepareCurrentSlide(index);
    }else{
        index--;
        prepareCurrentSlide(index);
    }
}

next.addEventListener('click', nextSlide);
prev.addEventListener('click', prevSlide);

const prepareCurrentSlide = ind =>{
    activeSlide(index);
    activeDot(index);
}

dots.forEach((item, indexDot) =>{
    item.addEventListener('click', () =>{
        index = indexDot;
        prepareCurrentSlide(index);
    })
})

setInterval(nextSlide, 2500)
```