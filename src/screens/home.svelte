<script>
    let src = 'static/images/tarik.png';
    let resumePath = 'static/pdf/Tarik.pdf';
</script>

<style>
    .main-container{
        height: 100vh;
        width: 100vw;
        background-color: #111;
    }
    @media (min-width: 991px)  {
        .image-frame{
            position: fixed;
            height: 200vh;
            width: 100vw;
            transform: rotate(-15deg);
            left: -83%;
            top: -50%;
        }
        .content-container{
            height: 100%;
            width: 100%;
            align-items: center;
            display: grid;
            grid-template-columns: 1.5fr 3fr;
        }
        .image-container{
            margin-left: 3em;
            height: calc(100% - 6em);
            z-index: 100;
            box-shadow: 0 0 7px rgba(0,0,0,.9);
            background-color: #111;
            border-radius: 1.5em;
        }
        .image-container img{
            border-radius: 1.5em;
            object-fit: cover;
            height: 100%;
            width: 100%;
        }
        .image-container-mobile{
            display: none;
        }

        .intro-section{
            max-width: 600px;
            margin: 0 auto;
        }
        .description-text{
            line-height: 2em;
            margin: 1em 0 1.5em 0;
        }
        .about-me-container{
            height: 4.8em;
            border-radius: 2.4em;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 0 2.4em;
            width: max-content;
        }
    }

    @media (max-width: 991px)  {
        .image-frame{
            display: none;
        }
        .content-container{
            height: 100%;
            width: 100%;
        }
        .image-container{
            display: none;
        }
        .image-container-mobile{
            justify-self: center;
            align-self: flex-end;
            height: 16em;
            width: 16em;
            border-radius: 50%;
            z-index: 100;
            box-shadow: 0 0 7px rgba(0,0,0,.9);
            background-color: #111;
            border: 4px solid #252525;
        }
        .image-container-mobile img{
            border-radius: 50%;
            object-position: 50% 10%;
            object-fit: cover;
            height: 100%;
            width: 100%;
        }
        .home-page-details{
            height: 100%;
            width: 100%;
            align-items: center;
            display: grid;
            grid-template-rows: 1fr 2fr;
        }

        .intro-section{
            display: flex;
            flex-direction: column;
            justify-items: center;
            align-items: center;
            padding: 0 1.6em;
            justify-self: center;
            align-self: center;
            max-width: 400px;
        }
        .intro-section p{
            text-align: center;
        }

        .description-text{
            line-height: 2em;
            margin: 1em 0;
        }
        .about-me-container{
            height: 4em;
            border-radius: 2em;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 0 2em;
            width: max-content;
        }
    }

    .hi-text{
        color: #eee;
        margin-bottom: 0.5em;
    }

    .about-me-container a{
        text-decoration: none;
    }

</style>

<section class="main-container">
    <div class="image-frame yellow-color-background"></div>
    <div class="content-container">
        <div class="image-container">
            <img src={src} alt="This is my personal image" title="tarik-sahni" aria-hidden="true" role="presentation"/>
        </div>
        <div class="home-page-details">
            <div class="image-container-mobile">
                <img src={src} alt="This is my personal image" title="tarik-sahni" aria-hidden="true" role="presentation"/>
            </div>
            <div class="intro-section">
                <h6 class="open-sans-font upper-case hi-text fs-3 fw-normal">Hi there ! &#128075;</h6>
                <h1 class="yellow-color poppins-font upper-case fw-bold fs-5">
                    <span class="my-details white-color">I'm</span>
                    Tarik Sahni
                </h1>
                <p class="open-sans-font white-color fs-2 description-text">Creative and self-starting Front-End Developer with 2+ years experience building stable E2E websites and apps in fast-paced, collaborative environments with great performance and SEO. Highly skilled in HTML/CSS/JavaScript and working knowledge of Web frameworks. Well-versed in Scrum and Agile.</p>
                <div class="about-me-container yellow-color-background">
                    <a href={resumePath} download="Tarik_Sahni_Resume"><span class="white-color upper-case fs-2 fw-medium" >Download Resume &nbsp; 💻</span></a>
                </div>
            </div>
        </div>
    </div>
</section>

