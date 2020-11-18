<template>
  <div id="flip-list-demo" v-on:mouseover="a" v-on:mousemove="a" v-on:mouseout="b">
    <transition-group name="flip-list" tag="ul">
      <li v-for="item in items" :key="item">
        {{ item }}
      </li>
    </transition-group>
  </div>
</template>

<script>

export default {
  data() {
    return {
      state: true,
      items: "voi guat."
    };
  },
  methods: {
    b() {
      this.items = "voi guat.";
    },
    a() {
      this.items = "voigu.at";
    }
  }
};
</script>

<style scoped>
#flip-list-demo {
  display: inline-block;
}

ul {
  cursor: pointer;
  display: inline-block;
  font-weight: bold;
}

ul:hover > li {
  text-decoration: underline;
}

li {
  display: inline-block;
}

.flip-list-move {
  transition: transform 0.8s ease;
}
</style>
