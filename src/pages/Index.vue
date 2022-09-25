<template>
  <Layout>

    <div class="carte">
        <h1>Maël Aramion</h1>
        <div class="img"></div>
        <p>Licence professionnelle MIAW, Web Developper</p>
        <div class="link-container">
          <a href="mailto:mael.aramio@gmail.com">mael.aramion@gmail.com</a>
        </div>
    </div>
  </Layout>
</template>

<script>
export default {
  icon: './src/favicon.png',
  metaInfo: {
    title: 'Maël Aramion',
    meta: [
      {
        name: 'Maël Aramion',
        content: 'Carte de visite'
      }
    ]
  }
}
</script>

<style>
@font-face {
  font-family: 'font1';
  src: url("/src/fonts/font1.ttf");
}
body{
  font-family: font1, sans-serif;
  background: #2f3640;
  color: #fbc531;
}
.img{
  width: 200px;
  height: 200px;
  border: 3px solid #fbc531;
  margin: auto;
  background-image: url("../images/moi.jpg");
  background-position: center;
  background-size: cover;
  border-radius: 150px;
}
.carte{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  border: 2px solid #fbc531;
  padding: 15px 100px;
  border-radius: 10px;
  z-index: 999;
  box-shadow: 10px 10px;
}
h1{
  text-align: center;
  text-transform: uppercase;
}
li{
  list-style: none  ;
}
.link-container{
  display: flex;
}
a{
  color: #7f8fa6  ;
  text-decoration: none;
  text-align: center;
  margin: auto;
}
a:hover{
  color: #fbc531;
  transition: 0.5s all;
}
</style>
