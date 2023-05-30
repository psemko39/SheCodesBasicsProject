<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>SheCodes Basics Project</title>
    <style>
          body {
           background: linear-gradient(109.6deg, rgb(20, 30, 48) 11.2%, rgb(36, 59, 85) 91.1%);
            color: #fff;
            width: 50%;
            margin: 60px auto;
            font-family: "Cerebri Sans", Arial, Helvetica, sans-serif;
          }

          h1 {
            text-align: center;
            color: #39475b;
          }

          h2 {
            text-align: center;
            color: #DCB45C;
            border: 2px solid #B5802E;
            padding: 15px;
            font-weight: 100;
            font-size: 20px;
            border-radius: 5px;
          }

          img {
            display: block;
            margin: 0 auto;
            max-width: 100%;
            border-radius: 10px;
          }

          p {
            line-height: 1.5;
            font-size: 14px;
            margin: 20px 0 10px;
            color: #FAF8D7;
          }

          button {
            display: block;
            margin: 15px auto;
            background: #222830;
            color:#DCB45C; 
            font-size: 15px;
            padding: 15px 20px;
            border: none;
            border-radius: 10px;
            box-shadow: 5px 5px 5px rgba(0, 0, 0, 0.3);
            transition: 200ms;
          }

          .buy-button:hover {
            opacity: 0.8;
            cursor: pointer;
    
          }

          .container {
            background: #39475B;
            max-width: 650px;
            margin: 0 auto;
            padding: 30px 60px;
            border: 2px solid black;
             box-shadow: 5px 5px 5px rgba(0, 0, 0, 0.3);
          }

          .mission-vision {
            display: block;
            text-align: center;
            font-size: 20px;
            color: #DCB45C;
            font-weight: bold;
          }

          .pillars {
            display: block;
            text-align: center;
            color:#DCB45C;
            font-weight: bold;
          }

          .fma-logo {
            display: block;
            margin: 0 auto;
            max-width: 50%;
            border-radius: 10px;
          }

        .social-media-container {
        display: flex;
        justify-content: center;
        margin-bottom: 10px;
      }

      .social-media {
        display: inline-block;
        padding: 10px;
        text-decoration: none;
        margin: 0 5px;
        color: #B5802E;
      }

      .social-media:hover {
        text-decoration: underline;
      }

      .connect-photo {
        display: block;
            margin: 0 auto;
            max-width: 7%;
            border-radius: 10px;
            margin-top: 200px;
            margin-bottom: 10px;
      }
      

        .footer {
            text-align: center;
            font-size: 12px;
        }

        .author {
            color:#B5802E;
            text-decoration: none;
        }

        .author:hover {
            text-decoration: underline;
        }
    </style>
  </head>
  <body>
    <div class="container">
      <h1>
        <img
          class="fma-logo"
          src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/083/641/original/FMA-logo-transparent.png?1685345622"
          alt="FMA Logo"
        />
      </h1>
      <h2> <strong>CSULB Financial Management Association</strong></h2>

      <hr />

      <img src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/083/648/original/FMA_SpringMixer-5-1-67.jpg?1685348653" alt="Hello" />
      <p>
        <span class="mission-vision"> <strong>Our Mission</strong></span>
        <br />
        To enrich students’ college experience by providing opportunities for
        students to develop professionally, academically, and socially in an
        interactive and enjoyable way.
        <br />
        <br />
        <span class="mission-vision"> <strong> Our Vision </strong></span>
        <br />
        College of Business students at CSULB are able to pursue high quality
        careers by using the resources we offer to create a meaningful and
        stable network during their time here at CSULB.
        <br />
        <br />
      </p>
      <br />
      <button class="buy-button"> <strong>Join FMA Today !</strong></button>

      <img class = "connect-photo" src="https://s3.amazonaws.com/shecodesio-production/uploads/files/000/083/672/original/PngItem_3618777.png?1685353638" 
      alt="connect with us image">
      <div class="social-media-container">
        <a 
        href="https://csulbfma.com/" 
        target="_blank" 
        class="social-media"
        >Website</a
        >
        <a
          href="https://www.linkedin.com/in/fmacsulb/"
          target="_blank"
          class="social-media"
          >Linkedin</a
        >
        <a
          href="https://www.instagram.com/fma_csulb/?hl=en"
          target="_blank"
          class="social-media"
          >Instagram</a
        >
      </div>

      <p class="footer">
        <em>This page was built by
        <a
          class="author"
          href="https://www.linkedin.com/in/penny-semko-8aa136248/"
          target="_blank"
        >
          Penny Semko</em></a
        >
      </p>
    </div>
    <script>
    function join() {
      let name = prompt("What is your name?");
      let email = prompt("What is your email address?");
      let major = prompt("What are you studying?");

      if (name && email && major) {
        alert(
          "Thank you " +
          name +
          "! Please await an email from the Memberships Team and have fun studying " + major + "!"
        );
      } else {
        alert("Please provide all the requested information.");
      }
    }

    let buyButton = document.querySelector(".buy-button");
    buyButton.addEventListener("click", join);
  </script>
  </body>
</html>
