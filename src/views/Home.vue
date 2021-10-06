<template>
  <div class="home">
    <div class="profile">
      <h2>Adharsh C S</h2>
      <div class="data">
        <div class="clg">
          <h3>College Details</h3>
          <div class="sep"></div>
          <div class="field">
            <span>Register Number</span>
            <p>111420243013</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Enrollment Year</span>
            <p>2020-2024</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Department Code</span>
            <p>A120008</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Boarding Point</span>
            <p>Thirumullaivoyal</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Bus Number</span>
            <p>Thirumullaivoyal</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Food</span>
            <p>Lunch Only</p>
          </div>
          <!-- <div class="sep"></div> -->
        </div>
        <div class="personal">
          <h3>College Details</h3>
          <div class="sep"></div>
          <div class="field">
            <span>Register Number</span>
            <p>111420243013</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Enrollment Year</span>
            <p>2020-2024</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Department Code</span>
            <p>A120008</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Boarding Point</span>
            <p>Thirumullaivoyal</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Bus Number</span>
            <p>Thirumullaivoyal</p>
          </div>
          <div class="sep"></div>
          <div class="field">
            <span>Food</span>
            <p>Lunch Only</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
};
</script>

<style scoped lang="less">
.sep {
  background: #363636;
  width: 90%;
  height: 2px;
  margin: 2px 0;
}

.home {
  width: 100%;
  height: 100%;
  background: rgb(14, 0, 255);
  background: linear-gradient(
    45deg,
    rgba(14, 0, 255, 1) 0%,
    rgba(0, 212, 255, 1) 100%
  );

  display: flex;
  justify-content: center;
  align-items: center;
  // flex-direction: column;

  .profile {
    width: 90%;
    height: 90%;

    background: #ffffff;

    border-radius: 8px;
    margin: 0 10px;
    display: flex;

    align-items: center;
    // justify-content: space-around;
    flex-direction: column;
    // color: white;

    h2 {
      width: calc(100% - 40px);
      height: 100px;
      background: #1f0029;
      border-radius: 8px 8px 0 0;
      display: flex;
      padding: 0 20px;
      align-items: center;
      font-size: 44px;
      color: white;
    }

    .data {
      width: 100%;
      height: calc(100% - 100px);
      display: flex;
      justify-content: space-around;
      align-items: center;
      .clg {
        width: 40%;
        height: auto;
        display: flex;
        flex-direction: column;
        align-items: center;

        h3 {
          width: 80%;
          text-align: left;
          font-size: 30px;
          margin: 5px 0;
        }

        .field {
          width: 80%;
          background: #ffffff;
          height: 70px;
          border-radius: 6px;
          display: flex;
          justify-content: center;
          align-items: center;
          flex-direction: column;
          h3 {
            width: 80%;
            text-align: left;
            font-size: 30px;
            margin: 5px 0;
          }
          span {
            width: 100%;
            font-size: 14px;
            text-align: left;
          }
          p {
            width: 100%;
            font-size: 24px;
            text-align: left;
          }
        }
      }
      .personal {
        
      }
    }
  }
}
</style>
