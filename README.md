# assignment5
<!doctype html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>David Chu's China Bistro</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
    <link rel="stylesheet" href="css/styles.css">
    <link href='https://fonts.googleapis.com/css?family=Oxygen:400,300,700' rel='stylesheet' type='text/css'>
    <link href='https://fonts.googleapis.com/css?family=Lora' rel='stylesheet' type='text/css'>
    <a href="#" onclick="$dc.loadMenuItems('SP');"></a>
    <a href="#" onclick="$dc.loadMenuItems({{randomCategoryShortName}});"></a>
    <img src='images/ajax-loader.gif'></div>
    <section class='row'>
        <section class='row'>
            <div class='clearfix visible-lg-block visible-md-block'></div>
            <style>
                span {
                    font-size: 1.3em;
                }

                address p {
                    color: #557c3e;
                    font-size: .8em;
                    line-height: 1.8;
                }

                testimonials {
                    font-style: italic;
                }

                testimonials p:nth-child(2) {
                    margin-top: 25px;
                }

                /* END FOOTER */



                HOME PAGE .container .jumbotron {
                    box-shadow: 0 0 50px #3F0C1F;
                    border: 2px solid #3F0C1F;
                }

                menu-tile,
                specials-tile,
                map-tile {
                    height: 250px;
                    width: 100%;
                    margin-bottom: 15px;
                    position: relative;
                    border: 2px solid #3F0C1F;
                    overflow: hidden;
                }

                menu-tile:hover,
                specials-tile:hover,
                map-tile:hover {
                    box-shadow: 0 1px 5px 1px #cccccc;
                }

                menu-tile {
                    background: url('../images/menu-tile.jpg') no-repeat;
                    background-position: center;
                }

                specials-tile {
                    background: url('../images/specials-tile.jpg') no-repeat;
                    background-position: center;
                }

                menu-tile span,
                specials-tile span,
                map-tile span {
                    position: absolute;
                    bottom: 0;
                    right: 0;
                    width: 100%;
                    text-align: center;
                    font-size: 1.6em;
                    text-transform: uppercase;
                    background-color: #000;
                    color: #fff;
                    opacity: .8;
                }

                /* END HOME PAGE */

                /* MENU CATEGORIES PAGE */
                .category-tile {
                    position: relative;
                    border: 2px solid #3F0C1F;
                    overflow: hidden;
                    width: 200px;
                    height: 200px;
                    margin: 0 auto 15px;
                }

                .category-tile span {
                    position: absolute;
                    bottom: 0;
                    right: 0;
                    width: 100%;
                    text-align: center;
                    font-size: 1.2em;
                    text-transform: uppercase;
                    background-color: #000;
                    color: #fff;
                    opacity: .8;
                }

                .category-tile:hover {
                    box-shadow: 0 1px 5px 1px #cccccc;
                }

                menu-categories-title+div {
                    margin-bottom: 50px;
                }

                /* END MENU CATEGORIES PAGE */

                /* SINGLE CATEGORY PAGE */
                .menu-item-tile {
                    margin-bottom: 25px;
                }

                .menu-item-tile hr {
                    width: 80%;
                }

                .menu-item-tile .menu-item-price {
                    font-size: 1.1em;
                    text-align: right;
                    margin-top: -15px;
                    margin-right: -15px;
                }

                .menu-item-tile .menu-item-price span {
                    font-size: .6em;
                }

                .menu-item-photo {
                    position: relative;
                    border: 2px solid #3F0C1F;
                    overflow: hidden;
                    padding: 0;
                    margin-right: -15px;
                    margin-left: auto;
                    margin-bottom: 20px;
                    max-width: 250px;
                }

                .menu-item-photo div {
                    position: absolute;
                    bottom: 0;
                    right: 0;
                    width: 80px;
                    background-color: #557c3e;
                    text-align: center;
                }

                .menu-item-description {
                    padding-right: 30px;
                }

                h3.menu-item-title {
                    margin: 0 0 10px;
                }

                .menu-item-details {
                    font-size: .9em;
                    font-style: italic;
                }

                /* END SINGLE CATEGORY PAGE */


                /********** Large devices only **********/
                @media (min-width: 1200px) {
                    .container .jumbotron {
                        background: url('../images/jumbotron_1200.jpg') no-repeat;
                        height: 675px;
                    }
                }

                /********** Medium devices only **********/
                @media (min-width: 992px) and (max-width: 1199px) {

                    /* Header */
                    logo-img {
                        background: url('../images/restaurant-logo_medium.png') no-repeat;
                        width: 100px;
                        height: 100px;
                        margin: 5px 5px 5px 0;
                    }

                    /* End Header */

                    /* Home Page */
                    .container .jumbotron {
                        background: url('../images/jumbotron_992.jpg') no-repeat;
                        height: 558px;
                    }

                    /* End Home Page */
                }

                /********** Small devices only **********/
                @media (min-width: 768px) and (max-width: 991px) {

                    /* Home Page */
                    .container .jumbotron {
                        background: url('../images/jumbotron_768.jpg') no-repeat;
                        height: 432px;
                    }

                    /* End Home Page */
                }

                /********** Extra small devices only **********/
                @media (max-width: 767px) {

                    /* Header */
                    .navbar-brand {
                        padding-top: 10px;
                        height: 80px;
                    }

                    .navbar-brand h1 {
                        /* Restaurant name */
                        padding-top: 10px;
                        font-size: 5vw;
                        /* 1vw = 1% of viewport width */
                    }

                    .navbar-brand p {
                        /* Kosher cert */
                        font-size: .6em;
                        margin-top: 12px;
                    }

                    .navbar-brand p img {
                        /* Star-K */
                        height: 20px;
                    }

                    collapsable-nav a {
                        /* Collapsed nav menu text */
                        font-size: 1.2em;
                    }

                    collapsable-nav a span {
                        /* Collapsed nav menu glyph */
                        font-size: 1em;
                        margin-right: 5px;
                    }

                    call-btn>a {
                        font-size: 1.5em;
                        display: block;
                        margin: 0 20px;
                        padding: 10px;
                        border: 2px solid #fff;
                        background-color: #f6b319;
                        color: #951c49;
                    }

                    xs-deliver {
                        margin-top: 5px;
                        font-size: .7em;
                        letter-spacing: .1em;
                        text-transform: uppercase;
                    }

                    /* End Header */

                    /* Footer */
                    .panel-footer section {
                        margin-bottom: 30px;
                        text-align: center;
                    }

                    .panel-footer section:nth-child(3) {
                        margin-bottom: 0;
                        /* margin already exists on the whole row */
                    }

                    .panel-footer section hr {
                        width: 50%;
                    }

                    /* End Footer */

                    /* Home Page */
                    .container .jumbotron {
                        margin-top: 30px;
                        padding: 0;
                    }

                    menu-tile,
                    specials-tile {
                        width: 360px;
                        margin: 0 auto 15px;
                    }

                    .menu-item-photo {
                        margin-right: auto;
                    }

                    .menu-item-tile .menu-item-price {
                        text-align: center;
                    }

                    .menu-item-description {
                        text-align: center;
                        ;
                    }
                }


                /********** Super extra small devices Only :-) (e.g., iPhone 4) **********/
                @media (max-width: 479px) {

                    /* Header */
                    .navbar-brand h1 {
                        /* Restaurant name */
                        padding-top: 5px;
                        font-size: 6vw;
                    }

                    /* End Header */

                    /* Home page */
                    menu-tile,
                    specials-tile {
                        width: 280px;
                        margin: 0 auto 15px;
                    }

                    .col-xxs-12 {
                        position: relative;
                        min-height: 1px;
                        padding-right: 15px;
                        padding-left: 15px;
                        float: left;
                        width: 100%;
                    }
                }
            </style>


</head>
<body>
    <header>
        <nav id="header-nav" class="navbar navbar-default">
            <div class="container">
                <div class="navbar-header">
                    <a href="index.html" class="pull-left visible-md visible-lg">
                        <div id="logo-img" alt="Logo image"></div>
                    </a>

                    <div class="navbar-brand">
                        <a href="index.html">
                            <h1>David Chu's China Bistro</h1>
                        </a>
                        <p>
                            <img src="images/star-k-logo.png" alt="Kosher certification">
                            <span>Kosher Certified</span>
                        </p>
                    </div>

                    <button id="navbarToggle" type="button" class="navbar-toggle collapsed" data-toggle="collapse"
                        data-target="#collapsable-nav" aria-expanded="false">
                        <span class="sr-only">Toggle navigation</span>
                        <span class="icon-bar"></span>
                        <span class="icon-bar"></span>
                        <span class="icon-bar"></span>
                    </button>
                </div>

                <div id="collapsable-nav" class="collapse navbar-collapse">
                    <ul id="nav-list" class="nav navbar-nav navbar-right">
                        <li id="navHomeButton" class="visible-xs active">
                            <a href="index.html">
                                <span class="glyphicon glyphicon-home"></span> Home</a>
                        </li>
                        <li id="navMenuButton">
                            <a href="#" onclick="$dc.loadMenuCategories();">
                                <span class="glyphicon glyphicon-cutlery"></span><br class="hidden-xs"> Menu</a>
                        </li>
                        <li>
                            <a href="#">
                                <span class="glyphicon glyphicon-info-sign"></span><br class="hidden-xs"> About</a>
                        </li>
                        <li>
                            <a href="#">
                                <span class="glyphicon glyphicon-certificate"></span><br class="hidden-xs"> Awards</a>
                        </li>
                        <li id="phone" class="hidden-xs">
                            <a href="tel:410-602-5008">
                                <span>410-602-5008</span></a>
                            <div>* We Deliver</div>
                        </li>
                    </ul><!-- #nav-list -->
                </div><!-- .collapse .navbar-collapse -->
            </div><!-- .container -->
        </nav><!-- #header-nav -->
    </header>

    <div id="call-btn" class="visible-xs">
        <a class="btn" href="tel:410-602-5008">
            <span class="glyphicon glyphicon-earphone"></span>
            410-602-5008
        </a>
    </div>
    <div id="xs-deliver" class="text-center visible-xs">* We Deliver</div>

    <div id="main-content" class="container"></div>

    <footer class="panel-footer">
        <div class="container">
            <div class="row">
                <section id="hours" class="col-sm-4">
                    <span>Hours:</span><br>
                    Sun-Thurs: 11:15am - 10:00pm<br>
                    Fri: 11:15am - 2:30pm<br>
                    Saturday Closed
                    <hr class="visible-xs">
                </section>
                <section id="address" class="col-sm-4">
                    <span>Address:</span><br>
                    7105 Reisterstown Road<br>
                    Baltimore, MD 21215
                    <p>* Delivery area within 3-4 miles, with minimum order of $20 plus $3 charge for all deliveries.
                    </p>
                    <hr class="visible-xs">
                </section>
                <section id="testimonials" class="col-sm-4">
                    <p>"The best Chinese restaurant I've been to! And that's saying a lot, since I've been to many!"</p>
                    <p>"Amazing food! Great service! Couldn't ask for more! I'll be back again and again!"</p>
                </section>
            </div>
            <div class="text-center">&copy; Copyright David Chu's China Bistro 2016</div>
        </div>
    </footer>

    <!-- jQuery (Bootstrap JS plugins depend on it) -->
    <script src="js/jquery-2.1.4.min.js"></script>
    <script src="js/bootstrap.min.js"></script>
    <script src="js/ajax-utils.js"></script>
    <script src="js/script.js"></script>
</body>

</html>
