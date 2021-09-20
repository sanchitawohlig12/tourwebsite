<template>
  <div class="review">
    <h1>Review</h1>
    <div class="wrapper">
      <p id="hi">
        If you miss this place while travelling to Bali, then trust me you have
        missed something worth visiting.
      </p>
    </div>
    <div>
      <v-rating
        v-model="rating"
        background-color="orange lighten-3"
        color="orange"
        small
      ></v-rating>
    </div>
    <span>Ashrini Borah,</span>
    <br />
    <span>Aug 24, 2021</span>
  </div>
</template>

<script>
export default {
  data: () => ({
    rating: 4,
  }),
}
</script>

<style>
#wrapper {
  background-color: #051e3e;
  height: 100vh;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}

#hi {
  animation: pulse 5s;
}

@keyframes pulse {
  0% {
    color: #051e3e;
  }
  10% {
    color: #051e3e;
  }
  30% {
    color: white;
  }
  50% {
    color: #051e3e;
  }
  60% {
    color: #051e3e;
  }
  80% {
    color: white;
  }
  100% {
    color: #051e3e;
  }
}

#hi:after {
  content: '';
  animation: spin 5s linear;
}

@keyframes spin {
  0% {
    content: 'Hi';
  }
  100% {
    content: 'How do you like it?';
  }
}
.review {
  text-align: center;
}
span {
  color: gray;
}
.review {
  margin-top: 5%;
}
</style>