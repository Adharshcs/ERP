<template>
  <nav class="navbar">
    <div class="logo">PECONNECT</div>
    <div class="nav-item">
      <p>HOME</p>
      <i class="fa fa-home"></i>
    </div>
    <div class="nav-item">
      <p>ATTENDANCE</p>
      <i class="fas fa-calendar-week"></i>
    </div>
    <div class="nav-item">
      <p>ACADEMICS</p>
      <i class="fas fa-book-reader"></i>
    </div>
    <div class="nav-item">
      <p>MATERIALS</p>
      <i class="fa fa-book"></i>
    </div>
    <div class="nav-item setting">
      <p>THEME</p>
      <i class="fa fa-sun"></i>
    </div>
    
    <!-- <div
      :class="{ selected: currentPage == item ? true : false }"
      class="items"
      v-for="(item, index) in routes"
      :key="index"
      @click="goToRoute(item)"
    >
      {{ item }}
    </div> -->
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  props: {
    routes: Array,
    currentPage: String,
  },
  setup(props, { emit }) {
    const goToRoute = (item) => {
      emit("change-route", item);
    };

    return {
      goToRoute,
    };
  },
};
</script>

<style lang="less" scoped>
.navbar {
  width: 200px;
  height: 100%;
  position: fixed;
  top: 0;
  left: -150px;
  background: #141414;
  color: white;
  display: flex;
  align-items: center;
  flex-direction: column;
  transition: 0.1s;
  &:hover {
    left: 0;
  }

  .setting {
    align-self: flex-end;
  }

  .nav-item {
    transition: 0.1s;
    display: flex;
    justify-content: space-between;
    width: 100%;
    p {
      transition: 0.1s;
      padding-left:25px;
      text-align: center;
      width: calc(100% - 30px);
    }
    i {
      transition: 0.1s;
      display: flex;
      justify-content: center;
      align-items: center;
      min-width: 50px;
      height: 50px;
    }
    &:hover {
      background: #141414 + #101010;
      color: #0088ff;
    }
  }
}

.selected {
  color: red;
}
</style>
