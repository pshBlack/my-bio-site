<template>
  <main>
    <div class="window" style="margin: 32px; min-width: 680px; height: 100%">
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
          <a
            style="justify-content: center; font-size: 28px; margin-top: 3rem"
            href="#"
            class="name-text"
          >
            &gt; &gt; &gt; Pavlo Vysochynskyi &lt; &lt; &lt;
          </a>
        </div>
        <div style="display: flex; justify-content: center">
          <p style="font-size: 16px" class="description-text">
            Full-Stack & Software Developer, Student Network Engineer
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
            <a
              href="https://discord.com/users/453236302507278348"
              target="_blank"
            >
              <div
                class="hexagon discord"
                style="
                  display: flex;
                  justify-content: center;
                  align-items: center;
                "
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
                style="
                  display: flex;
                  justify-content: center;
                  align-items: center;
                "
              >
                <Linkedin style="color: white" />
              </div>
            </a>
          </div>
          <div class="">
            <a href="https://github.com/pshBlack" target="_blank">
              <div
                class="hexagon github"
                style="
                  display: flex;
                  justify-content: center;
                  align-items: center;
                "
              >
                <Github style="color: white" />
              </div>
            </a>
          </div>
          <div class="">
            <a href="https://t.me/fxpashok" target="_blank">
              <div
                class="hexagon telegram"
                style="
                  display: flex;
                  justify-content: center;
                  align-items: center;
                "
              >
                <Send style="color: white" />
              </div>
            </a>
          </div>

          <div class="">
            <a href="mailto:berezhnogo11@gmail.com">
              <div
                class="hexagon mail"
                style="
                  display: flex;
                  justify-content: center;
                  align-items: center;
                "
              >
                <Mail style="color: white" />
              </div>
            </a>
          </div>
        </div>
        <fieldset
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
          <div class="nav-button"><p>My Projects</p></div>
          <div class="nav-button"><p>About me</p></div>
        </fieldset>
        <fieldset
          style="margin-top: 30px; margin-right: 2px; background-color: #c0c0c0"
        >
          <legend>My CV</legend>
          <iframe
            src="/Pavlo-Vysochynskyi-Resume-ENG.pdf"
            width="100%"
            height="600px"
          />
        </fieldset>
      </div>
    </div>
  </main>
</template>
<script setup lang="js">
import "@/assets/styles/98.css";
import "@/assets/styles/main.css"
import {Linkedin, Github, Send, Mail} from "lucide-vue-next";
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
}

.nav-button:hover {
  cursor: pointer;
  background: #dd5858;
}

.nav-button p {
  text-align: center;
  padding: 0px;
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
  background: #1e3050;
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
