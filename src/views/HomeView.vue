<script setup lang="ts">
// import images
import magic_Hogwarts_Crest from "../assets/magic-Hogwarts-Crest.png";
import Dumbledore_image from "../assets/邓布利多.jpg";
import McGonagall_image from "../assets/麦格教授.jpg";
import Snape_image from "../assets/斯内普教授.jpg";
import Hagrid_image from "../assets/海格.jpg";
import study_magic1 from "../assets/study-magic-1.jpg";
import study_magic2 from "../assets/study-magic-2.jpg";
import study_magic3 from "../assets/study-magic-3.jpg";

// styles
const teacher_image_style = {
  width: "100px",
  height: "100px",
  borderRadius: "50%",
};

const Hogwarts_Crest_style = {
  width: "100px",
  height: "100px",
  borderRadius: "50%",
};

const study_magic_style = {
  width: "auto",
  height: "300px",
};


</script>
<template>
  <div class="home">
    <div class="magic-container">
      <div class="magic-header">
        <!-- 校徽 -->
        <img :src="magic_Hogwarts_Crest" :style="Hogwarts_Crest_style" />
        <!-- 菜单 同学录、课程、教师名录 -->
        <div class="magic-links">
          <router-link to="/courses" class="magic-link">课程</router-link>
          <router-link to="/students" class="magic-link">同学录</router-link>
          <router-link to="/teachers" class="magic-link">教师名录</router-link>
          <router-link to="/students" class="magic-link">办理入学</router-link>
        </div>
      </div>
      <!-- banner图 -->
      <div class="magic-image">
        <!-- 欢迎标题 -->
        <h1 class="magic-title">欢迎来到霍格沃茨</h1>
      </div>

      <!-- 学校简介 -->
      <h2>学校概况</h2>
      <div class="magic-school">
        <p>霍格沃茨魔法学校（Hogwarts School of Witchcraft and
          Wizardry）是一所位于苏格兰高地的魔法学校，是英国魔法界最负盛名的魔法学校之一。霍格沃茨是一所七年制的学校，从11岁到18岁的巫师和女巫可以在这里接受魔法教育。
        </p>
        <p>
          霍格沃茨的校训是“Draco dormiens nunquam titillandus”（拉丁文，意为“不要挠醒睡着的龙”），校徽上有四个学院的标志，分别是格兰芬多、赫奇帕奇、拉文克劳和斯莱特林。
        </p>
      </div>

      <!-- 大巫师 -->
      <h2>最受欢迎的教师</h2>
      <div class="grand-wizard">
        <div class="grand-sorcerer">
          <img :src="Dumbledore_image" :style="teacher_image_style" />
          <p>阿不思·邓布利多（Albus Dumbledore）是霍格沃茨的校长，他是一位非常有智慧的巫师，也是一位非常有爱心的人。他是霍格沃茨的创始人之一，也是格兰芬多学院的创始人。</p>
        </div>

        <div class="grand-sorcerer">
          <img :src="McGonagall_image" :style="teacher_image_style" />
          <p>米勒娃·麦格教授（Minerva McGonagall）是霍格沃茨的副校长，她是一位非常严格的老师，但是她也是一位非常有爱心的人。她是霍格沃茨的创始人之一，也是格兰芬多学院的创始人。</p>
        </div>

        <div class="grand-sorcerer">
          <img :src="Snape_image" :style="teacher_image_style" />
          <p>西弗勒斯·斯内普（Severus Snape）是霍格沃茨的魔药学教授，他是一位非常有才华的巫师，但是他也是一位非常复杂的人。他是霍格沃茨的创始人之一，也是格兰芬多学院的创始人。</p>
        </div>

        <div class="grand-sorcerer">
          <img :src="Hagrid_image" :style="teacher_image_style" />
          <p>鲁伯特·海格（Rubeus Hagrid）是霍格沃茨的魔法生物学教授，他是一位非常善良的巫师，但是他也是一位非常激进的人。他是霍格沃茨的创始人之一，也是格兰芬多学院的创始人。</p>
        </div>
      </div>

      <!-- 入学指南 -->
      <h2>入学指南</h2>
      <div class="magic-school">
        <p>霍格沃茨魔法学校每年都会举行一次入学仪式，新生们会在这里接受魔法师的教育。如果你想成为一名优秀的巫师或女巫，那么你就应该来霍格沃茨魔法学校学习魔法。</p>
        <p>如果你想成为一名优秀的巫师或女巫，那么你就应该来霍格沃茨魔法学校学习魔法。霍格沃茨魔法学校是一所非常有名的魔法学校，它是英国魔法界最负盛名的魔法学校之一。</p>
        <div class="study_magic">
          <img :src="study_magic1" :style="study_magic_style">
          <img :src="study_magic2" :style="study_magic_style">
          <img :src="study_magic3" :style="study_magic_style">
        </div>
      </div>

      <!-- 明星课程 -->
      <h2>课程安排</h2>
      <div class="magic-class">
        <p>霍格沃茨魔法学校有很多优秀的课程，比如魔法学、魔药学、魔法生物学、魔法历史等等。这些课程都是由一些非常有才华的老师来教授的，他们都是一些非常有爱心的人。</p>
        <p>以下为必修课程：</p>
        <div class="cur-classes">
          <span>黑魔法防御术</span>
          <span>变形术</span>
          <span>符咒学</span>
          <span>魔药学</span>
          <span>药草学</span>
          <span>天文学</span>
          <span>魔法史</span>
          <span>飞行学</span>
        </div>
      </div>

      <!-- 页尾 -->
      <div class="footer">
        <p>2024 Hogwarts School of Witchcraft and Wizardry</p>
        <p>Designed by Harry Potter</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.magic-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #000;
  color: #fff;
}

.magic-header {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  padding: 1rem;
}

.magic-title {
  font-size: 3rem;
  margin-bottom: 2rem;
}


.magic-image {
  width: 80%;
  height: 400px;
  background: url("../assets/home.jpg") no-repeat;
  animation: move 30s linear 0s infinite;
}

@keyframes move {
  0% {
    background-position: 0 0;
  }

  40% {
    background-position: 50% 50%;
  }

  60% {
    background-position: 50% 50%;
  }

  100% {
    background-position: 0 0;
  }
}

.magic-links {
  display: flex;
  gap: 1rem;
}

.magic-link {
  font-size: 1.5rem;
  color: #fff;
  text-decoration: none;
  padding: 0.5rem 1rem;
  border: 1px solid #fff;
  border-radius: 5px;
}

.magic-school {
  width: 80%;
  margin: 2rem;
}

.grand-wizard {
  width: 80%;
  margin: 2rem;
  display: flex;
  flex-direction: row;
  gap: 1rem;
}

.grand-sorcerer {
  height: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  align-items: center;
}


.study_magic {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 1rem;
  margin-top: 2rem;
}

.magic-class {
  width: 80%;
  margin: 2rem;
}

.cur-classes {
  display: flex;
  flex-direction: row;
  gap: 1rem;
}

.footer {
  font-size: 0.8rem;
  width: 80%;
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  gap: 1rem;
  align-items: center;
  padding: 1rem;
  background-color: #000;
  color: #fff;
}
</style>
