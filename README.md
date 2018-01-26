# button
My cool button (green)
<head>
<link href=https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.0.0-beta/css/bootstrap.min.css rel="stylesheet">

<script>
$(function() {  
  $('#btn-11')
    .on('mouseenter', function(e) {
			var parentOffset = $(this).offset(),
      		relX = e.pageX - parentOffset.left,
      		relY = e.pageY - parentOffset.top;
			$(this).find('span').css({top:relY, left:relX})
    })
    .on('mouseout', function(e) {
			var parentOffset = $(this).offset(),
      		relX = e.pageX - parentOffset.left,
      		relY = e.pageY - parentOffset.top;
    	$(this).find('span').css({top:relY, left:relX})
    });
  $('[href=#]').click(function(){return false});
});
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Open+Sans:400|Raleway:300);
html {
  text-align: center;
  background-color: #eeeeee;
}
html *,
html *:before,
html *:after {
  box-sizing: border-box;
  -webkit-transition: 0.5s ease-in-out;
  transition: 0.5s ease-in-out;
}
html i, html em,
html b, html strong,
html span {
  -webkit-transition: none;
  transition: none;
}

*:before,
*:after {
  z-index: -1 !important;
}


a, a:visited {
  text-decoration: none;
  line-height: 80px;
  color: black;
}

.centerer {
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
  padding: 0 1rem;
}

@media (min-width: 600px) {
  .wrap {
    width: 50%;
    float: left;
  }
}
[id^="btn-"] {
  position: relative;
  display: block;
  overflow: hidden;
  width: 100%;
  height: 80px;
  max-width: 250px;
  margin: 1rem auto;
  text-transform: uppercase;
  border: 1px solid currentColor;
}

@-webkit-keyframes criss-cross-left {
  0% {
    left: -20px;
  }
  50% {
    left: 50%;
    width: 20px;
    height: 20px;
  }
  100% {
    left: 50%;
    width: 375px;
    height: 375px;
  }
}

@keyframes criss-cross-left {
  0% {
    left: -20px;
  }
  50% {
    left: 50%;
    width: 20px;
    height: 20px;
  }
  100% {
    left: 50%;
    width: 375px;
    height: 375px;
  }
}

@-webkit-keyframes criss-cross-right {
  0% {
    right: -20px;
  }
  50% {
    right: 50%;
    width: 20px;
    height: 20px;
  }
  100% {
    right: 50%;
    width: 375px;
    height: 375px;
  }
}
@keyframes criss-cross-right {
  0% {
    right: -20px;
  }
  50% {
    right: 50%;
    width: 20px;
    height: 20px;
  }
  100% {
    right: 50%;
    width: 375px;
    height: 375px;
  }
}
#btn-11 {
  position: relative important!;
  color: #006969;
}
#btn-11:before, #btn-11:after {
  position: absolute;
  top: 50%;
  content: '';
  width: 20px;
  height: 20px;
  background-color: #008282 !important;
  border-radius: 50%;
}
#btn-11:before {
  left: -20px;
  -webkit-transform: translate(-50%, -50%);
          transform: translate(-50%, -50%);
}
#btn-11:after {
  right: -20px;
  -webkit-transform: translate(50%, -50%) ;
          transform: translate(50%, -50%) ;
}
#btn-11:hover {
  color: #ffffff;
}
#btn-11:hover:before {
  -webkit-animation: criss-cross-left 0.8s both;
          animation: criss-cross-left 0.8s both;
  -webkit-animation-direction: alternate;
          animation-direction: alternate;
}
#btn-11:hover:after {
  -webkit-animation: criss-cross-right 0.8s both;
          animation: criss-cross-right 0.8s both;
  -webkit-animation-direction: alternate;
          animation-direction: alternate;
}

</style>
</head>

<body>
<h3>Membership Categories</h3>

Our dues structure and membership options are for Schools, Teachers Continuing Education Providers, Supporters and Allied members:
<ul>
 	<li>Allied- $500 membership for companies that provide products and services to the education sector, as well as other stakeholder organizations in the massage therapy field that wish to support the work of the Alliance</li>
 	<li>Schools- $300 membership for institutions offering entry-level training programs in massage, bodywork, and somatic therapies</li>
 	<li>Continuing Education Providers- $125 membership for those individuals, businesses, or institutions whose primary educational activity is offering post-graduate training</li>
 	<li>Teacher/Administrator- $75 membership </strong>for <em>instructors or administrators</em> in those institutions</li>
 	<li>Supporter - $75 Membership -for individuals who support the work of the Alliance. Supporter members are NOT teachers, school owners, or CE Providers, but wish to be support the mission of the AFMTE</li>
</ul>
When is the best time of year to join the Alliance? ANY TIME! Your membership year begins on the date you first join the organization, so there’s no pro-rating of dues or waiting until the next calendar year comes around. Your annual renewal is due on the anniversary of your original membership. It's pretty simple. Members are welcome to participate in work on most of the Alliance's Committees, serve as committee chairs, vote in elections, and serve on the Board of Directors and Nominating Committee. Click the links below for complete information on the <strong>benefits</strong> of Alliance membership in each category. 

<div class="centerer">
<h1>Allied</h1>
<h1>$500, 15 months</h1>
<h4>See: <a href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&amp;webcode=shopping&amp;prd_key=3c1059e7-a585-4956-bedf-476f1150b17f " target="_blank" rel="noopener">See Benefits</a></h4>
<div class="wrap">

<a id="btn-11" href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&amp;webcode=shopping&amp;prd_key=3c1059e7-a585-4956-bedf-476f1150b17f">Allied</a>

<a id="btn-11" style="text-decoration: none;" href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&amp;webcode=shopping&amp;prd_key=3c1059e7-a585-4956-bedf-476f1150b17f">Allied</a>

</div>
</div>
<table style="width:100%"></table>

<section class="header-hero hfeed site">
<div class="hero-wrapper">
<div class="hero-bg" style="background: url('https://images.unsplash.com/photo-1453847668862-487637052f8a?dpr=1&amp;auto=compress,format&amp;fit=crop&amp;w=1948&amp;h=&amp;q=80&amp;cs=tinysrgb&amp;crop=');"></div>
<div class="overlay"></div>
<div class="container">
<div class="row">
<div class="col-md-7"><header class="entry-header">
<h1 class="page-title custom_box_title">Who We Are</h1>
<p class="custom_box_paragraph">The Alliance for Massage Therapy Education is an independent organization that has been established by educators, for educators. Recognizing the diverse nature of our field, membership in the Alliance is open to all who work in the many disciplines across the spectrum of massage, bodywork, and somatic therapies.</p>

</header></div>
</div>
</div>
</div>
<div class="breadcrumbs-wrapper-line"></div>
</section>
<p style="text-align: center;"><a title="Click Here For School Member Information" href="https://www.afmte.org/membership/school/" target="_blank" rel="noopener">School</a> | <a title="Click Here For CE Provider Member Information" href="https://www.afmte.org/membership/ce/" target="_blank" rel="noopener">CE Provider</a> | <a title="Click Here For Teacher Member Information" href="https://www.afmte.org/membership/teacher/" target="_blank" rel="noopener">Teacher</a> | <a href="https://www.afmte.org/membership/supporter/">Supporter </a>| <a title="Click Here For Allied Member Information" href="https://www.afmte.org/about/allied-members/" target="_blank" rel="noopener">Allied</a> | <a href="https://www.afmte.org/membership/allied-member-directory/">Allied Member Directory</a> | <a href="https://www.afmte.org/membership/school-member-directory/">School Member Directory</a> | <a title="Click Here To Join The Alliance" href="https://www.afmte.org/membership/join/" target="_blank" rel="noopener">JOIN </a></p>

<style>
#nav {
    display: none;
}

#footer-widgeted {
    display: none;
} 
</style>

<style>

body {
    font-family: "Open Sans", sans-serif;
    min-height: 100vh;
    min-width: 320px; 
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale; 
}

/*Typography*/

/*Page Header*/
.header-hero {
    position: relative;
    z-index: 2;
    overflow: hidden;
    background-color: #008282;
}
.hero-wrapper {
    padding: 90px 0;
}
.header-hero .hero-bg {
    position: absolute;
    top: 0px;
    width: 100%;
    height: 110%;
    background-size: cover !important;
    background-repeat: no-repeat !important;
    background-position: center center !important;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
    z-index: -1;
}
.header-hero .overlay {
    position: absolute;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 100%;
    background-image: -webkit-gradient(linear,left top, right bottom,from(#8DBDC1),to(#8CA65F));
    background-image: linear-gradient(to bottom right,#002727,#327272);
    opacity: .6; 
} 

.custom_box_title { 

    line-height: 70px !important;
    letter-spacing: .5px !important;
    font-weight: 500 !important;
    font-style: normal !important;
    color: #fff !important;
    font-size: 40px !important;
    position:relative;
    left: -15%;
    z-index:4;
    border-bottom: none !important;
}


.custom_box_paragraph {
     border:none !important;
    font-size: 14px !important;
    color: #fff !important;
    font-weight: 500 !important; 
    line-height: 1.55em !important;
    margin: 0px;
    position: relative;
    z-index: 4;
    border:none !important;
     text-align:left;
width:500;
margin-left:50px;
}

h1,
h3 {
  font-family: "Raleway", "Open Sans", sans-serif !important;
  margin: 0 !important;
  line-height: 1 !important;
}
</style>
</body>
