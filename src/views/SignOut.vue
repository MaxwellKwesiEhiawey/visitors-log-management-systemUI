<template>
  <div class="signout">
    <h3>SignOut</h3>
    <form action="" @submit="handleSubmit" >
      <label Email></label>
      <input placeholder="email" type="text" required v-model="email" />
      <p>{{ email }}</p>
      <div class="submit">
        <button class="btn">
          SignOut
        </button>
        <router-link class="QR" to="/qrcode"
        ><button id="btn-q" class="btn">
            Use QR-code Instead
          </button></router-link
      >
      </div>
    </form>
    
  </div>
  
</template>

<script>
export default {
  data() {
    return {
      email: ""
    };
  },
  methods: {
    handleSubmit() {
      try {
        this.$router.push("");
      } catch (e) {
        console.log(e);
      }
    }
  }
};
</script>
<style scoped>
.btn {
  background: rgb(245, 213, 176);
  color: #a7082f;
  width: 100px;
  border-radius: 20px;
  height: 25px;
  border: 2.5px solid #690009;
  cursor: pointer;
  outline: none;
}
.QR {
  padding-left: 40px;
  padding-top: 100px;
  border-top: 40px;
}
#btn-q{
  width: 110px;
  height: 40px;
}
.signout{
  height: 400px;
}
h3 {
  color: #a7082f;
}
input {
  background: rgb(248, 236, 224);
  border-radius: 5px;
  border: 2.5px solid #690009;
  width: 200px;
  outline: none;
}
 .submit{
  padding-bottom: 10px;
  margin: 0px;
  display: flex;
  padding: 0 2px;
  margin: 30px;
  padding-left: 600px;
  padding-right: 200px;
  justify-content: space-between;
}
</style>