<template>
  <div class="title-bar">
    <div
      class="title-bar-text"
      style="font-size: 9px; letter-spacing: 1px; user-select: none"
    >
      File Explorer - C:/Users/Pablo/My-Cool-Resume.html
    </div>
    <div class="title-bar-controls">
      <button aria-label="Minimize"></button>
      <button aria-label="Maximize"></button>
      <button aria-label="Close"></button>
    </div>
  </div>
  <hr style="color: var(--dialog-black)" />
  <div class="window-body">
    <div style="display: flex; justify-content: center">
      <NuxtLink
        to="/"
        style="justify-content: center; font-size: 28px; margin-top: 3rem"
        class="name-text"
      >
        &gt; &gt; &gt; Pavlo Vysochynskyi &lt; &lt; &lt;
      </NuxtLink>
    </div>
    <div style="display: flex; justify-content: center">
      <p style="font-size: 16px" class="description-text">
        Vue & React Frontend Developer, UX/UI Designer, Network Engineer Student
      </p>
    </div>
    <div
      style="
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 20px;
      "
    >
      <div class="">
        <a href="https://discord.com/users/453236302507278348" target="_blank">
          <div
            class="hexagon discord"
            style="display: flex; justify-content: center; align-items: center"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="26"
              height="26"
              fill="white"
              class="bi bi-discord"
              viewBox="0 0 16 16"
            >
              <path
                d="M13.545 2.907a13.2 13.2 0 0 0-3.257-1.011.05.05 0 0 0-.052.025c-.141.25-.297.577-.406.833a12.2 12.2 0 0 0-3.658 0 8 8 0 0 0-.412-.833.05.05 0 0 0-.052-.025c-1.125.194-2.22.534-3.257 1.011a.04.04 0 0 0-.021.018C.356 6.024-.213 9.047.066 12.032q.003.022.021.037a13.3 13.3 0 0 0 3.995 2.02.05.05 0 0 0 .056-.019q.463-.63.818-1.329a.05.05 0 0 0-.01-.059l-.018-.011a9 9 0 0 1-1.248-.595.05.05 0 0 1-.02-.066l.015-.019q.127-.095.248-.195a.05.05 0 0 1 .051-.007c2.619 1.196 5.454 1.196 8.041 0a.05.05 0 0 1 .053.007q.121.1.248.195a.05.05 0 0 1-.004.085 8 8 0 0 1-1.249.594.05.05 0 0 0-.03.03.05.05 0 0 0 .003.041c.24.465.515.909.817 1.329a.05.05 0 0 0 .056.019 13.2 13.2 0 0 0 4.001-2.02.05.05 0 0 0 .021-.037c.334-3.451-.559-6.449-2.366-9.106a.03.03 0 0 0-.02-.019m-8.198 7.307c-.789 0-1.438-.724-1.438-1.612s.637-1.613 1.438-1.613c.807 0 1.45.73 1.438 1.613 0 .888-.637 1.612-1.438 1.612m5.316 0c-.788 0-1.438-.724-1.438-1.612s.637-1.613 1.438-1.613c.807 0 1.451.73 1.438 1.613 0 .888-.631 1.612-1.438 1.612"
              />
            </svg>
          </div>
        </a>
      </div>
      <div class="">
        <a
          href="https://www.linkedin.com/in/pavlo-vysochynskyi-2069a3331/"
          target="_blank"
        >
          <div
            class="hexagon linkedin"
            style="display: flex; justify-content: center; align-items: center"
          >
            <Linkedin style="color: white" />
          </div>
        </a>
      </div>
      <div class="">
        <a href="https://github.com/pshBlack" target="_blank">
          <div
            class="hexagon github"
            style="display: flex; justify-content: center; align-items: center"
          >
            <Github style="color: white" />
          </div>
        </a>
      </div>
      <div class="">
        <a href="https://t.me/fxpashok" target="_blank">
          <div
            class="hexagon telegram"
            style="display: flex; justify-content: center; align-items: center"
          >
            <Send style="color: white" />
          </div>
        </a>
      </div>

      <div class="">
        <a href="mailto:berezhnogo11@gmail.com">
          <div
            class="hexagon mail"
            style="display: flex; justify-content: center; align-items: center"
          >
            <Mail style="color: white" />
          </div>
        </a>
      </div>
    </div>
    <!-- <fieldset
      style="
        margin-top: 15px;
        background-color: #c0c0c0;
        display: flex;
        justify-content: center;
        gap: 50px;
      "
      class="nav-fieldset"
    >
      <legend>Navigation</legend>
      <NuxtLink to="/projects" class="nav-button"
        ><div><p>My Projects</p></div></NuxtLink
      >
      <NuxtLink to="/about" class="nav-button"
        ><div><p>About me</p></div></NuxtLink
      >
    </fieldset> -->
  </div>
</template>
<script setup lang="js">
import "@/assets/styles/98.css";
import {Linkedin, Github, Send, Mail} from "lucide-vue-next";
</script>
<style scoped></style>
