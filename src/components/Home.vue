<template>
  <body>
    <header>
      <div class="share-button"></div>
    </header>
    <div class="container">
      <div class="image-container">
        <img
          src="../assets/images/sanplast-avatar.jpg"
          alt="Sanplast Logo Avatar"
        />
      </div>
      <h1>@sanplastindustrialtda</h1>

      <a class="tile" href="">
        <div class="icon">
          <font-awesome-icon :icon="['fas', 'house']" size="lg"/>
        </div>
        <p>Sanplast</p>
        <div class="tile-share-button"></div>
      </a>
      <a class="tile" href="">
        <div class="icon">
          <font-awesome-icon :icon="['fab', 'linkedin']" size="xl" />
        </div>
        <p>Linkedin</p>
        <div class="tile-share-button"></div>
      </a>
      <a class="tile" href="">
        <div class="icon">
          <font-awesome-icon :icon="['fab', 'facebook']" size="xl"/>
        </div>
        <p>Facebook</p>
        <div class="tile-share-button"></div>
      </a>
    </div>
  </body>
</template>

<script setup></script>

<style>
body {
  margin: 0;
  padding: 0;
  background: white;
  color: black;
  display: flex;
  align-items: center;
  flex-direction: column;
  width: 100vw;
}

header {
  width: 95%;
  max-width: 788px;
  display: flex;
  justify-content: flex-end;
  padding: 12px;
  margin-top: 15px;
}

.share-button {
  width: 40px;
  height: 40px;
  border-radius: 20px;
  background-color: black;
}

.container {
  width: 91%;
  max-width: 680px;
  margin: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  font-size: 20px;
  margin-bottom: 30px;
}

a {
  text-decoration: none;
  color: white;
}

.tile {
  width: 100%;
  height: 56px;
  background-color: rgb(37, 37, 37);
  margin: 7px;
  border-radius: 17px;
  display: flex;
  justify-content: space-between;
}

.tile-share-button {
  margin: 8px;
  width: 40px;
  height: 40px;
  border-radius: 20px;
  background-color: rgb(52, 52, 52);
}

.image-container {
  height: 96px;
  width: 96px;
  border-radius: 48px;
  overflow: hidden;
}

.image-container img {
  height: 100%;
}

.icon {
  margin: 16px 10px;
  width: 44px;
  height: 44px;
}
</style>
