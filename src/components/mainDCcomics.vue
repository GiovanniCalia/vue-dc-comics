<template>
<main>
    <div class="first-main">
      <div class="container">
        <h1>--> Content goes here --></h1>
      </div>
    </div>

    <div class="second-main">
      <div class="container">
        <ul class="ul-images">
          <li class="li-inline-block">
            <a href="#!">
              <img src="../../src/assets/img/buy-comics-digital-comics.png" alt="DC">
              <div>digital comics</div>
            </a>
          </li>
          <li class="li-inline-block">
            <a href="#!">
              <img src="../../src/assets/img/buy-comics-merchandise.png" alt="DC">
              <div>dc merchandise</div>
            </a>
          </li>
          <li class="li-inline-block">
            <a href="#!">
              <img src="../../src/assets/img/buy-comics-subscriptions.png" alt="DC">
              <div>subscription</div>
            </a>
          </li>
          <li class="li-inline-block">
            <a href="#!">
              <img id="img-shop" src="../../src/assets/img/buy-comics-shop-locator.png" alt="DC">
              <div>comic shop locator</div>
            </a>
          </li>
          <li class="li-inline-block">
            <a href="#!">
              <img src="../../src/assets/img/buy-dc-power-visa.svg" alt="DC">
              <div>dc power visa</div>
            </a>
          </li>

        </ul>
      </div>
    </div>

    <div class="container third-main">
      <div class="container float">
        <div class="little-container">
          <ul class="ul-second-main">
            <h2>dc comics</h2>
            <li class="second-li" v-for="element in DCcomicsLinks" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>

            <h2>shop</h2>
            <li class="second-li" v-for="element in shopLinks" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>
          </ul>
          <ul class="ul-second-main">
            <h2>dc</h2>
            <li class="second-li" v-for="element in DCLinks" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>
          </ul>
          <ul class="ul-second-main">
            <h2>sites</h2>
            <li class="second-li" v-for="element in sites" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>
          </ul>
        </div>
      </div>
      <img src="../../src/assets/img/dc-logo-bg.png" alt="big DC">
    </div>
</main>

</template>

<script>
export default {
  name: 'mainDCcomics',
  data () {
    return {
      DCcomicsLinks: [
        {
          href: '#',
          text: 'Characters'
        },
        {
          href: '#',
          text: 'Comics'
        },
        {
          href: '#',
          text: 'Movies'
        },
        {
          href: '#',
          text: 'TV'
        },
        {
          href: '#',
          text: 'Games'
        },
        {
          href: '#',
          text: 'Videos'
        },
        {
          href: '#',
          text: 'News'
        }
      ],
      shopLinks: [
        {
          href: '#',
          text: 'Shop DC'
        },
        {
          href: '#',
          text: 'Shop DC collectibles'
        }
      ],
      DCLinks: [
        {
          href: '#',
          text: 'Terms of use'
        },
        {
          href: '#',
          text: 'Privacy policy (New)'
        },
        {
          href: '#',
          text: 'Ad Choices'
        },
        {
          href: '#',
          text: 'Advertising'
        },
        {
          href: '#',
          text: 'Jobs'
        },
        {
          href: '#',
          text: 'Subscriptions'
        },
        {
          href: '#',
          text: 'Talent Workshops'
        },
        {
          href: '#',
          text: 'CPSC Certificates'
        },
        {
          href: '#',
          text: 'Ratings'
        },
        {
          href: '#',
          text: 'Shop Help'
        },
        {
          href: '#',
          text: 'Contact Us'
        }
      ],
      sites: [
        {
          href: '#!',
          text: 'DC'
        },
        {
          href: '#!',
          text: 'MAD Magazine'
        },
        {
          href: '#!',
          text: 'DC Kids'
        },
        {
          href: '#!',
          text: 'DC Universe'
        },
        {
          href: '#!',
          text: 'DC Power visa'
        }
      ]
    }
  }
}
</script>

<style scoped lang='scss'>
@import '@/assets/styles/otherstyles/variables.scss';

main{
  background-image: url(../../src/assets/img/footer-bg.jpg);
  background-size: cover;
}

.little-container{
  width: 600px;
}

.ul-second-main{
  float: left;
  margin: 2rem;
}

.float:after{
    content: "";
    display: table;
    clear: both;
}

.first-main{
  background-color: black;
}

.second-main{
  background-color: $blue_color;
}

#img-shop{
  width: 10%;
  margin-bottom: 1rem;
  margin-left: -1rem;
}

.third-main{
  display: flex;
  max-height: 400px;
  overflow: hidden;

  img{
    width: 500px;
    height: 500px;
    position: relative;
    bottom: 2rem;
  }
}

.ul-images {
  text-align: center;
}

h1{
  color: white;
  line-height: 8rem;
}

.li-inline-block{
  display: inline-block;
  margin: 3rem 0;
  width: 220px;

  a{
    text-transform: uppercase;
    text-decoration: none;
    color: white;
    display: flex;
    align-items: center;

    img{
      width: 12%;
      margin-right: 0.4rem;
    }

  }
}

h2 {
  text-transform: uppercase;
  margin-bottom: 1rem;
  color: white;
  margin-top: 1rem;
}

.second-li{
  list-style-type: none;
  margin-bottom: 5px;

  a{
  text-decoration: none;
  color: grey;
}
}

</style>
