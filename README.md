btn

<html>
  <head>
    <link
      rel="stylesheet"
      href="https://s3-us-west-2.amazonaws.com/s.cdpn.io/85807/font-awesome.css"
    />
    <!-- css style starts here -->
    <style>
      .clearfix {
        display: inline-block;
      }
      .clearfix:after {
        visibility: hidden;
        display: block;
        font-size: 0;
        content: " ";
        clear: both;
        height: 0;
      }

      * html .clearfix {
        height: 1%;
      }

      .clearfix {
        display: block;
      }

      body {
        padding: 30px 20px 20px 20px;
        font-family: "Montserrat", sans-serif;
		background-color: #92a8d1;
        background-image: -webkit-gradient(
          linear,
          left top,
          right bottom,
          color-stop(0, #222),
          color-stop(0.61, #ededed)
		 
        );
		
        background-image: -o-linear-gradient(right bottom, #222 0%, #444 61%);
        background-image: -moz-linear-gradient(right bottom, #222 0%, #444 61%);
        background-image: -webkit-linear-gradient(
          right bottom,
          #222 0%,
          #444 61%
        );
        background-image: -ms-linear-gradient(right bottom, #222 0%, #444 61%);
        background-image: linear-gradient(
          to right bottom,
          #222222 0%,
          #444444 61%
        );
      }

      a {
        text-decoration: none;
        color: #0198e1;
      }

      .divider {
        width: 100%;
        float: left;
      }
      .divider:after {
        position: absolute;
        width: 100%;
        margin-top: 0px;
        bottom: -11px;
        left: -3px;
        background: #595959;
        content: "";
        display: block;
        -moz-transform: skew(-31deg, 0deg);
        -ms-transform: skew(-31deg, 0deg);
        -webkit-transform: skew(-31deg, 0deg);
        transform: skew(-31deg, 0deg);
        height: 11px;
      }

      .contOut {
        opacity: 0;
        width: 100%;
        max-width: 1080px;
        margin: 0 auto;
        background: #fff;
        position: relative;
        overflow: visible;
        margin-bottom: 6px;
      }
      .contOut:before {
        position: absolute;
        width: 6px;
        margin-top: 6px;
        left: -6px;
        background: #8c8c8c;
        content: "";
        display: block;
        -moz-transform: skew(0deg, -61deg);
        -ms-transform: skew(0deg, -61deg);
        -webkit-transform: skew(0deg, -61deg);
        transform: skew(0deg, -61deg);
        height: 100%;
      }
      .contOut .contIn {
        width: 100%;
        float: left;
      }
      .contOut .contIn .section {
        padding-left: 30px;
        padding-right: 30px;
      }
      .contOut .contIn .section.top {
        padding-top: 30px;
        padding-bottom: 15px;
      }
      .contOut .contIn .section.top:hover img {
        -webkit-filter: grayscale(0%);
        filter: grayscale(0%);
      }
      .contOut .contIn .logoCont {
        float: left;
        width: 15%;
      }
      .contOut .contIn .logoCont .logo {
        width: 100%;
        max-width: 100px;
        min-width: 50px;
        height: auto;
        min-height: 50px;
        -webkit-filter: grayscale(100%);
        filter: grayscale(100%);
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px;
        border-radius: 2px;
        border: solid 1px #cccccc;
      }
      .contOut .contIn h1 {
        width: 45%;
        float: left;
        display: inline-block;
        font-family: "Playfair Display", serif;
        margin: -6px 0 0 0;
        font-size: 40px;
        line-height: 40px;
      }
      .contOut .contIn p.tagline {
        float: left;
        width: 45%;
        font-size: 14px;
      }
      .contOut .contIn p.tagline span {
        color: #999999;
      }
      .contOut .contIn .moreInfo {
        float: right;
        width: 40%;
        text-align: right;
      }
      .contOut .contIn .moreInfo p {
        margin: 0;
        line-height: 20px;
        word-wrap: break-word;
      }

      .middle {
        padding-top: 20px;
        padding-bottom: 20px;
      }
      .middle h2 {
        border-left: solid 0 #fff;
        -moz-transition: all 200ms ease-in;
        -o-transition: all 200ms ease-in;
        -webkit-transition: all 200ms ease-in;
        transition: all 200ms ease-in;
      }
      .middle h2 i.fa {
        display: inline-block;
        margin-left: 10px;
      }
      .middle h2 i.fa:hover {
        cursor: pointer;
        color: #0176ae;
      }
      .middle:hover h2 {
        border-left: solid 10px black;
        padding-left: 8px;
        -moz-transition: all 100ms ease-in;
        -o-transition: all 100ms ease-in;
        -webkit-transition: all 100ms ease-in;
        transition: all 100ms ease-in;
      }
      .middle .job {
        width: 100%;
        float: left;
      }
      .middle .job h2 {
        margin: 0;
      }
      .middle .job h2 span {
        float: right;
        display: inline-block;
        font-size: 16px;
        background: black;
        color: #fff;
        padding: 6px 8px;
        min-width: 120px;
        text-align: center;
      }
      .middle .job p {
        margin: 6px 0;
      }
      .middle .job p .brag {
        display: inline-block;
        margin: 10px 0;
        font-style: italic;
        background: #dbdbdb;
        padding: 20px 20px 20px 50px;
        color: #333;
        text-align: justify;
        border-bottom: solid 1px #bfbfbf;
        position: relative;
        text-shadow: 0 1px 1px #fff;
        max-height: 40px;
      }
      .middle .job p .brag:before {
        position: absolute;
        left: 0;
        top: 0;
        content: "";
        width: 0;
        height: 0;
        border-top: 40px solid transparent;
        border-bottom: 40px solid transparent;
        border-left: 40px solid #fff;
      }

      .skills {
        width: 49%;
        display: block;
        float: left;
        padding-bottom: 20px;
      }
      .skills h3 {
        margin: 20px 20px 10px 20px;
        text-transform: uppercase;
        position: relative;
      }
      .skills h3 .fa {
        position: absolute;
        top: -4px;
        right: 0;
        padding: 4px;
        -moz-border-radius: 3px;
        -webkit-border-radius: 3px;
        border-radius: 3px;
      }
      .skills ul {
        font-size: 14px;
        list-style: none;
        margin: 0;
        padding: 0 20px;
      }
      .skills ul li {
        float: left;
        padding: 4px 6px;
        margin: 0 4px 4px 0;
      }
      .skills ul li.light {
        opacity: 0.6;
      }
      .skills.odd {
        margin-right: 2%;
      }
      .skills.code {
        background: #0198e1;
      }
      .skills.code .fa {
        background: #30bbfe;
        -moz-box-shadow: inset 0 1px 2px #003149;
        -webkit-box-shadow: inset 0 1px 2px #003149;
        box-shadow: inset 0 1px 2px #003149;
      }
      .skills.code li {
        background: #016fa4;
        text-shadow: 0 1px 1px #0198e1;
      }
      .skills.code li:hover {
        background: #0183c3;
      }
      .skills.code li.prim {
        text-shadow: none;
        background: #004262;
        color: #fff;
        clear: left;
      }
      .skills.software {
        background: #608341;
      }
      .skills.software .fa {
        background: #86b060;
        -moz-box-shadow: inset 0 1px 2px #151d0e;
        -webkit-box-shadow: inset 0 1px 2px #151d0e;
        box-shadow: inset 0 1px 2px #151d0e;
      }
      .skills.software li {
        background: #425a2d;
        text-shadow: 0 1px 1px #608341;
      }
      .skills.software li:hover {
        background: #516f37;
      }
      .skills.software li.prim {
        text-shadow: none;
        background: #222e17;
        color: #fff;
        clear: left;
      }

      ul.buttons {
        margin: 0;
        padding: 0;
        list-style: none;
      }
      ul.buttons li {
        float: left;
        text-align: center;
        display: inline-block;
        width: 32%;
        margin-right: 1%;
        -moz-border-radius: 2px;
        -webkit-border-radius: 2px;
        border-radius: 2px;
        position: relative;
        margin-bottom: 8px;
      }
      ul.buttons li a {
        display: inline-block;
        padding: 10px 0;
        color: #fff;
      }
      ul.buttons li:last-child {
        margin-right: 0;
        background: #8b4513;
        border-bottom: solid 3px #311807;
        -moz-transition: all 100ms ease-in-out;
        -o-transition: all 100ms ease-in-out;
        -webkit-transition: all 100ms ease-in-out;
        transition: all 100ms ease-in-out;
        width: 33%;
      }
      ul.buttons li:last-child:hover {
        background: #b85b19;
        border-bottom: solid 3px #753a10;
        -moz-transition: all 200ms ease-in-out;
        -o-transition: all 200ms ease-in-out;
        -webkit-transition: all 200ms ease-in-out;
        transition: all 200ms ease-in-out;
      }
      ul.buttons li:nth-child(1) {
        background: #b5509c;
        border-bottom: solid 3px #702f60;
        -moz-transition: all 100ms ease-in-out;
        -o-transition: all 100ms ease-in-out;
        -webkit-transition: all 100ms ease-in-out;
        transition: all 100ms ease-in-out;
      }
      ul.buttons li:nth-child(1):hover {
        background: #c474b0;
        border-bottom: solid 3px #a6468e;
        -moz-transition: all 200ms ease-in-out;
        -o-transition: all 200ms ease-in-out;
        -webkit-transition: all 200ms ease-in-out;
        transition: all 200ms ease-in-out;
      }
      ul.buttons li:nth-child(2) {
        background: #608341;
        border-bottom: solid 3px #2e3f1f;
        -moz-transition: all 100ms ease-in-out;
        -o-transition: all 100ms ease-in-out;
        -webkit-transition: all 100ms ease-in-out;
        transition: all 100ms ease-in-out;
      }
      ul.buttons li:nth-child(2):hover {
        background: #79a552;
        border-bottom: solid 3px #547239;
        -moz-transition: all 200ms ease-in-out;
        -o-transition: all 200ms ease-in-out;
        -webkit-transition: all 200ms ease-in-out;
        transition: all 200ms ease-in-out;
      }
      ul.buttons li:nth-child(3) {
        background: #0198e1;
        border-bottom: solid 3px #01537b;
        -moz-transition: all 100ms ease-in-out;
        -o-transition: all 100ms ease-in-out;
        -webkit-transition: all 100ms ease-in-out;
        transition: all 100ms ease-in-out;
        margin-right: 0;
        width: 33%;
      }
      ul.buttons li:nth-child(3):hover {
        background: #17b3fe;
        border-bottom: solid 3px #0187c8;
        -moz-transition: all 200ms ease-in-out;
        -o-transition: all 200ms ease-in-out;
        -webkit-transition: all 200ms ease-in-out;
        transition: all 200ms ease-in-out;
      }
      ul.buttons li:nth-child(4) {
        background: #ff6103;
        border-bottom: solid 3px #9c3a00;
        -moz-transition: all 100ms ease-in-out;
        -o-transition: all 100ms ease-in-out;
        -webkit-transition: all 100ms ease-in-out;
        transition: all 100ms ease-in-out;
      }
      ul.buttons li:nth-child(4):hover {
        background: #ff8136;
        border-bottom: solid 3px #e95700;
        -moz-transition: all 200ms ease-in-out;
        -o-transition: all 200ms ease-in-out;
        -webkit-transition: all 200ms ease-in-out;
        transition: all 200ms ease-in-out;
      }
      ul.buttons li:nth-child(5) {
        background: #444;
        border-bottom: solid 3px #111111;
        -moz-transition: all 100ms ease-in-out;
        -o-transition: all 100ms ease-in-out;
        -webkit-transition: all 100ms ease-in-out;
        transition: all 100ms ease-in-out;
      }
      ul.buttons li:nth-child(5):hover {
        background: #5e5e5e;
        border-bottom: solid 3px #373737;
        -moz-transition: all 200ms ease-in-out;
        -o-transition: all 200ms ease-in-out;
        -webkit-transition: all 200ms ease-in-out;
        transition: all 200ms ease-in-out;
      }

      @media (max-width: 1010px) {
        .contOut .contIn h1,
        .contOut .contIn p.tagline {
          width: 42%;
          margin-left: 3%;
        }

        .skills.code,
        .skills.software {
          width: 100%;
        }

        .skills.code {
          margin-bottom: 10px;
        }

        ul.buttons li {
          width: 48%;
          margin-bottom: 10px;
        }
        ul.buttons li:nth-child(3),
        ul.buttons li:last-child {
          width: 48%;
        }

        ul.buttons li:nth-child(even) {
          float: right;
          margin-right: 0;
        }
      }
      @media (max-width: 850px) {
        .middle .job p .brag {
          padding-left: 70px;
          max-height: 60px;
        }
        .middle .job p .brag:before {
          border-top: 50px solid transparent;
          border-bottom: 50px solid transparent;
          border-left: 50px solid #fff;
        }

        .contOut .contIn .logoCont {
          width: 35%;
        }
        .contOut .contIn .logoCont .logo {
          max-width: 200px;
        }
        .contOut .contIn h1 {
          width: 62%;
          float: right;
          text-align: right;
          margin-bottom: 10px;
        }
        .contOut .contIn .moreInfo {
          width: 60%;
        }
        .contOut .contIn p.tagline {
          clear: left;
          width: 30%;
          margin: 0;
        }
      }
      .contracts {
        width: 100%;
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
        box-sizing: border-box;
        padding: 20px 30px;
      }
      .contracts h3 {
        margin: 0 0 20px 0;
      }
      .contracts .contract {
        -moz-box-sizing: border-box;
        -webkit-box-sizing: border-box;
        box-sizing: border-box;
        padding: 10px;
        width: 24%;
        min-height: 160px;
        background: #ffc;
        border: solid 1px #ffff99;
        -moz-box-shadow: 0 1px 2px #999;
        -webkit-box-shadow: 0 1px 2px #999;
        box-shadow: 0 1px 2px #999;
        color: #333300;
        float: left;
        margin-right: 1%;
        margin-bottom: 10px;
        position: relative;
        padding-bottom: 15px;
      }
      .contracts .contract h4 {
        margin: 0;
      }
      .contracts .contract p.desc {
        font-size: 14px;
        color: #4d4d00;
        word-wrap: break-word;
      }
      .contracts .contract p.desc a:hover {
        text-decoration: underline;
      }
      .contracts .contract span.date {
        position: absolute;
        bottom: 5px;
        right: 5px;
        font-size: 12px;
        color: #999900;
      }

      @media (max-width: 800px) {
        .contracts .contract {
          width: 49%;
        }
      }
      @media (max-width: 620px) {
        .middle .job p .brag {
          padding-left: 80px;
          max-height: 80px;
        }
        .middle .job p .brag:before {
          border-top: 60px solid transparent;
          border-bottom: 60px solid transparent;
          border-left: 60px solid #fff;
        }
      }
      @media (max-width: 570px) {
        .middle .job p .brag {
          padding-left: 90px;
          max-height: 100px;
        }
        .middle .job p .brag:before {
          border-top: 70px solid transparent;
          border-bottom: 70px solid transparent;
          border-left: 70px solid #fff;
        }

        ul.buttons li {
          width: 100%;
          margin-right: 0;
        }
        ul.buttons li:nth-child(3),
        ul.buttons li:last-child {
          width: 100%;
        }

        .skills ul li {
          float: none;
        }

        .contOut .contIn h1 {
          font-size: 34px;
        }

        .contracts .contract {
          width: 100%;
          margin-right: 0;
        }
      }
      @media (max-width: 500px) {
        .middle .job p .brag {
          padding-left: 20px;
          max-height: none;
        }
        .middle .job p .brag:before {
          border-top: none;
          border-bottom: none;
          border-left: none;
        }

        .middle .job h2 span {
          margin-top: 10px;
        }

        .contOut .contIn h1 {
          font-size: 28px;
        }
        .contOut .contIn .moreInfo {
          font-size: 14px;
        }
      }
      @media (max-width: 450px) {
        .contOut .contIn .moreInfo,
        .contOut .contIn p.tagline {
          font-size: 12px;
        }
      }
      .sm {
        list-style: none;
        position: absolute;
        top: 10px;
        right: 30px;
        margin: 0;
      }
      .sm li {
        display: inline-block;
        float: left;
        margin-left: 6px;
      }
      .sm li a {
        color: #ccc;
      }
      .sm li a:hover {
        color: #fff;
      }

      @import url("https://fonts.googleapis.com/css?family=Josefin+Sans");

* {
  font-family: "Josefin Sans", sans-serif;
}

.wrapper {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  max-width: 350px;
  width: 100%;
  background: #fff;
  padding: 25px;
  border-radius: 5px;
  box-shadow: 4px 4px 2px rgba(254, 236, 164, 1);
}

.wrapper h2 {
  text-align: center;
  margin-bottom: 20px;
  text-transform: uppercase;
  letter-spacing: 3px;
  color: #332902;
}

.input_field {
  margin-bottom: 10px;
}

 .input_field input[type="text"],
 textarea {
  border: 1px solid #e0e0e0;
  width: 100%;
  padding: 10px;
}

 textarea {
  resize: none;
  height: 80px;
}

 .btn input[type="submit"] {
  border: 0px;
  margin-top: 15px;
  padding: 10px;
  text-align: center;
  width: 100%;
  background: #00ffff;
  color: #000000;
  text-transform: uppercase;
  letter-spacing: 5px;
  font-weight: bold;
  border-radius: 25px;
  cursor: pointer;
}

#error_message {
  margin-bottom: 20px;
  background: #fe8b8e;
  padding: 0px;
  text-align: center;
  font-size: 14px;
  transition: all 0.5s ease;
}

    </style>
    <!-- css style ends here -->
  </head>
  <div class="contOut clearfix">
    <div class="contIn">
      <div class="section top clearfix">
        <div class="logoCont">
          <!img src="test.jpg" width=100 height=100>
          
        </div>
        <h1 style="color:SlateBlue;">Ravi Kumar</h1>
        <div class="moreInfo">
          <p>
            House no.15<br />Main road<br />Namkum-(W),Ranchi-835103<br />ravikumar@gmail.com<br />
             +91 92684638856<br /><a href="http://onelittledesigner.com" target="_blank"
              ></a
            >
          </p>
        </div>
        <p class="tagline">
          <br />Tools Admin<br />(Monitoring Tools)<br />
        </p>
      </div>
      <div class="divider"></div>
    </div>
  </div>
  <div class="contOut clearfix">
    <div class="contIn">
      <div class="section middle clearfix">
        <div class="job">
          <h2 style="color:Tomato;">
            Career Profile
          </h2>
          <p>
            <strong>Position: </strong>Tools Administrator<br /><strong
              >Description: </strong
            >I am monitoring tools Administrator.
            <br /><span class="brag"
              >I am working in Wipro SPGI team from last 3 years, have been working on multiple monitoring technology- Scom, APM, Sitescope, Service Now and Datadog</span
            >
          </p>	
        </div>
      </div>
      <div class="divider"></div>
    </div>
  </div>
  <div class="contOut clearfix">
    <div class="contIn">
      <div class="section middle clearfix">
        <div class="job">
          <h2 style="color:Tomato;">
            Experience Summary
          </h2>
          <p>
            <strong>Position: </strong>Tools Administrator<br /><strong
              >Description: </strong
            >Monitoring Tools Administrator
            <br /><ul>
                <li>Working on multiple monitoring tools like-com, APM, Sitescope, Service Now and Datadog </li>
               <li>Serving as a hands-on subject matter expert in configuring monitoring setup for the different calss of servers like- Windows, Linux and AWS</li>
               <li>Good knowledge on functionality of monitoring tools</li>
               </ul>  
          </p>
        </div>
      </div>
      <div class="divider"></div>
    </div>
  </div>
  <div class="contOut clearfix">
    <div class="contIn">
      <div class="section middle clearfix">
        <div class="job">
          <h2 style="color:Tomato;">
            Skills
          </h2>
          <p>
            <strong>Position: </strong>Tools Administrator<br /><strong
              >Description: </strong
            >Monitoring Tools Administrator 
             <br /><ul><li>Excellent verbal, interpersonal, and written communication skills</li>
<li>Team player with the ability to work in a fast-paced environment</li>
<li>Strong analytical, problem-solving and decision making capabilities</li>
<li>Strong contributer towards setting up monitoring configuraton on Windows, Linux and AWS servers</li>
</ul>
          </p>
        </div>
      </div>
      <div class="divider"></div>
    </div>
  </div>
  <div class="contOut clearfix">
    <div class="contIn">
      <div class="section middle clearfix">
        <div class="job">
          <h2 style="color:Tomato;">
            Responsibility Handled
          </h2>
          <p>
 <ul><li>Always ready to support</li>
<li>Knowledge sharing among Team Members</li>
<li>Always completing task before given time</li>
<li>Responsible to support teams always</li>
</ul>
          </p>
        </div>
      </div>
      <div class="divider"></div>
    </div>
  </div>
  <div class="contOut clearfix">
    <div class="contIn">
      <div class="section middle clearfix">
        <div class="job">
          <h2 style="color:Tomato;">
            Acadmic summary
          </h2>
          <p>
              <span class="brag"
              >Bachelor of Computer Science | Ranchi University, Jharkhand | 2014-17</br>     
               High school | St. Aloysius High School, Ranchi</br> 
              </span>
          </p>
        </div>
      </div>
      <div class="divider"></div>
    </div>
  </div>
  <div class="contOut clearfix half">
    <div class="contIn">
      <div class="section middle clearfix">
        <h2 style="color:Tomato;">
          Contact Me
        </h2>
        <div id="error_message">
     
        </div>
        <form action="" id="myform" onsubmit = "return validate();">
          <div class="input_field">
              <input type="text" placeholder="Name" id="name">
          </div>
          <div class="input_field">
              <input type="text" placeholder="Address" id="subject">
          </div>
          <div class="input_field">
              <input type="text" placeholder="Phone" id="phone">
          </div>
          <div class="input_field">
              <input type="text" placeholder="Email" id="email">
          </div>
          <div class="input_field">
              <textarea placeholder="Message" id="message"></textarea>
          </div>
          <div class="btn">
              <input type="submit">
          </div>
        </form>
      </div>
      <div class="divider"></div>
    </div>
  </div>
  <!-- jquery starts here -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
  <script>
    $(window).load(function () {
      // Page Load Anim
      $(".contOut").animate(
        {
          opacity: "1",
        },
        1200
      );
      // Jobs Accordion
      $(".fa-plus").closest(".job").find("p").slideUp();
      $(".openBtn").on("click", function () {
        if ($(this).hasClass("open")) {
          $(this)
            .removeClass("open")
            .removeClass("fa-minus")
            .addClass("fa-plus");
          $(this)
            .closest(".job")
            .find("p")
            .animate(
              {
                opacity: "0",
              },
              200
            )
            .slideUp();
        } else {
          $(this).addClass("open").removeClass("fa-plus").addClass("fa-minus");
          $(this).closest(".job").find("p").slideDown().animate(
            {
              opacity: "1",
            },
            400
          );
        }
      });
    });
  </script>

  <script>
    function validate(){
  var name = document.getElementById("name").value;
  var subject = document.getElementById("subject").value;
  var phone = document.getElementById("phone").value;
  var email = document.getElementById("email").value;
  var message = document.getElementById("message").value;
  var error_message = document.getElementById("error_message");
  
  error_message.style.padding = "10px";
  
  var text;
  if(name.length < 3){
    text = "Please Enter valid Name";
    error_message.innerHTML = text;
    return false;
  }
  if(subject.length < 10){
    text = "Please Enter more than 10 Characters in address";
    error_message.innerHTML = text;
    return false;
  }
  if(isNaN(phone) || phone.length != 10){
    text = "Please Enter valid Phone Number";
    error_message.innerHTML = text;
    return false;
  }
  if(email.indexOf("@") == -1 || email.length < 6){
    text = "Please Enter valid Email";
    error_message.innerHTML = text;
    return false;
  }
  if(message.length <= 140){
    text = "Please Enter More Than 140 Characters in message";
    error_message.innerHTML = text;
    return false;
  }
  alert("Thankyou!");
  return true;
}
  </script>
  <!-- jquery ends here -->
</html>
