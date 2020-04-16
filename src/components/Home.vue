<template>
  <div class="home">
    <div class="logo-container">
      <h1 class="logo-en">hi·sa·shi</h1>
      <h1 class="logo-jp">ヒ·サ·シ</h1>
    </div>

    <div class="salutation">
      <span class="salutation-big">HELLO!</span>
      <span class="salutation-japanese">こんにちは</span>
    </div>
    <div class="contact">
      <span class="contact-intro"
        >My name is Lionel Koller and I'm a Web Developer from Austria with
        Front-end and UI / UX Design skills. Get in touch with me!
      </span>
      <div class="contact-links">
        <a href="mailto:lionel@hisashi.at">
          <font-awesome-icon :icon="['fas', 'envelope']" size="2x"
        /></a>
        <a
          href="https://www.linkedin.com/in/lionel-koller-088a20108/"
          target="_blank"
          ><font-awesome-icon :icon="['fab', 'linkedin']" size="2x"
        /></a>
      </div>
    </div>
    <img
      class="img-fluid main-image"
      src="../assets/hisashiAT_main_image.png"
      alt="Japanese small street with lines"
    />
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style scoped>
/* XS devices (portrait phones) */
h1 {
  font-weight: 700;
  font-size: 1.8em;
}

a {
  color: black;
}

a:hover {
  color: #7f216c;
}

span {
  font-size: 1.2em;
}

.logo-container h1 {
  text-decoration: none;
  text-align: center;
  display: block;
}

.logo-container,
.logo-en {
  transition: 0.3s;
}

.logo-container {
  height: 35px;
  overflow: hidden;
  width: 200px;
  margin: 10px 0 0 0;
}

.logo-en {
  margin-top: 0;
}

.logo-container:hover .logo-en {
  margin-top: -40px;
}

.logo-jp {
  font-family: "Noto Sans JP", sans-serif;
  font-weight: 700;
}

.salutation {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  position: absolute;
  top: 20%;
  right: 10%;
}

.salutation-big {
  font-size: 4em;
  font-weight: 700;
  text-transform: uppercase;
  line-height: 80px;
}

.salutation-japanese {
  font-family: "Noto Sans JP", sans-serif;
  font-size: 1.5em;
  color: white;
  background: black;
  padding: 1px 3px 1px 3px;
  margin: 0 15px 0 0;
}

.contact {
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 400px;
  left: 10%;
  max-width: 240px;
}

.contact-intro {
  margin: 0 0 20px 0;
}

.contact-links {
  display: flex;
  margin: 0 0 25px 0;
}

.contact-links a:first-child {
  margin: 0 35px 0 0;
}

.main-image {
  position: absolute;
  top: 40%;
}

@media (min-width: 375px) {
  .contact {
    top: 500px;
  }
}

@media (min-width: 500px) {
  .contact {
    top: 350px;
  }
}

/* Small devices (landscape phones) */
@media (min-width: 576px) {
  .contact {
    top: 400px;
  }

  .main-image {
    top: 30%;
  }
}

/* iPhone X */
@media (min-width: 768px) and (max-height: 375px) {
  .contact {
    top: 400px;
    max-width: 300px;
  }
}

/* Medium devices (tablets) */
@media (min-width: 768px) and (min-height: 376px) {
  .salutation {
    top: 15%;
  }

  .salutation-big {
    font-size: 5em;
    line-height: 120px;
  }

  .salutation-japanese {
    font-size: 1.8em;
  }

  .contact {
    top: 600px;
    max-width: 300px;
  }
}

/* Large devices (desktops)  */
@media (min-width: 992px) {
  .contact {
    top: 550px;
  }
  .main-image {
    top: 20%;
  }
}

/* iPad Pro Portrait */
@media (min-width: 1024px) {
  .contact {
    top: 600px;
    max-width: 320px;
  }
}

/* Extra large devices (large desktops) */
@media (min-width: 1200px) {
  .salutation-big {
    font-size: 7em;
    line-height: 120px;
  }

  .contact {
    top: 600px;
  }
}

@media (min-width: 1300px) {
  .contact {
    top: 800px;
    max-width: 400px;
  }
}
</style>
