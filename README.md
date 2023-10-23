# Lab4Web
<h1 align="center"> Pertanyaan Dan Tugas </h1>

![image](https://github.com/hafizalkariem/ProjectUAS/assets/115614957/cf87474a-05a3-41dc-be8b-6e8be7af1a47)

Dalam Ketentuan tugas tersebut kita disuruh untuk membuat layout baru untuk menu about dan menu kontak. dimana di bagian about kita disuruh untuk membuat single layout dengan isian deskripsi,portofolio dll. adapun untuk layout kontak kita disuruh untuk membuat form dengan isi email,message,nama dll. berikut jawaban dari tugas tugas berikut

## About Menu
<h2 align="center"> HTML </h2>

```html

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>About Me</title>
    <link rel="stylesheet" href="style.css" />
    <style>
      body {
        line-height: 1;
        font-size: 100%;
        font-family: "Open Sans", sans-serif;
        color: #5a5a5a;
        min-height: 1250px;
      }
    </style>

    <!-- script feather icons -->
    <script src="https://unpkg.com/feather-icons"></script>
  </head>
  <body>
    <div id="about-content">
      <div id="about-sidebar">
        <section>
          <div class="about-img">
            <img src="DSCF5703.JPG" alt="profil" />
          </div>
          <div class="bio">
            <h3>Ahmad Hapizhudin</h3>
            <p>Santri/designer/gamers from Bekasi</p>
          </div>
          <div class="about-widget">
            <ul>
              <li><a href="home.html">Home</a></li>
              <li><a href="artikel.html">Artikel</a></li>
              <li><a href="about.html" class="active">About</a></li>
              <li><a href="kontak.html">Kontak</a></li>
            </ul>
          </div>
          <div class="about-footer">
            <p>&copy; 2023 - Universitas Pelita Bangsa</p>
          </div>
        </section>
      </div>
      <div>
        <section id="about-main">
          <div class="Text">
            <h1 class="top">I am</h1>
            <h1 class="bottom"><i>'THE CREATOR'</i></h1>
            <p class="about-quotes">
              <i> "Berhentilah sekolah dan mulailah belajar"</i>
            </p>

            <div class="feather-icons">
              <a
                href="https://instagram.com/hafizkariem?igshid=OGQ5ZDc2ODk2ZA=="
              >
                <i data-feather="instagram" class="icon-lg"></i>
              </a>
              <a href="https://www.facebook.com/fyzz.fyzz.77?mibextid=2JQ9oc">
                <i data-feather="facebook" class="icon-lg"></i>
              </a>
              <a href="https://www.facebook.com/fyzz.fyzz.77?mibextid=2JQ9oc">
                <i data-feather="twitter" class="icon-lg"></i>
              </a>
              <a href="https://www.facebook.com/fyzz.fyzz.77?mibextid=2JQ9oc"
                ><i data-feather="linkedin" class="icon-lg"></i
              ></a>

              <a href="https://www.facebook.com/fyzz.fyzz.77?mibextid=2JQ9oc"
                ><i data-feather="discord" class="icon-lg"></i
              ></a>
            </div>
          </div>
          <div class="image">
            <img src="aru-transformed.png" alt="mookrom" />
          </div>
          <script>
            feather.replace();
          </script>
        </section>
      </div>
    </div>
  </body>
</html>

```

<h2 align="center"> CSS </h2>

```css
/* About */
* {
  margin: 0;
  padding: 0;
}
#about-sidebar {
  position: fixed;
  display: block;
  align-items: center;
  background-color: #f3f5f9;
  float: left;
  width: 260px;
  min-height: 100vh;
  box-shadow: 0 0 1em #cccccc;
  /* background-image: linear-gradient(to top, #fffcfc, #77777c); */
  background-image: linear-gradient(240deg, #b8b3b3, #dadde2, #f3f5f9);
}
.about-img {
  justify-content: center;
  display: flex;
  margin-top: 20px;
}
.about-img img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 3px #1d1d1d;
  object-fit: cover;
  object-position: 0 50%;
}

#about-content h3 {
  text-decoration: none;
}
.bio {
  margin-top: 15px;
  padding: 20px;
}
.about-widget {
  justify-content: center;
  display: flex;
}
.about-widget ul {
  list-style-type: none;
}
.about-widget li {
  padding-top: 20px;
  padding-bottom: 10px;
  font-size: 20px;
  font-family: sans-serif;
}
.about-widget li a {
  text-decoration: none;
  color: #5a5a5a;
}
.about-widget li a.active,
.about-widget ul li a:hover {
  color: #ffffff;
}
.about-footer {
  margin-top: 66px;

  padding: 10px 15px;
  box-shadow: 0 0 1em #cccccc;
}
.about-footer p {
  font-size: 15px;
  text-align: center;
}

/* about main */

#about-main {
  display: flex;
  margin-left: 260px;
  background-color: #f1f1f1;
  width: 1089px;
  height: 100vh;
  background-size: cover;
}
.Text {
  margin-top: 150px;
  position: relative;
  padding-left: 100px;
  padding-right: 0px;
  padding-top: 50px;
  font-family: "montserrat";
  z-index: 1;
}
.Text h1.top {
  font-size: 50px;
  color: #000000;
  letter-spacing: 2px;
}
.Text h1.bottom {
  font-size: 50px;
  color: #000000;
  letter-spacing: 2px;
  font-weight: bold;
}
.about-quotes {
  color: black;
  margin-top: 10px;
}
.about-quotes i {
  font-size: 24px;
  font-weight: bold;
}

.feather-icons {
  display: flex;
  margin: 10px;
  margin-left: 0px;
}
.feather-icons svg {
  margin: 5px;
}
.icon-lg {
  width: 40px;
  height: 40px;
}
.feather-icons a {
  color: #0c0b0b;
}
.feather-icons a:hover {
  color: #968f8f;
}
.image img {
  width: 620px;
  height: 100vh;
}

```

<b>Hasilnya</b>
![Screenshot 2023-10-22 210107](https://github.com/hafizalkariem/ProjectUAS/assets/115614957/7c8638f5-5cf9-4666-9e70-02d4b79a84ad)

## Kontak Menu

<h2 align="center"> HTML </h2>

```html
<div id="contact-container">
        <div class="contact-content">
          <div class="contact-person">
            <h1>contact</h1>
            <p>ahmadhapiz224@gmail.com</p>
            <p>+6282226221535</p>
            <p>Bekasi, Jawa Barat</p>
          </div>
          <div class="contact-form">
            <h1>Pesan & Saran</h1>
            <section>
              <form action="form.php" method="post">
                <p>
                  <label for="nama">Nama</label>
                  <input type="text" id="nama" name="nama" />
                </p>
                <p>
                  <label for="alamat email">Email</label>
                  <input type="email" id="Email" name="Email" />
                </p>
                <p>
                  <label for="message">message</label>
                  <textarea
                    name="message"
                    id="message"
                    cols="30"
                    rows="10"
                  ></textarea>
                </p>
                <p><input type="submit" value="kirim" /></p>
              </form>
            </section>
          </div>
          <div class="contact-visit">
            <h1>Visit</h1>
            <div class="visit-youtube">
              <p>Always visit my youtube channel</p>
              <a
                href="https://www.youtube.com/channel/UC_6t_LNvrYb0MQFlBLbvGwg"
              >
                <img src="Youtube_logo.png" alt="logo youtube" />
              </a>
            </div>
          </div>
        </div>
      </div>
```

<h2 align="center"> CSS </h2>


```css
#contact-container {
  position: relative;
  margin-left: 260px;
  width: 1089px;
  height: 100vh;
  overflow: hidden;
  background-image: url(DSC08724.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  position: absolute;
  z-index: 1; /* Ubah z-index ke 1 */
}

#contact-container::before {
  content: "";
  background-image: url(DSC08724.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  position: relative;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.2);
  z-index: 0; /* Ubah z-index ke 0 */
}

.contact-content {
  display: flex;
  justify-content: space-between;
  position: center;
  height: 100vh;
  align-items: flex-start;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
  backdrop-filter: blur(10px);
  z-index: 2;
}

.contact-content h1 {
  margin-bottom: 20px;
}
.contact-content p {
  margin-bottom: 20px;
}

.contact-content h1 {
  font-size: 40px;
  color: white;
}
.contact-content p {
  color: #ffffff;
}
.contact-person .contact-form .contact-visit {
  flex: 1;
  margin: 0 10px;
}

/* contact person start */
.contact-person {
  text-align: center;
  margin-top: 100px;
}
.contact-person h1 .contact-person p {
  display: inline-block;
  margin-top: 20px;
  margin-bottom: 20px;
}
.contact-person h1 {
  margin-bottom: 40px;
}
.contact-person p {
  margin: 40px;
  color: white;
}

/* contact person end */

/* pesan dan saran start */
.contact-form {
  margin-top: 100px;
}
.contact-message section form {
  display: flex;
  flex-direction: column;
  max-width: 300px;
  margin: 0 auto;
  padding: 20px;
  background-color: #f5f5f5;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
}
.contact-message label {
  font-weight: bold;
  margin-bottom: 5px;
}
.contact-form p {
  margin: 20px;
  min-width: 300px;
}
.contact-form h1 {
  text-align: center;
}
input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 5px;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
  background-color: transparent;
}
input[type="submit"] {
  background-color: #007bff;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 18px;
}

input[type="submit"]:hover {
  background-color: #0056b3;
}
/* pesan dan saran end */

/* visit start */

.contact-visit {
  text-align: center;
  margin-top: 100px;
  margin-right: 40px;
}
.visit-youtube img {
  width: 100px;
  height: 50px;
}

/* visi end */

```

<b>Hasilnya</b>

![Screenshot 2023-10-23 231302](https://github.com/hafizalkariem/ProjectUAS/assets/115614957/60680bad-30bc-4499-8e77-384010626479)



