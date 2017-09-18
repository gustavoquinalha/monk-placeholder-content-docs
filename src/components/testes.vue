<template>
<div class="hello">

  <div class="">
    <div class="" v-show="isLoading" v-cloak>
      <div class="container wrap">
        <div class="col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box" v-for="x in 3">
          <placeholderContent type="card" :photo="true" :title="true" :description="false" :number="1" :button="false" :imageSize="400"></placeholderContent>
        </div>
      </div>
    </div>

    <div class="" v-show="!isLoading" v-cloak>
      <div class="container wrap justify-content-center align-items-center">
        <div class="col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box" v-for="x in teste">
          <div class="container justify-content-start align-items-center">
            <div class="picture">
              <img :src="x.profile" width="180%" alt="">
            </div>
            <div class="container column justify-content-start align-items-center">
              <div class="example-text">
                <h1>{{x.name}}</h1>
                <p>{{x.time}}</p>
              </div>
            </div>
          </div>
          <div class="image-ex" v-bind:style="{ 'background-image': 'url(' + x.img + ')' }">
            <!-- <img :src="x.img" width="100%" alt=""> -->
          </div>
        </div>
      </div>
    </div>

    <div class="container align-items-center justify-content-center">
      <div class="">
        <span class="btn start" :to="{ name: 'Docs' }" @click="tryAgain">Try again</span>
      </div>
    </div>
  </div>

<div class="relative">
  <div class="container align-items-start"><pre><code class="html" id="card2">&lt;template&gt;
  &lt;div class=&quot;hello&quot;&gt;
    &lt;div class=&quot;&quot; v-show=&quot;isLoading&quot; v-cloak&gt;
      &lt;div class=&quot;container wrap&quot;&gt;
        &lt;div class=&quot;col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box&quot; v-for=&quot;x in 3&quot;&gt;
          &lt;placeholderContent type=&quot;card&quot; :photo=&quot;true&quot; :title=&quot;true&quot; :description=&quot;false&quot; :number=&quot;1&quot; :button=&quot;false&quot; :imageSize=&quot;400&quot;&gt;&lt;/placeholderContent&gt;
        &lt;/div&gt;
      &lt;/div&gt;
    &lt;/div&gt;

    &lt;div class=&quot;&quot; v-show=&quot;!isLoading&quot; v-cloak&gt;
      &lt;div class=&quot;container wrap justify-content-center align-items-center&quot;&gt;
        &lt;div class=&quot;col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box&quot; v-for=&quot;x in teste&quot;&gt;
          &lt;div class=&quot;container justify-content-start align-items-center&quot;&gt;
            &lt;div class=&quot;picture&quot;&gt;
              &lt;img :src=&quot;x.profile&quot; width=&quot;180%&quot; alt=&quot;&quot;&gt;
            &lt;/div&gt;
            &lt;div class=&quot;container column justify-content-start align-items-center&quot;&gt;
              &lt;div class=&quot;example-text&quot;&gt;
                &lt;h1&gt;x.nome&lt;/h1&gt;
                &lt;p&gt;x.time&lt;/p&gt;
              &lt;/div&gt;
            &lt;/div&gt;
          &lt;/div&gt;
          &lt;div class=&quot;image-ex&quot; v-bind:style=&quot;{ 'background-image': 'url(' + x.img + ')' }&quot;&gt;
          &lt;/div&gt;
        &lt;/div&gt;
      &lt;/div&gt;
    &lt;/div&gt;
  &lt;/div&gt;
&lt;/template&gt;

&lt;script&gt;
import placeholderContent from '../../node_modules/monk-placeholder-content/src/components/placeholder-content.vue'

export default {
  name: 'hello',
  data () {
    return {
      isLoading: true,
      teste: [{
        name: 'Will smith',
        time: 'Agora pouco',
        profile: 'https://fashionfoodandflirts.files.wordpress.com/2013/04/fresh-prince-will-smith.jpg',
        img: 'https://s2.glbimg.com/aAjW1O_ErEF6fbcfh9nkZh9mBxw=/227x0:779x600/570x620/smart/http://s2.glbimg.com/_wZd-4_-aTqEE3ZaZITdonmzvpo=/0x0:1060x600/1060x600/s.glbimg.com/po/tt2/f/original/2017/09/13/iphone_8_plus_tela_aplicativos_apps_mao.jpg'
      },
      {
        name: 'Will smith',
        time: 'Agora pouco',
        profile: 'https://www.rickey.org/wp-content/uploads/2015/08/fresh_prince_header.jpg',
        img: 'https://jovemnerd.com.br/wp-content/uploads/2016/08/fresh-prince-vitrine-760x428.jpg'
      },
      {
        name: 'Will smith',
        time: 'Agora pouco',
        profile: 'https://fashionfoodandflirts.files.wordpress.com/2013/04/fresh-prince-will-smith.jpg',
        img: 'https://art-s.nflximg.net/ef14e/f435deeec5987212d8fe76b75ab7015bb73ef14e.jpg'
      }]
    }
  },
  components: {
    placeholderContent
  },
  methods: {
    Loading: function () {
      setTimeout(this.fakeFetch, 2000)
    },
    tryAgain: function () {
      this.isLoading = !this.isLoading
      setTimeout(this.fakeFetch, 2000)
    }
  },
  mounted () {
    this.Loading()
  }
}
&lt;/script&gt;

&lt;style scoped&gt;
&lt;/style&gt;


  </code></pre>
    <div class="copy-btn">
      <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#card2" style="height: 20px">copy</a>
    </div>
  </div>
</div>
</div>
</template>

<script>
import placeholderContent from '../../node_modules/monk-placeholder-content/src/components/placeholder-content.vue'

export default {
  name: 'hello',
  data () {
    return {
      isLoading: true,
      teste: [{
        name: 'Will smith',
        time: 'Agora pouco',
        profile: 'https://fashionfoodandflirts.files.wordpress.com/2013/04/fresh-prince-will-smith.jpg',
        img: 'https://s2.glbimg.com/aAjW1O_ErEF6fbcfh9nkZh9mBxw=/227x0:779x600/570x620/smart/http://s2.glbimg.com/_wZd-4_-aTqEE3ZaZITdonmzvpo=/0x0:1060x600/1060x600/s.glbimg.com/po/tt2/f/original/2017/09/13/iphone_8_plus_tela_aplicativos_apps_mao.jpg'
      },
      {
        name: 'Will smith',
        time: 'Agora pouco',
        profile: 'https://www.rickey.org/wp-content/uploads/2015/08/fresh_prince_header.jpg',
        img: 'https://jovemnerd.com.br/wp-content/uploads/2016/08/fresh-prince-vitrine-760x428.jpg'
      },
      {
        name: 'Will smith',
        time: 'Agora pouco',
        profile: 'https://fashionfoodandflirts.files.wordpress.com/2013/04/fresh-prince-will-smith.jpg',
        img: 'https://art-s.nflximg.net/ef14e/f435deeec5987212d8fe76b75ab7015bb73ef14e.jpg'
      }]
    }
  },
  components: {
    placeholderContent
  },
  methods: {
    fakeFetch: function () {
      this.isLoading = !this.isLoading
    },
    Loading: function () {
      setTimeout(this.fakeFetch, 2000)
    },
    tryAgain: function () {
      this.isLoading = !this.isLoading
      setTimeout(this.fakeFetch, 2000)
    }
  },
  mounted () {
    this.Loading()
  }
}
</script>


<style scoped>
.btn-copy {
  transform: translateY(20px);
}
code, pre {
  text-align: left!important;
}
.btn {
  cursor: pointer
}

.card-ex {
  background: blue;
  width: 100%;
}

.image-ex {
  height: 400px;
  margin-top: 12px;
  overflow: hidden;
  background-position: center;
  background-size: cover;
  border-radius: 3px
}

.example-text {
  text-align: left;
  /*background: red*/
}

.example-text h1 {
  font-size: 18px
}

.example-text p {
  font-size: 14px
}

.picture {
  height: 60px;
  width: 60px;
  border-radius: 50%;
  margin-right: 20px;
  background: red;
  overflow: hidden;
}

.photo {
  height: 400px;
  border-radius: 40px!important;
  overflow: hidden;
}

.box {
  padding: 20px;
  box-sizing: border-box;
}

.hello {
  width: 1200px;
  max-width: 90%;
  margin: 0 auto;
}

.example {
  padding-top: 100px;
  padding-bottom: 100px;
  text-align: left
}

.example label {
  font-weight: 600;
  padding-bottom: 20px
}
</style>
