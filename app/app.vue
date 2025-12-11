<template>
  <main>
    <div
      class="window"
      style="margin: 32px; min-width: 680px; max-width: 730px; height: 100%"
    >
      <NavigationBar />
      <NuxtPage style="margin: 0px 7px 12px 7px" />
    </div>
  </main>
</template>
<script setup lang="js">
import "@/assets/styles/98.css";
</script>
<style>
main {
  display: flex;
  justify-content: center;
  align-items: center;
}

.nav-button {
  width: 220px;
  font-size: 14px;
  font-weight: bolder;
  margin: 5px 10px;
  background: #f2f2f2;
  box-shadow: 6px 5px #808080;
  transition: background 0.3s;
  text-decoration: none;
}

.nav-button:hover {
  cursor: pointer;
  background: #dd5858;
}

.nav-button p {
  text-align: center;
  padding: 0px;
  color: var(--dialog-black);
  font-weight: bold;
}

.background {
  background-repeat: no-repeat;
  background-size: cover; /* або contain */
}
.hexagon {
  height: 50px; /* adjust to control the size  */
  aspect-ratio: cos(30deg);
  clip-path: polygon(-50% 50%, 50% 100%, 150% 50%, 50% 0);
  background: #353535;
  transition: background 0.3s, translate 0.3s;
  cursor: pointer;
}
.hexagon.discord:hover {
  background: #5d69f2;
}
.hexagon.linkedin:hover {
  background: #0a66c2;
}
.hexagon.telegram:hover {
  background: #2da7e2;
}
.hexagon.github:hover {
  background: #171a18;
}
.hexagon.mail:hover {
  background: #c5221e;
}
.hexagon:hover {
  translate: 0 -10px;
}

@media screen and (max-width: 600px) {
  .description-text {
    font-size: 10px !important;
  }
  .window {
    min-width: 350px !important;
  }
  .name-text {
    font-size: 20px !important;
  }

  .nav-fieldset {
    flex-direction: column !important;
    gap: 15px !important;
  }
  .nav-button {
    margin: 0px 0px !important;
    width: 100% !important;
    gap: 0px !important;
  }
  .hexagon {
    height: 40px !important;
  }
  .nav-button p {
    font-size: 14px !important;
  }
  .title-bar-text {
    font-size: 8px !important;
  }
}
</style>
