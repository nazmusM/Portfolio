<!DOCTYPE html>
<html lang="en">
<head>
    <style type="text/css" media="all">
      *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    
}
html{
    font-size: 10px;
    font-family: Verdana;
    scroll-behavior: smooth;
    
}
a{
    text-decoration: none;
    color: green;
}
.container{
    min-height: 70vh;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}
#hero{
    background: orange;
    background-size: cover;
    background-position: center;
    position: relative;
    z-index: 1;
}
#hero::after{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background-color: black;
    opacity: .7;
    z-index: -1;
}
#hero h1{
    display: block;
    width: fit-content;
    font-size: 4rem;
    position: relative;
    color: transparent;
    animation: reveal .5s ease forwards;
    animation-delay: 1.5s;
}
 .cta{
    display: inline-block;
    padding: 10px 30px;
    color: crimson;
    background-color: transparent;
    border: 2px solid crimson;
    font-size: 2rem;
    border-radius: 50px;
    text-transform: uppercase;
    letter-spacing: .1rem;
    margin-top: 30px;
    transition: .3s ease;
    transition-property: background-color, color;
} .cta:hover{
    color: white;
    background-color: crimson;
}
#hero h1 span{
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 0;
    background-color: yellow;
    animation: text_reveal_box 1s ease;
    animation-delay: 1s;
    
    
    
}
@keyframes text_reveal_box{
    50%{width: 100%;
    left: 0;
        
    }
    100%{
        width: 0;
   left: 100%;
    }
}
@keyframes reveal{
    100%{
        color: yellow;
    }
}
#hero h1:nth-child(1){
    animation-delay: 1.5s;
}
#hero h1:nth-child(2){
    animation-delay: 2.5s;
}
#hero h1:nth-child(1) span{
    animation-delay: 1s
}
#hero h1:nth-child(2) span{
    animation-delay: 2s;
}
#services{
    
}
#services .services{
    flex-direction: column;
    text-align: center;
    max-width: 1500px;
    margin:0 auto;
    padding:10px 0;
    }
  .section-title{
    font-size: 4rem;
    font-weight: 300px;
    color: blue;
    margin-bottom: 10px;
    text-transform: uppercase;
    letter-spacing: .2rem;
    text-align: center;
}
#services .service-top p{
    font-size: 1.4rem;
    
    margin-top: 5px;
    line-height: 2.5rem;
    font-weight: 300;
    letter-spacing: .05rem;
}
#services .service-bottom{
display: flex;
align-items: center;
justify-items: center;
flex-wrap: wrap;
}
#services .service-item{
    flex-basis: 80%;
    display: flex;
    align-items: flex-start;
    justify-content: center;
    flex-direction: column;
    padding:30px;
    background: silver;
    border: 2px solid red;
    border-radius: 10px;
    margin: 10px 10%;
    
    
}
#services .services p{
    font-weight: bold;
    text-align: left;
    margin: 0 auto;
    text-align: center;
}
#services .service-bottom .icon img{
    height: 25px;
    width: 25px;
    object-fit: cover;
    margin-bottom: 20px;

}
#services .service-item h2{
    margin-bottom: 20px;
    font-size: 3rem;
    color: red;
    text-align: center;
}

#services .service-item p{
    color: crimson;
    text-align: left;
    font-size: 1.2rem;
    line-height: 1.9rem;
}
#projects .section-title span{
    color: crimson;
}
#projects .section-title{
    color: blue;
    font-weight: bold;
    font-size: 3rem;
}
.project-info h1{
    color: orange;
    font-size: 2rem;
    font-weight: bold;
}
.project-info{
    text-align: center;
    border: 2px solid blue;
    border-radius: 10px;
    padding: 10px;
    margin-bottom: 15px;
    background: #008080;
    margin-left: 15px;
    margin-right: 15px;
}
hr{
    border-top:1px solid orange;
    border-bottom: 1px solid orange;
    border-left: .9px solid orange;
    border-right: .9px solid orange;
}
.project-info h2{
    font-weight: bold;
    color: orange;
    text-align: right;
    margin: 5px 5px 5px 5px;
}
.project-info p{
    color: white;
    text-align: left;
    margin: 0 auto;
    font-size: 1rem;
}
#about .section-title{
    color: black;
    font-weight: bold;
    border-bottom: 2px solid red;
    border: 5px solid crimson;
    padding: 10px;
    margin-left: 10px;
    margin-right: 10px;
    background: #008080;
    border-radius: 5px;


}
#about h2{
    text-align: center;
    font-size: 2rem;
    color: blue;
    margin-top: 2rem;
    margin-bottom: 2rem;
}
#about p{
    margin-left: 25px;
    margin-right: 25px;
    font-size: 15px;
    margin-bottom: 20px;
}

.col-right{
    border: 5px solid red;
    padding: 20px;
    background: grey;
}
.contact-info {
    height:150px;
    width:320px;
    
    border-radius:10px ;
    text-align: center;
    margin-top: 20px ;
    padding: 55px;
    background: silver;
   
  
  
}
.contact-info h1{ 
font-size: 20px;
    color: blue;
    
}
.contact-info:hover{
background: crimson;
transition: .7s;}
#contact .section-title{
    color: Blue;
}
#contact .section-title span{
    color: red;
}
#footer{
    background-image: linear-gradient(60deg, #29323c 0%, #485563 100%);
    margin-top: 40px;
}

#about .about{
    min-height: 400px;
}
#footer .footer{
    min-height: 100px;
    flex-direction: column;
    padding-top: 50px;
    padding-bottom: 10px;
}
.brand h1{
    font-size: 3rem;
    text-transform: uppercase;
    color: green;
}
.brand h2{
    font-size: 2rem;
    color: white;
    text-align: center;
    margin-top: 10px;
    margin-bottom: 10px;
}
.brand span{
    color: red;
}
#footer p{
font-size: 1.2rem;
    color: white;
    font-weight: bold;
    margin-top: 10px;
    margin-bottom: 10px;
    text-align: center;}

#footer .footer{
    display: flex;
}

#footer .social{
    display: flex;
   margin: 0 5px;
   margin-bottom: 25px;
   margin-top: 5px;
}
#footer .social-item{
    margin: 5px;
}
#header{
    position: fixed;
    z-index: 1000;
    left: 0;
    top: 0;
    width: 100vw;
    height: auto;
  
}
#header .header{
    min-height: 8vh;
    background: transparent;
}
#header .nav-bar{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    height: 100%;
    max-width: 1300px;
    padding: 10px 10px;
    
    
    }
 #header  .nav-list ul{
        list-style: none;
        position: absolute;
        background-color: purple;
        width: 65vw;
        height: 100vh;
        left: 130px;
        top:0;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        z-index: 1;
        overflow-x: hidden;
        display: none;
        
   
}
#header  .nav-list ul.active{
    display:flex ;
    
}
    
}
#header .nav-list ul a{
    font-size: 2.5rem;
    font-weight: bold;
    letter-spacing: .2rem;
    text-decoration: none;
    color: white;
    text-transform: uppercase;
    padding: 20px;
    display: block;
}
#header .nav-list ul a::after{
    content:attr(data-after);
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) scale(0);
    font-size: 8rem;
    letter-spacing: 50px;
    z-index: -1;
    color: rgba(240, 248, 255, 0.021);
    transition: .3s ease letter-spacing;
    
}
#header .nav-list ul li:hover a::after{
    transform: translate(-50%, -50%) scale(1);
    letter-spacing: initial;
}
#header .hamburger{
    height: 45px;
    width: 45px;
    display: inline-block;
    
    position: relative;
    z-index: 100;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}

#header .hamburger .bar{
    height: 2px;
    width: 30px;
    background-color: black;
    position: relative;
    z-index: -1;
}
#header .hamburger .bar::after,
#header .hamburger .bar::before{
    content:'';
    position: absolute;
    height: 100%;
    width: 100%;
    left: 0;
    background-color: black;
    transition: .5s;
  
}
#header .hamburger .bar::after{
    top: 8px;
   }
   #header .hamburger .bar::before{
       bottom: 8px;
   }
#header .hamburger.active .bar::after {
    top: 8px;
  transform: rotate(45deg);
}
#header .hamburger.active .bar::before {
    bottom: 8px;
    transform: rotate(-45deg);
}

#header .hamburger.active .bar::before,
#header .hamburger.active .bar::after{
    top: 0;
    bottom: 0;
}
#header ul{
    font-size: 3rem;
    padding: 20px;
    line-height: 5rem;
    font-weight: bold;
     color: white;
     
}


#header ul a{
    color: red;
}
#header .hamburger.active .bar{
    background: transparent;
}
#header .hamburger::after{
    position: absolute;
    content:'';
    height: 100%;
    width: 100%;
    border-radius: 50px;
    border: 2px solid black;
    animation: hamburger 1s ease infinite;
}
@keyframes hamburger{
    0%{
        opacity: 1;
        transform: scale(1)
    }
    100%{
        opacity: 0;
        transform: scale(1.5)
    }
}

    </style>
    <meta charset="UTF-8">
    <title>My Portfolio</title>
</head>
<body>
    <section id="header">
        <div class="header container">
            <div class="nav-bar">
                <div class="brand">
                    <a href="#hero"><h1>Nazmus <span>Sakib</span></h1></a>
                </div>
                <div class="nav-list">
                    <div class="hamburger">
                        <div class="bar">   </div>
                    </div>
                    <ul>
                      <li><a href="#hero" data-after="Home">Home</a></li>
<li><a href="#services" data-after="Services">Services</a></li>
<li><a href="#projects"data-after="Projects">Projects</a></li>
<li><a href="#about" data-after="About">About</a></li>
<li><a href="#contact" data-after="Contact">Contact</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
    <section id="hero">
        <div class="hero container">
            <div>
                <h1>Nazmus <span></span></h1>
                <h1>Sakib<span></span></h1>
                <a href="#projects" class="cta">Portfolio</a>
            </div>
        </div>
    </section>
    <section id="services">
        <div class="services container">
            <div class="service-top">
                <h1 class="section-title">Serv<span>i</span>ces</h1>
          <p id="p">My name is Nazmus Sakib My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>      
            </div>
            <div class="service-bottom">
                <div class="service-item">
                    <div class="icon">
                        <img src="https://img.icons8.com/ios-glyphs/30/000000/about.png"/>
                    </div>
                    <h2>Web Design</h2>
                    <p>My name is Nazmus Sakib My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>
                </div><div class="service-item">
                    <div class="icon">
                        <img src="https://img.icons8.com/ios-glyphs/30/000000/about.png"/>
                    </div>
                    <h2>Web Design</h2>
                    <p>My name is Nazmus Sakib My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>
                </div><div class="service-item">
                    <div class="icon">
                        <img src="https://img.icons8.com/ios-glyphs/30/000000/about.png"/>
                    </div>
                    <h2>Web Design</h2>
                    <p>My name is Nazmus Sakib My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>
                </div><div class="service-item">
                    <div class="icon">
                        <img src="https://img.icons8.com/ios-glyphs/30/000000/about.png"/>
                    </div>
                    <h2>Web Design</h2>
                    <p>My name is Nazmus Sakib My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>
                </div><div class="service-item">
                    <div class="icon">
                        <img src="https://img.icons8.com/ios-glyphs/30/000000/about.png"/>
                    </div>
                    <h2>Web Design</h2>
                    <p>My name is Nazmus Sakib My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>
                </div><div class="service-item">
                    <div class="icon">
                        <img src="https://img.icons8.com/ios-glyphs/30/000000/about.png"/>
                    </div>
                    <h2>Web Design</h2>
                    <p>My name is Nazmus Sakib My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>
                </div>
            </div>
        </div>
    </section>
    <section id="projects">
        <div class="projects container">
            <div class="projects-header">
                <h1 class="section-title">
                    Recent <span>Projects</span>
                </h1>
                <div class="all-projects">
                    <div class="project-items">
                        <div class="project-info">
                            <h1>Project 1</h1><hr>
                            <h2>Freelancer's Choice</h2>
                            <p>
                                My name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib Syam
                            </p>
                        </div>
                    </div>
                     <div class="project-items">
                        <div class="project-info">
                            <h1>Project 2</h1><hr>
                            <h2>Freelancer's Choice</h2>
                            <p>
                                My name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib Syam
                            </p>
                        </div>
                    </div> <div class="project-items">
                        <div class="project-info">
                            <h1>Project 3</h1><hr>
                            <h2>Freelancer's Choice</h2>
                            <p>
                                My name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib Syam
                            </p>
                        </div>
                    </div> <div class="project-items">
                        <div class="project-info">
                            <h1>Project 4</h1><hr>
                            <h2>Freelancer's Choice</h2>
                            <p>
                                My name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib Syam
                            </p>
                        </div>
                    </div> <div class="project-items">
                        <div class="project-info">
                            <h1>Project 5</h1><hr>
                            <h2>Freelancer's Choice</h2>
                            <p>
                                My name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib SyamMy name is Nazmus Sakib Syam
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section id="about">
        <div class="about container">
            <div class="col-left">
                <div class="about-bg"></div>
            </div>
            <div class="col-right">
                <h1 class="section-title">About <span>Me</span></h1>
                <h2>Front End Developer</h2>
                <p>My name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus SakibMy name is Nazmus Sakib</p>
                <a id="resume" class="cta" href="#">Download Resume</a>
            </div>
        </div>
    </section>
    <section id="contact">
        <div class="contact container">
            <div>
                <h1 class="section-title">
                    Contact <span>Info</span>
                </h1>
                <div class="contact-items">
                    <div class="contact-item">
                        
                            
                        </div>
                        <div class="contact-info">
                            <h1>Phone:</h1>
                            <h2><a href="tel:+8801770769066">+8801770769066</a></h2>
                            
                        </div>
                    </div><div class="contact-item">
                        <div class="icon">
                            
                        </div>
                        <div class="contact-info">
                            <h1>Email:</h1>
                            <h2><a href="mailto: nazmussakibsyam@gmail.com">nazmussakibsyam@gmail.com</a></h2>
                            
                        </div>
                    </div><div class="contact-item">
                        <div class="icon">
                            
                        </div>
                        <div class="contact-info">
                            <h1>Address:</h1>
                            <h2>Ghatail, Tangail, Dhaka
Bangladesh</h2>
                            
                        </div>
                    </div>
                    
                </div>
                    
                
            </div>
        
    </section>
    <section id="footer">
        <div class="footer container">
            <div class="brand">
                <h1><span>Nazmus</span> Sakib</h1>
                <h2>Choose Your Best</h2>    </div> <div class="social">
                <div class="social-item">
                        <a href="https://m.facebook.com/nazmusemu1"><img src="https://img.icons8.com/offices/35/000000/facebook-new.png"/></a>
                        
                    </div>  <div class="social-item">
                        <a href="https://mobile.twitter.com/nazmusM2"><img src="https://img.icons8.com/color/35/000000/twitter--v1.png"/></a>
                        
                    </div>  <div class="social-item">
                        <a href="https://www.instagram.com/nazmusm1/"><img src="https://img.icons8.com/officexs/35/000000/instagram-new.png"/></a>
                        
                    </div> <div class="social-item">
                        <a href="https://www.linkedin.com/mwlite/in/nazmus-sakib-syam-915a50204"><img src="https://img.icons8.com/fluency/35/000000/linkedin-circled.png"/></a>
                        
                        </div>
                        
                    </div>
               
                
           
            <p class="name">copyright © 2022||<span>Nazmus Sakib</span>❤️<span>Mitu Akter</span>||All rights reserved</p>
        </div>
    </section>
    <script>
const hamburger = document.querySelector("#header .hamburger");
const header = document.querySelector("#header .nav-list ul");
const menu_item = document.querySelectorAll("#header .nav-list ul li a");
const mobile_menu = document.querySelector("#header .nav-bar .nav-list ul");

hamburger.addEventListener("click",() => {
    header.classList.toggle("active");
    hamburger.classList.toggle("active");
});

menu_item.forEach((item) => {
    item.addEventListener("click", () => {
        hamburger.classList.toggle("active");
        mobile_menu.classList.toggle("active");
    })
})

</script>
</body>
</html>
