styles.css

/*Master styles*/
body {
    font-family: "Questrial", sans-serif;
    margin: 0px;

}

.container {
    display: grid;
    grid-template-columns: 1fr;
}

/*Nav styles*/
.nav-wrapper {
     display: flex;
     justify-content: space-between;
     padding: 38px;
 }

 .left-side {
     display: flex;
 }

 .nav-wrapper > .left-side >div {
    margin-right: 20px;
    font-size: 0.9em;
    text-transform: uppercase;
}

.nav-link-wrapper {
    height: 22px;
    border-bottom: 1px solid transparent;
    transition: border-bottom 0.5s;
}

.nav-link-wrapper a {
    color: #8a8a8a;
    text-decoration: none;
    transition: color 0.5s;
}

.nav-link-wrapper:hover {
    border-bottom: 1px solid black;
}

.nav-link-wrapper a:hover {
    color: black;
}

.active-nav-link {
    border-bottom: 1px solid black;
}

.active-nav-link a {
    color: black !important;
}

/*Portfolio styles*/

.portfolio-items-wrapper {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}

.portfolio-item-wrapper {
    position: relative;
}

.portfolio-img-background {
    height: 400px;
    width: 100%;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

.img-text-wrapper {
    position: absolute;
    top: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100%;
    text-align: center;
    padding-left: 100px;
    padding-right: 100px;
}

.logo-wrapper img {
    width: 50%;
    margin-bottom: 20px;
}

.img-text-wrapper .subtitle {
    transition: 1s;
    font-weight: 600;
    color: transparent;
}

.img-text-wrapper:hover .subtitle {
    font-weight: 600;
    color: grey;


}

.img-darken {
    transition: 1s;
    filter: brightness(10%);
}

.two-column-wrapper {
    display: grid;
    grid-template-columns: 1fr 1fr;
}

.profile-image-wrapper img {
    width: 100%;
}

.profile-content-wrapper{
    padding: 30px;
}

.profile-content-wrapper h1 {
    background-color: lightgray;
    color: black;
}

.profile-content-wrapper p {
    color: darkslategrey;
    font-size: 120%;
}


<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <title>Page Title</title>
    <link href="https://fonts.googleapis.com/css2?family=Questrial&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <div class="nav-wrapper">
            <div class="left-side">
                <div class="nav-link-wrapper active-nav-link">
                    <a href="index.html">Home</a>
                </div>

                <div class="nav-link-wrapper">
                 <a href="about.html">About</a>
                </div>
            </div>

            <div class="right-side">
                <div class="brand">
                    <div>VELOScity Tech, Inc.</div>
                </div>
            </div>
        </div>

        <div class="content-wrapper">
            <div class="portfolio-items-wrapper">

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style="background-image: url(Wallpaper/image1.jpg);"></div>

                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img class= "hover-image" src="Logos/logo1.png" alt="">
                        </div>

                        <div class="subtitle">
                            Virtual Reality
                        </div>

                        <div class="subtitle">
                            Experience life from a whole new dimension - with technologies that could bring you to places you have never been before
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style="background-image: url(Wallpaper/image2.jpg);"></div>

                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="Logos/logo2.png">
                        </div>

                        <div class="subtitle">
                            Drone Technology
                        </div>

                        <div class="subtitle">
                            Hovering different plains for photography, lightweight transport, and game experience is much easier with aerial technologies.
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style="background-image: url(Wallpaper/image3.jpg);"></div>

                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="Logos/logo3.png">
                        </div>

                        <div class="subtitle">
                            Digital Art
                        </div>

                        <div class="subtitle">
                            Express your emotions with technology's way of lines, stroke, and colours that could take you to a whole new level of artistry
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style="background-image: url(Wallpaper/image4.jpg);"></div>

                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="Logos/logo4.png">
                        </div>

                        <div class="subtitle">
                            HI-tech Photography
                        </div>

                        <div class="subtitle">
                            Capture the world and its beauty in a whole new level to bring every single detail to a pixel of your new gallery      
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style="background-image: url(Wallpaper/image5.jpg);"></div>

                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="Logos/logo5.png">
                        </div>

                        <div class="subtitle">
                            Music
                        </div>

                        <div class="subtitle">
                            Sing your heart out to the beats of music from all ages and genres with great music techs
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style="background-image: url(Wallpaper/image8.jpg);"></div>

                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="Logos/logo6.png">
                        </div>

                        <div class="subtitle">
                            Gaming and Entertainment
                        </div>

                        <div class="subtitle">
                           Explore a whole new world of adventure with the best graphics to improve your gameplay with whole some fun
                        </div>
                    </div>
                </div>
            
            </div>
        </div>

    </div>
</body>
<script>
    const portfolioItems = document.querySelectorAll('.portfolio-item-wrapper')

    portfolioItems.forEach(portfolioItem=>{
        portfolioItem.addEventListener('mouseover', ()=> {
            portfolioItem.childNodes[1].classList.add('img-darken');
        })
    })

    portfolioItems.forEach(portfolioItem=>{
        portfolioItem.addEventListener('mouseout', ()=> {
            portfolioItem.childNodes[1].classList.remove('img-darken');
        })
    })

</script>
</html>
