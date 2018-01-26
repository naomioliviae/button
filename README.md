<head>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<script src="https://code.jquery.com/jquery-2.2.4.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.3/umd/popper.min.js" integrity="sha384-vFJXuSJphROIrBnz7yo7oB41mKfc8JzQZiCq4NCceLEaO4IHwicKwpJf9c9IpFgh" crossorigin="anonymous"></script>

<script>
$(document).ready(function() {

  $(".toggle-accordion").on("click", function() {
    var accordionId = $(this).attr("accordion-id"),
      numPanelOpen = $(accordionId + ' .collapse.in').length;
    
    $(this).toggleClass("active");

    if (numPanelOpen == 0) {
      openAllPanels(accordionId);
    } else {
      closeAllPanels(accordionId);
    }
  })

  openAllPanels = function(aId) {
    console.log("setAllPanelOpen");
    $(aId + ' .panel-collapse:not(".in")').collapse('show');
  }
  closeAllPanels = function(aId) {
    console.log("setAllPanelclose");
    $(aId + ' .panel-collapse.in').collapse('hide');
  }
     
});
</script>

<style type="text/css">
body {
  color: #6a6c6f;
  background-color: #f7f7f7;
  font-size: 15px;
}

.container {
  max-width: 960px;
}

.panel-default>.panel-heading {
  color: #333;
  background-color: #fff;
  border-color: #e4e5e7;
  padding: 0;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.panel-default>.panel-heading a {
  display: block;
  padding: 10px 15px;
}

.panel-default>.panel-heading a:after {
  content: "";
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: 400;
  line-height: 0;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  float: right;
  transition: transform .25s linear;
  -webkit-transition: -webkit-transform .25s linear;
}

.panel-default>.panel-heading a[aria-expanded="true"] {
  background-color: #eee;
}

.panel-default>.panel-heading a[aria-expanded="true"]:after {
  content: "\2212";
  -webkit-transform: rotate(180deg);
  transform: rotate(180deg);
}

.panel-default>.panel-heading a[aria-expanded="false"]:after {
  content: "\002b";
  -webkit-transform: rotate(90deg);
  transform: rotate(90deg);
}

.accordion-option {
  width: 100%;
  float: left;
  clear: both;
  margin: 15px 0;
}

.accordion-option .title {
  font-size: 20px;
  font-weight: bold;
  float: left;
  padding: 0;
  margin: 0;
}

.accordion-option .toggle-accordion {
  float: right;
  font-size: 16px;
  color: #6a6c6f;
}

.accordion-option .toggle-accordion:before {
  content: "Expand All";
}

.accordion-option .toggle-accordion.active:before {
  content: "Collapse All";
}

#nav {
    display: none;
}

#footer-widgeted {
    display: none;
} 

body {
    font-family: "Open Sans", sans-serif;
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
    font-size: 50px !important;
    position:relative;
     text-align:center;
     width:100%;
    margin-left:15%;
    z-index:4;
    border-bottom: none !important;
}


.custom_box_paragraph {
     border:none !important;
    font-size: 18px !important;
    color: #fff !important;
    font-weight: 400 !important; 
    line-height: 1.55em !important;
    margin: 0px;
    position: relative;
    z-index: 4;
    border:none !important;
     text-align:left;
     width:100%;
    margin-left:15%;

}

h1,
h3 {
  font-family: "Raleway", "Open Sans", sans-serif !important;
  margin: 0 !important;
  line-height: 1 !important;
}
</style>

</head>


<body>
<div class="container">
<div class="accordion-option">
    <h3 class="title">Join today and receive an additional 3 months of membership!</h3>
    <a href="javascript:void(0)" class="toggle-accordion active" accordion-id="#accordion"></a>
  </div>

</div>
<div class="clearfix"></div>
<div id="accordion" class="panel-group" role="tablist" aria-multiselectable="true">
<div class="panel panel-default">
<div id="headingOne" class="panel-heading" role="tab">
<h4 class="panel-title"><a role="button" href="#collapseOne" data-toggle="collapse" data-parent="#accordion" aria-expanded="false" aria-controls="collapseOne">
Allied Membership, $500 for 15 months
</a></h4>
</div>
<div id="collapseOne" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingOne">
<ul>
 	<li class="panel-body">CE Directory: Announce workshops, webinars or educational opportunities.
Advertise on the Alliance Website: Receive year-round exposure in our Allied Member Directory with a hot-linked logo.</li>
 	<li class="panel-body">Advertising Discounts: Receive advertising discounts with MASSAGE Magazine and Massage Today
AFMTE Member Logo: Download the membership logo</li>
 	<li class="panel-body">2019 Educational Congress Discounts: Save $100 on registration for the 2019 Educational Congress. Exhibitors and Sponsors receive additional member discounts.</li>
 	<li class="panel-body">Voting Rights: Vote at our Annual Business Meetings.</li>
</ul>

<div class="container">

<a href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&webcode=shopping&prd_key=3c1059e7-a585-4956-bedf-476f1150b17f&utm_campaign=assessmentguide15for12&utm_source=SMA"><button class="btn-3">Get Allied Membership</button></a>
</div>

</div>
</div>
<div class="panel panel-default">
<div id="headingTwo" class="panel-heading" role="tab">
<h4 class="panel-title"><a class="collapsed" role="button" href="#collapseTwo" data-toggle="collapse" data-parent="#accordion" aria-expanded="true" aria-controls="collapseTwo">
School Membership, $300 for 15 months
</a></h4>
</div>
<div id="collapseTwo" class="panel-collapse collapse in" role="tabpanel" aria-labelledby="headingTwo">
<ul>
 	<li class="panel-body">Advertise on the Alliance Website: Receive year-round exposure in our School Member Directory with a hot-linked logo.</li>
 	<li class="panel-body">CE Directory: Access our continuing education course directory to announce CE courses, workshops, webinars or educational opportunities</li>
 	<li class="panel-body">Online Training Center: Receive online training through MaxKnowledge including a free training course and discounts on additional courses</li>
 	<li class="panel-body">Advertising Discounts: Receive advertising discounts with MASSAGE Magazine and Massage Today</li>
 	<li class="panel-body">AFMTE Member Logo: Use the membership logo</li>
 	<li class="panel-body">2019 Educational Congress Discounts: Save $100 on registration for the 2019 Educational Congress. Exhibitors and Sponsors receive additional member discounts.</li>
 	<li class="panel-body">Voting Rights: Vote at our Annual Business Meetings.</li>
</ul>
<div class="container">

<a href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&webcode=shopping&prd_key=03222371-a1cc-4dfa-9280-9859db73bd51&utm_campaign=assessmentguide15for12&utm_source=SMA"><button class="btn-3">Get School Membership</button></a>
</div>

</div>
</div>
<div class="panel panel-default">
<div id="headingThree" class="panel-heading" role="tab">
<h4 class="panel-title"><a class="collapsed" role="button" href="#collapseThree" data-toggle="collapse" data-parent="#accordion" aria-expanded="false" aria-controls="collapseThree">
CE Provider Membership, $125 for 15 months
</a></h4>
</div>
<div id="collapseThree" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingThree">
<ul>
 	<li class="panel-body">CE Directory: Access our continuing education course directory to announce CE courses, workshops, webinars or educational opportunities</li>
 	<li class="panel-body">Online Training Center: Receive online training through MaxKnowledge including a free training course and discounts on additional courses</li>
 	<li class="panel-body">AFMTE Member Logo: Use the membership logo</li>
 	<li class="panel-body">2019 Educational Congress Discounts: Save $100 on registration for the 2019 Educational Congress. Exhibitors and Sponsors receive additional member discounts.</li>
 	<li class="panel-body">Voting Rights: Vote at our Annual Business Meetings.</li>
</ul>
<div class="container">

<a href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&webcode=shopping&prd_key=63f3b8ce-77bf-48b3-80dd-75cfaef79cb5&utm_campaign=assessmentguide15for12&utm_source=SMA"><button class="btn-3">Get CE Provider Membership</button></a>
</div>
</div>
</div>
<div class="panel panel-default">
<div id="headingFour" class="panel-heading" role="tab">
<h4 class="panel-title"><a class="collapsed" role="button" href="#collapseFour" data-toggle="collapse" data-parent="#accordion" aria-expanded="false" aria-controls="collapseFour">
Teacher Membership, $75 for 15 months
</a></h4>
</div>
<div id="collapseFour" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingFour">
<ul>
 	<li class="panel-body">Teacher Education Resource Directory: Access our searchable database of educational resources that help massage therapy and bodywork teachers achieve competency in the TESP standards and submit resources for possible inclusion.</li>
 	<li class="panel-body">Online Training Center: Receive online training through MaxKnowledge including a free training course and discounts on additional courses</li>
 	<li class="panel-body">AFMTE Member Logo: Use the membership logo</li>
 	<li class="panel-body">2019 Educational Congress Discounts: Save $100 on registration for the 2019 Educational Congress. Exhibitors and Sponsors receive additional member discounts.</li>
 	<li class="panel-body">Voting Rights: Vote at our Annual Business Meetings.</li>
</ul>
<div class="container">

<a href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&webcode=shopping&prd_key=3e3e96bc-b060-494a-9303-95c284f3fd10&utm_campaign=assessmentguide15for12&utm_source=SMA"><button class="btn-3">Get Teacher Membership</button></a>
</div>
</div>
</div>
<div class="panel panel-default">
<div id="headingFour" class="panel-heading" role="tab">
<h4 class="panel-title"><a class="collapsed" role="button" href="#collapseFive" data-toggle="collapse" data-parent="#accordion" aria-expanded="false" aria-controls="collapseFive">
Supporter Membership, $75 for 15 months
</a></h4>
</div>
<div id="collapseFive" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingFive">
<ul>
 	<li class="panel-body">Teacher Education Resource Directory: Access our searchable database of educational resources that help massage therapy and bodywork teachers achieve competency in the TESP standards and submit resources for possible inclusion.</li>
 	<li class="panel-body">Online Training Center: Receive online training through MaxKnowledge including a free training course and discounts on additional courses</li>
 	<li class="panel-body">AFMTE Member Logo: Use the membership logo</li>
 	<li class="panel-body">2019 Educational Congress Discounts: Save $100 on registration for the 2019 Educational Congress. Exhibitors and Sponsors receive additional member discounts.</li>
 	<li class="panel-body">Voting Rights: Vote at our Annual Business Meetings.</li>
</ul>
<div class="container">

<a href="https://netforum.avectra.com/eweb/shopping/shopping.aspx?site=afmte&webcode=shopping&prd_key=52fd6a4f-d885-4cfd-a657-a337ae1c8eb5&utm_campaign=assessmentguide15for12&utm_source=SMA"><button class="btn-3">Get Supporter Membership</button></a>
</div>
</div>
</div>
</div>
<h3>Membership Categories</h3>
Our dues structure and membership options are for Schools, Teachers Continuing Education Providers, Supporters and Allied members:
<ul>
 	<li>Allied- $500 membership for companies that provide products and services to the education sector, as well as other stakeholder organizations in the massage therapy field that wish to support the work of the Alliance</li>
 	<li>Schools- $300 membership for institutions offering entry-level training programs in massage, bodywork, and somatic therapies</li>
 	<li>Continuing Education Providers- $125 membership for those individuals, businesses, or institutions whose primary educational activity is offering post-graduate training</li>
 	<li>Teacher/Administrator- $75 membership for <em>instructors or administrators</em> in those institutions</li>
 	<li>Supporter - $75 Membership -for individuals who support the work of the Alliance. Supporter members are NOT teachers, school owners, or CE Providers, but wish to be support the mission of the AFMTE</li>
</ul>
When is the best time of year to join the Alliance? ANY TIME! Your membership year begins on the date you first join the organization, so there’s no pro-rating of dues or waiting until the next calendar year comes around. Your annual renewal is due on the anniversary of your original membership. It's pretty simple. Members are welcome to participate in work on most of the Alliance's Committees, serve as committee chairs, vote in elections, and serve on the Board of Directors and Nominating Committee. Click the links below for complete information on the <strong>benefits</strong> of Alliance membership in each category.

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

</div>

<style>@import url(https://fonts.googleapis.com/css?family=Open+Sans:400|Raleway:400);
html {

  background-color: #eeeeee;
  margin-top: 0px !important;
}

#nav {
    display: none;
}

.sociable {
    display: none;
}

#footer-widgeted {
    display: none;
} 

#content h4 {
	font-family: Raleway;
	font-weight: 600;
	font-size: 18px;
	text-align: center;
	}
</style>

<style>


.container {
  padding: 2em;
}

/* GENERAL BUTTON STYLING */
button,
button::after {
  -webkit-transition: all 0.3s;
	-moz-transition: all 0.3s;
  -o-transition: all 0.3s;
	transition: all 0.3s;
}

button {
  background: #16723c;
  border: 2px solid #2e8150;
  border-radius: 5px;
  color: #F7F7F7;
  display: block;
  overflow: hidden;
  font-size: 1.3em;
  font-family: Raleway;
  font-weight: 600;
  width: 100%;
  height: 80px;
  max-width: 650px;
  margin: 1em auto;
  padding: 1.4em 8em;
  position: relative;
  text-transform: uppercase;
}

button::before,
button::after {
  background: #F7F7F7;
  opacity: .6;
  content: '';
  position: absolute;
  z-index: 1;
}

button:hover {
  color: #F7F7F7;
}



/* BUTTON 3 */
.btn-3::after {
  height: 0;
  left: 50%;
  top: 50%;
  width: 0;
}

.btn-3:hover:after {
  height: 100%;
  left: 0;
  top: 0;
  width: 100%;
}
a:link {
    text-decoration: none;
}

a:visited {
    text-decoration: none;
}

a:hover {
    text-decoration: none;
}

a:active {
    text-decoration: underline;
    color: #00a250;
}

#content .page ul li {
    margin: 5px 0px 5px 50px;
}

</body>


</body>
