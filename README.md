авторизация
===========
![Alt-текст](https://4.bp.blogspot.com/EJIfQVyo9XD89XsDkYI5Y5GjmytbV7UlxfGdc9UbdAZAfuBFYx4xQsgxqPd5cjQ71ak0rS_hR8OWtIaL1g=w1080-h608-p-no-v0 "")
система авторизации ещё не дороботана 
-------------------------------------
будет доступна к 5 июню 2021 года
---------------------------------
index.html
==========
`<!DOCTYPE html>
<html>
<head class="header">
  <meta charset="UTF-8">
  <title>Четыре правила вёрстки</title>
  <link rel="stylesheet" href="style.css">
   <link rel="shortcut icon" href="https://lh3.googleusercontent.com/UCgehEVAkaAq0nKhn5ZdTmDjU6SPE0I-DJfl0NLFivj2PVB56h2wMiAiAD2-UH5GJICV_4h5v7ECdKpcl15weCf3HVj8gT7W7_ZpaoMagOPMbfMvfL-UVva52p4OVuwOC-CwDZHBYV0XOFzDzvCeL9TYIn2Sjg4DudWQWkHUaFrV_gn5o_MlCKz2rGMbifsTqWuy3yu1F9bQF2SjqADrYmvnKrQFqOQ8MAehW4JyKk0wk8ktiuP6tJNWWphHaS5aahUvlOBkIeF7hIHUB3QI97brFb8XKqWd2ezV6PS2YXVAUm4mNiFZRt5cbdkxTz5YnmFUO3bFD-gXaFsmEaS02Ithysv3ojVbygPsDEL5xySTTZnqML14LjnHzT8sEGn0wfR_fRYPxbBXEuDbt7uk0OzOGvxi-Ebt8QCLkSCgp8LSjegeczt1-Y9SmQL4OmMz1pHzxwwS8xCoRelyvfMEzVkK_5ieyQnIVJEccIjsBMZA3XrHA4FmjqRBgpl6QT_TOP73s_c5xkpRCfx3dH23zlUKhf8mR25vQPMhtPbEYvLAuCMF5XhHRZCLBzrdICeEO9St-XLa6aqRtPcyTjVW3U_hoTQkvL8y7aEihLRvxhWc6g6tNpl-uu3s1h3Sr5f0M1MI7K7Kwbp1XPswpUit_O6pHmFz7orvp8PAwUd1NXkZGdeuXkJfpe8jC2FU3eY=w328-h249-no?authuser=0" type="image/x-icon">
</head>
<body>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script src="jquery.cookie.js"></script>
<header class="header">
    <div class="overlay">
      <h1 class="header-title">Четыре правила вёрстки</h1>
    </div>
  </header>
  <div dir="ltr" style="text-align: left;" trbidi="on">
<html>
<head>

<style>
body {font-family: Arial, Helvetica, sans-serif;}

/* Full-width input fields */
input[type=text], input[type=password] {
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    box-sizing: border-box;
}

/* Set a style for all buttons */
button {
    background-color: #4CAF50;
    color: white;
    padding: 14px 20px;
    margin: 8px 0;
    border: none;
    cursor: pointer;
    width: 100%;
}

button:hover {
    opacity: 0.8;
}

/* Extra styles for the cancel button */
.cancelbtn {
    width: auto;
    padding: 10px 18px;
    background-color: #f44336;
}

/* Center the image and position the close button */
.imgcontainer {
    text-align: center;
    margin: 24px 0 12px 0;
    position: relative;
}

img.avatar {
    width: 40%;
    border-radius: 50%;
    margin: 10px auto;
}

.container {
    padding: 16px;
}

span.psw {
    float: right;
    padding-top: 16px;
}

/* The Modal (background) */
.modal {
    display: none; /* Hidden by default */
    position: fixed; /* Stay in place */
    z-index: 1; /* Sit on top */
    left: 0;
    top: 0;
    width: 100%; /* Full width */
    height: 100%; /* Full height */
    overflow: auto; /* Enable scroll if needed */
    background-color: rgb(0,0,0); /* Fallback color */
    background-color: rgba(0,0,0,0.4); /* Black w/ opacity */
    padding-top: 60px;
}

/* Modal Content/Box */
.modal-content {
    background-color: #fefefe;
    margin: 5% auto 15% auto; /* 5% from the top, 15% from the bottom and centered */
    border: 1px solid #888;
    width: 80%; /* Could be more or less, depending on screen size */
}

/* The Close Button (x) */
.close {
    position: absolute;
    right: 25px;
    top: 0;
    color: #000;
    font-size: 35px;
    font-weight: bold;
}

.close:hover,
.close:focus {
    color: red;
    cursor: pointer;
}

/* Add Zoom Animation */
.animate {
    -webkit-animation: animatezoom 0.6s;
    animation: animatezoom 0.6s
}

@-webkit-keyframes animatezoom {
    from {-webkit-transform: scale(0)} 
    to {-webkit-transform: scale(1)}
}
    
@keyframes animatezoom {
    from {transform: scale(0)} 
    to {transform: scale(1)}
}

/* Change styles for span and cancel button on extra small screens */
@media screen and (max-width: 300px) {
    span.psw {
       display: block;
       float: none;
    }
    .cancelbtn {
       width: 100%;
    }
}
</style>
</head>
<body>
    <style>
   .card {
    background: #007E3E; /* Цвет фона */
    color: #fff; /* Цвет текста */
    padding: 10px; /* Поля вокруг текста */
    border-radius: 20px; /* Уголки */
   }
  </style>
 </head>
 <body>
<script>
  window.onload = function () {
    document.body.classList.add('loaded_hiding');
    window.setTimeout(function () {
      document.body.classList.add('loaded');
      document.body.classList.remove('loaded_hiding');
    }, 500);
  }
</script>
<div class="preloader">
  <div class="preloader__row">
    <div class="preloader__item"></div>
    <div class="preloader__item"></div>
  </div>
</div>
<style>

.preloader {
  /*фиксированное позиционирование*/
  position: fixed;
  /* координаты положения */
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  /* фоновый цвет элемента */
  background: #e0e0e0;
  /* размещаем блок над всеми элементами на странице (это значение должно быть больше, чем у любого другого позиционированного элемента на странице) */
  z-index: 1001;
}

.preloader__row {
  position: relative;
  top: 50%;
  left: 50%;
  width: 70px;
  height: 70px;
  margin-top: -35px;
  margin-left: -35px;
  text-align: center;
  animation: preloader-rotate 2s infinite linear;
}

.preloader__item {
  position: absolute;
  display: inline-block;
  top: 0;
  background-color: #337ab7;
  border-radius: 100%;
  width: 35px;
  height: 35px;
  animation: preloader-bounce 2s infinite ease-in-out;
}

.preloader__item:last-child {
  top: auto;
  bottom: 0;
  animation-delay: -1s;
}

@keyframes preloader-rotate {
  100% {
    transform: rotate(360deg);
  }
}

@keyframes preloader-bounce {

  0%,
  100% {
    transform: scale(0);
  }

  50% {
    transform: scale(1);
  }
}

.loaded_hiding .preloader {
  transition: 0.3s opacity;
  opacity: 0;
}

.loaded .preloader {
  display: none;
}
</style>
<button onclick="document.getElementById('id01').style.display='block'" style="width: auto;">Login</button>

<div class="modal" id="id01">
  
  <form action="/action_page.php" class="modal-content animate">
    <div class="imgcontainer">
      <span class="close" onclick="document.getElementById('id01').style.display='none'" title="Close Modal">×</span><div class="separator" style="clear: both; text-align: center;">
<a href="https://4.bp.blogspot.com/EJIfQVyo9XD89XsDkYI5Y5GjmytbV7UlxfGdc9UbdAZAfuBFYx4xQsgxqPd5cjQ71ak0rS_hR8OWtIaL1g=w1080-h608-p-no-v0" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" data-original-height="608" data-original-width="1080" height="360" src="https://4.bp.blogspot.com/EJIfQVyo9XD89XsDkYI5Y5GjmytbV7UlxfGdc9UbdAZAfuBFYx4xQsgxqPd5cjQ71ak0rS_hR8OWtIaL1g=w1080-h608-p-no-v0" width="640" /></a></div>
</div>
<div class="container">
      <label for="uname"><b>Username</b></label>
      <input name="uname" placeholder="Enter Username" required="" type="text" />

      <label for="psw"><b>Password</b></label>
      <input name="psw" placeholder="Enter Password" required="" type="password" />
        
      <button type="submit">Login</button>
      <label>
        <input checked="checked" name="remember" type="checkbox" /> Remember me
      </label>
    </div>
<div class="container" style="background-color: #f1f1f1;">
      <button class="cancelbtn" onclick="document.getElementById('id01').style.display='none'" type="button">Cancel</button>
      <span class="psw">Forgot <a href="https://draft.blogger.com/u/1/blogger.g?blogID=5042441321428311860#">password?</a></span>
    </div>
</form>
</div>
<script>
// Get the modal
var modal = document.getElementById('id01');

// When the user clicks anywhere outside of the modal, close it
window.onclick = function(event) {
    if (event.target == modal) {
        modal.style.display = "none";
    }
}
</script>

</body>
</html>



</div>

  <section class="content">
    <div class="card">
      <img class="card-image"
           src="https://pictures.s3.yandex.net/frontend-developer/free-course/card-1.jpg">
      <h3 name = "Пустота"class="card-title">Пустота</h3>
      <p class="card-text">Простое правило, которое часто нарушают: ставьте рядом элементы с похожим смыслом и окружайте их пустым пространством. Пустота — мощное средство воздействия.</p>
    </div>
    <div class="card  no-right-margin">
      <img class="card-image"
           src="https://pictures.s3.yandex.net/frontend-developer/free-course/card-2.jpg">
      <h3 name = "Сетка" class="card-title">Сетка</h3>
      <p class="card-text">Размеры элементов и расстояния между ними укладываются в гармоничную схему — её называют сеткой. Если элемент выпадает из сетки, что-то не так.</p>
    </div>
    <div class="card">
    <img class="card-image" src="https://pictures.s3.yandex.net/frontend-developer/free-course/card-3.jpg">  
    <h3 name = "Шрифты" class="card-title">Шрифты</h3>  
    <p class="card-text">Не больше трёх шрифтов на сайт. Один для заголовков, второй — для всех остальных текстов, третий — для выделения важных слов. И всё.</p>
</div>
    <div class="card no-right-margin">
    <img class="card-image" src="https://pictures.s3.yandex.net/frontend-developer/free-course/card-4.jpg">  
    <h3 name = "Цвета" class="card-title">Цвета</h3>  
    <p class="card-text">Обычно на сайте два цвета: ведущий и акцентный. Подобрать удачную цветовую пару можно специальными инструментами.</p>
</div>
  </section>
<footer class="footer">
    <h4 class="footer-author"></h4>
</footer>
  <script src="//code-ya.jivosite.com/widget/mmXR2vT1ww" async></script>
</div>
</body>
</html>` element here instead.
