<template>
  <header>
    <div class="container">
      <div class="icon">
        <img src="../assets/images/dc-logo-bg.png" alt="">
      </div>

      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :key="link.url">{{ link.testo }}</a>
        </li>
       
      </ul>
    </div>
    
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
  // props: {
  //   msg: String
  // }
  data(){
    return {
      links: [
        {
          testo: "characters",
          url: "#",
          active: false,
        },
        {
          testo: "comics",
          url: "#",
          active: false,
        },
        {
          testo: "movies",
          url: "#",
          active: false,
        },
        {
          testo: "tv",
          url: "#",
          active: false,
        },
        {
          testo: "games",
          url: "#",
          active: false,
        },
        {
          testo: "collectible",
          url: "#",
          active: false,
        },
        {
          testo: "videos",
          url: "#",
          active: false,
        },
        {
          testo: "fans",
          url: "#",
          active: false,
        },
        {
          testo: "news",
          url: "#",
          active: false,
        },
        {
          testo: "shop",
          url: "#",
          active: false,
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import '../style/variables.scss';

.container {
  width: 70%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 0;
  ul {
    display: flex;
    justify-content: space-around;
    li {
      list-style-type: none;
      margin: 0 15px;
      font-size: 12px;
      text-transform: uppercase;
      a {
        text-decoration: none;
        color: #000;

        &.active,
        &:hover {
          border-bottom: 5px solid $bgAzzurro;
        }
      }
    }
  }
}

.icon {
  img {
    width: 100px;
    transform: rotate(25deg);
  }
}


</style>
