<script setup>
defineProps({
  subject: {
    type: String,
    required: true
  },
  //0000 - 2359
  start: {
    type: Number,
    required: true
  },
  end: {
    type: Number,
    required: true
  },
  type: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="subject quadsubject" v-if="type==='quad'">
    <h1 class="title">{{ subject }}</h1>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <p class="time">{{ start }} - {{ end }}</p>
    <p class="day">{{ day }}</p>
  </div>
  <div class="subject doublesubject" v-else-if="type==='double'">
    <h1 class="title">{{ subject }}</h1>
    <br>
    <br>
    <p class="time">{{ start }} - {{ end }}</p>
    <p class="day">{{ day }}</p>
  </div>
  <div class="subject fullsubject" v-else-if="type==='full'">
    <h1 class="title">{{ subject }}</h1>
    <br>
    <p class="time">{{ start }} - {{ end }}</p>
    <p class="day">{{ day }}</p>
  </div>
  <div class="subject halfsubject" v-else-if="type === 'half'">
    <h1 class="title">{{ subject }}</h1>
    <p class="time">{{ start }} - {{ end }}</p>
    <p class="day">{{ day }}</p>
  </div>
  <div class="error" v-else>
    <h1 class="title">Error</h1>
    <p class="time">Error</p>
    <p class="day">Error</p>
  </div>
</template>
<style scoped>
.quadsubject {
  background-color: #f1f1f1;
  border: 1px solid black;
  border-radius: 5px;
  padding: 5px;
  margin: 5px;
  width: 100%;
  height: 100%;
  color: rgb(0, 0, 0);

}
.doublesubject {
  background-color: #f1f1f1;
  border: 1px solid black;
  border-radius: 5px;
  padding: 5px;
  margin: 5px;
  width: 100%;
  height: 100%;
  color: rgb(0, 0, 0);

}
.fullsubject {
  background-color: #f1f1f1;
  border: 1px solid black;
  border-radius: 5px;
  padding: 5px;
  margin: 5px;
  width: 100%;
  height: 100%;
  color: black;;
}

.halfsubject {
  background-color: #f1f1f1;
  border: 1px solid black;
  border-radius: 5px;
  padding: 5px;
  margin: 5px;
  width: 100%;
  height: 100%;
  color: black; 
}

.subject {
  text-align: center;
}
.error {
  color: red;
}
</style>
