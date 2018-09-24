<template>
  <div class="animated fadeIn">
    <b-row>
      <b-col md="auto">
        <b-card class="m-card" v-on:click="goNaver">
          <b-card-body class="pb-0">
            <img class="m-icon no-drag" src="img/icons/naver.png" alt="admin@bootstrapmaster.com"/>
            <p class="m-icon-text no-drag">NAVER</p>
          </b-card-body>
        </b-card>
      </b-col>
      <b-col md="auto">
        <b-card class="m-card" v-on:click="goGoogle">
          <b-card-body class="pb-0">
            <img class="m-icon no-drag" src="img/icons/google.png" alt="admin@bootstrapmaster.com"/>
            <p class="m-icon-text no-drag">Google</p>
          </b-card-body>
        </b-card>
      </b-col>
    </b-row>
    <p>Hello World</p>
    <b-col sm="6" lg="3">
      <b-button>B Button</b-button>
    </b-col>
    <b-col sm="6" lg="3">
      <button>Button Example</button>
    </b-col>
  </div>
</template>

<script>

export default {
  name: 'firstpage',
  methods: {
    goNaver() {
      window.open('http://www.naver.com');
    },
    goGoogle() {
      window.open('http://www.google.com');
    }
  }
}
</script>

<style>
.m-card {
  background-color: transparent;
  width: 200px;
  height: 200px;
}

.m-card:hover {
  background: rgba(0, 0, 0, 0.1);
  z-index: 2;
}

.m-card:focus {
  box-shadow: 0 0 10px 1px rgba(0, 0, 144, 0.3);
}

.m-card:active:hover {
  background: rgba(0, 0, 0, 0.2);
  z-index: 2;
}

.m-icon {
  width: 120px;
  height: 120px;
  text-align: center;
}

.m-icon-text {
  text-align: center;
  margin-top: 5px;
  font-size: 15px;
  font-weight: bold;
  font-family: Arial, Helvetica, sans-serif;
}

.m-button {
  background-color: green
  
}

.m-button:hover {
  background-color: blue
}

.m-button:focus {
  background-color: aliceblue
}

.no-drag {
  -ms-user-select: none; 
  -moz-user-select: -moz-none; 
  -webkit-user-select: none; 
  -khtml-user-select: none; 
  user-select: none;
}

</style>


