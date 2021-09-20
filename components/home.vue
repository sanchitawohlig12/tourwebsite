<template>
  <div>
    <div>
      <h1>Nusa Penida Tour Guide</h1>
      <p>
        Totalling some 200 square kilometres, Nusa Penida is much larger than
        the better known Nusa Lembongan. However, tourist infrastructure is very
        limited here but growing fast.
      </p>

      <p></p>
      <p>
        Due to a lack of natural fresh water, little is grown or produced on
        Nusa Penida, and even some basic foodstuffs come in by boat. Visitors
        should therefore expect higher prices than in Bali, and not bank on any
        tourism-related luxury items being available for purchase here.
      </p>
    </div>
    <div class="out">
      <div class="in">
        <v-carousel cycle>
          <v-carousel-item
            v-for="(item, i) in items"
            :key="i"
            :src="item.src"
            reverse-transition="fade-transition"
            transition="fade-transition"
          >
            <h5>{{ item.title }}</h5>
          </v-carousel-item>
        </v-carousel>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          src: 'https://firebasestorage.googleapis.com/v0/b/nuxt-web-template.appspot.com/o/slides%2Fcrystal-bay-beach-2.jpg?alt=media&token=be8ffb8f-17e9-4b85-bf4a-9dff7f38348a',
          title: 'kelingking beach',
        },
        {
          src: 'https://firebasestorage.googleapis.com/v0/b/nuxt-web-template.appspot.com/o/slides%2Fbroken-beach.jpg?alt=media&token=d5c744e6-9fd4-4df0-8552-03659675f6d7',
          title: 'kelingking beach',
        },
        {
          src: 'https://firebasestorage.googleapis.com/v0/b/nuxt-web-template.appspot.com/o/slides%2Fklingking-beach.jpg?alt=media&token=0608592e-0bca-43ce-b535-857065b67ef5',
          title: 'kelingking beach',
        },
        {
          src: 'https://firebasestorage.googleapis.com/v0/b/nuxt-web-template.appspot.com/o/slides%2Fangel-billabong.jpg?alt=media&token=9d4b2f99-3667-464e-9d6a-5c4b6850bf84',
          title: 'kelingking beach',
        },
      ],
      overlay: false,
      absolute: false,
    }
  },
}
</script>
<style scoped>
h1 {
  color: gray;
}
p {
  padding-top: -5%;
  color: gray;
  font-size: 15px;
  text-align: left;
}
.in {
  border: white 15px solid;
}
.out {
  border: rgb(231, 218, 220) 35px solid;
}
h5 {
  margin-top: 50%;
  margin-left: 5%;
  color: rgb(231, 37, 69);
}
</style>