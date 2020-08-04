<script>
    import {
        GITHUB_URL,
        LINKED_IN_URL,
        TWITTER_URL,
        FACEBOOK_URL,
        WHATSAPP_URL
    } from 'Constants/constants'
</script>

<style>

    @media (min-width: 991px) {
        .header {
            position: fixed;
            right: 30px;
            bottom: 0;
            z-index: 3;
            display: flex;
            align-items: center;
            height: calc(100vh - 200px);
            top: 100px;
            opacity: 1;
            transition: opacity 0.3s;
            -webkit-transition: opacity 0.3s;
        }

        .header-mobile {
            display: none;
        }

        li.icon-box:hover{
            background-color: #ffb400;
        }

        li.icon-box{
            width: 50px;
            height: 50px;
            list-style: none;
            position: relative;
            display: flex;
            align-items: center;
            transition: .3s;
            margin: 20px 0;
            border-radius: 50%;
            background: #2b2a2a;
        }

        a{
            display: block;
            padding: 0;
            width: 50px;
            height: 50px;
            text-decoration: none;
        }

        a:hover h2{
            opacity: 1;
            right: 27px;
            margin: 0;
            text-align: center;
            border-radius: 30px 0 0 30px;
            background-color: #ffb400;
        }

        a h2 {
            font-family: 'Poppins', sans-serif;
            z-index: -1;
            position: absolute;
            top: 0;
            right: 0;
            opacity: 0;
            color: #fff;
            line-height: 50px;
            font-weight: 500;
            transition: all .3s;
            border-radius: 30px;
            text-transform: uppercase;
            padding: 0 25px 0 30px;
            height: 50px;
        }

        .fa {
            font-size: 19px;
            position: absolute;
            pointer-events: none;
            left: 0;
            right: 0;
            margin: 0 auto;
            display: block;
            text-align: center;
            top: 15px;
            color: white;
        }
    }

</style>

<header class="header" id="header">

    <ul class="icon-menu">
        <li class="icon-box active">
            <i class="fa fa-github-alt"></i>
            <a href={GITHUB_URL} target="_blank">
                <h2>Github</h2>
            </a>
        </li>
        <li class="icon-box">
            <i class="fa fa-linkedin"></i>
            <a href={LINKED_IN_URL} target="_blank">
                <h2>LinkedIn</h2>
            </a>
        </li>
        <li class="icon-box">
            <i class="fa fa-twitter"></i>
            <a href={TWITTER_URL} target="_blank">
                <h2>Twitter</h2>
            </a>
        </li>
        <li class="icon-box">
            <i class="fa fa-facebook-f"></i>
            <a href={FACEBOOK_URL} target="_blank">
                <h2>Facebook</h2>
            </a>
        </li>
        <li class="icon-box">
            <i class="fa fa-whatsapp"></i>
            <a href={WHATSAPP_URL} target="_blank">
                <h2>WhatsApp</h2>
            </a>
        </li>
    </ul>

    <!-- MWeb Page -->
    <nav role="navigation" class="header-mobile">
        <div id="menuToggle">
            <input type="checkbox">
            <span></span>
            <span></span>
            <span></span>
            <ul class="list-unstyled" id="menu">
                <li class="active"><a href="index.html"><i class="fa fa-home"></i><span>Home</span></a></li>
                <li><a href="about.html"><i class="fa fa-user"></i><span>About</span></a></li>
                <li><a href="portfolio.html"><i class="fa fa-folder-open"></i><span>Portfolio</span></a></li>
                <li><a href="contact.html"><i class="fa fa-envelope-open"></i><span>Contact</span></a></li>
                <li><a href="blog.html"><i class="fa fa-comments"></i><span>Blog</span></a></li>
            </ul>
        </div>
    </nav>
    <!-- Mobile Menu Ends -->
</header>