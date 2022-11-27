<template>
  <section>
    <div class="wrapper">
      <form
        @submit.prevent="onSubmit"
        action=""
        method="post"
        >
          <p class="form-text">ENTER YOUR ACCESS TOKEN</p>
          <input v-model="token" type="text" placeholder="insert your token here" class="form-input"/>
          <p class="form-text is-right">PRESS ENTER</p>
      </form>
    </div>
  </section>
</template>

<script>
import axios from "axios";

export default {
  name: 'FormTokenComponent',
  data() {
    return {
      token: ""
    }
  },
  methods: {
    onSubmit() {
      axios.post('https://reqres.in/api/users?page=1', {
        token: this.token
      }).then((response) => {
        console.log(response.data)
      }).catch((error) => {
        console.log(error);
      });
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.form-text {
  font-weight: 300;
  color: #9ca3af;
}
.form-text.is-right {
  text-align: right;
  padding: .5em;
}
.form-input {
  display: block;
  width: 100%;
  outline: none;
  font-size: 3rem;
  line-height: 1;
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid #ff7834;
}
</style>
