<template>
<div class="hello">
  <div class="intro-block">
    <h1>Examples</h1>
  </div>

  <div class="example example1">
    <label for="">Simple content</label>
    <placeholderContent type="simple" :title="true" :number="3" :button="true"></placeholderContent>
    <div class="container align-items-center">
      <div v-highlight style="width: 100%"><pre><code class="html" id="simple">&lt;placeholderContent type=&quot;simple&quot; :title=&quot;true&quot; :number=&quot;3&quot; :button=&quot;true&quot;&gt;&lt;/placeholderContent&gt;</code></pre>
      </div>
      <div class="copy-btn">
        <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#simple" style="height: 20px">copy</a>
      </div>
    </div>
  </div>

  <div class="example example2">
    <label for="">Table content</label>
    <placeholderContent type="table" :title="true" :button-title="true" :number="3" :button="true"></placeholderContent>
    <div class="container align-items-center">
      <div v-highlight style="width: 100%">
        <pre><code class="html" id="table">&lt;placeholderContent type=&quot;table&quot; :title=&quot;true&quot; :button-title=&quot;true&quot; :number=&quot;3&quot; :button=&quot;true&quot;&gt;&lt;/placeholderContent&gt;</code></pre>
      </div>
      <div class="copy-btn">
        <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#table" style="height: 20px">copy</a>
      </div>
    </div>

  </div>


  <div class="example example3">
    <label for="">Card content</label>
    <div class="container wrap">
      <div class="col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box" v-for="x in 3">
        <placeholderContent type="card" :title="false" :description="true" :number="3" :photo="false" :button="false"></placeholderContent>
      </div>
    </div>

    <div class="container align-items-center">
      <div v-highlight style="width: 100%">
        <pre><code class="html">&lt;placeholderContent type=&quot;card&quot; :title=&quot;false&quot; :description=&quot;true&quot; :number=&quot;3&quot; :photo=&quot;false&quot; :button=&quot;false&quot;&gt;&lt;/placeholderContent&gt;</code></pre>
      </div>
      <div class="copy-btn">
        <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#card1" style="height: 20px">copy</a>
      </div>
    </div>
  </div>

  <div class="example example4">
    <label for="">Card content</label>
    <div class="container wrap">
      <div class="col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box" v-for="x in 3">
        <placeholderContent type="card" :title="true" :description="true" :number="2" :photo="false" :button="false"></placeholderContent>
      </div>
    </div>
    <div class="container align-items-center">
      <div v-highlight style="width: 100%">
        <pre><code class="html">&lt;placeholderContent type=&quot;card&quot; :title=&quot;false&quot; :description=&quot;true&quot; :number=&quot;3&quot; :photo=&quot;false&quot; :button=&quot;false&quot;&gt;&lt;/placeholderContent&gt;</code></pre>
      </div>

      <div class="copy-btn">
        <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#card1" style="height: 20px">copy</a>
      </div>
    </div>
  </div>

  <div class="example example5">
    <label for="">Card content 2</label>
    <div class="container wrap">
      <div class="col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box" v-for="x in 3">
        <placeholderContent type="card" :photo="true" :title="true" :description="false" :number="1" :button="false"></placeholderContent>
      </div>
    </div>
    <div class="container align-items-center">
      <div v-highlight style="width: 100%">
        <pre><code class="html">&lt;placeholderContent type=&quot;card&quot; :photo=&quot;true&quot; :title=&quot;true&quot; :description=&quot;false&quot; :number=&quot;1&quot; :button=&quot;false&quot;&gt;&lt;/placeholderContent&gt;</code></pre>
      </div>

      <div class="copy-btn">
        <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#card2" style="height: 20px">copy</a>
      </div>
    </div>
  </div>

  <div class="example example6">
    <label for="">Card content 3</label>
    <div class="container wrap">
      <div class="col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box" v-for="x in 3">
        <placeholderContent type="card" :photo="false" :title="true" :description="false" :number="1" :button="false"></placeholderContent>
      </div>
    </div>
    <div class="container align-items-center">
      <div v-highlight style="width: 100%">
        <pre><code class="html">&lt;placeholderContent type=&quot;card&quot; :photo=&quot;false&quot; :title=&quot;true&quot; :description=&quot;false&quot; :number=&quot;1&quot; :button=&quot;false&quot;&gt;&lt;/placeholderContent&gt;</code></pre>
    </div>
      <div class="copy-btn">
        <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#card3" style="height: 20px">copy</a>
      </div>
    </div>
  </div>


  <div class="example example7">
    <label for="">Card content 4</label>
    <div class="container wrap">
      <div class="col-12 col-xl-4 col-lg-4 col-md-6 col-sm-12 box" v-for="x in 3">
        <placeholderContent type="card" :photo="true" :title="false" :description="true" :number="2" :button="false" :head="false"></placeholderContent>
      </div>
    </div>
    <div class="container align-items-center">
      <div v-highlight style="width: 100%">
        <pre><code class="html">&lt;placeholderContent type=&quot;card&quot; :photo=&quot;true&quot; :title=&quot;false&quot; :description=&quot;true&quot; :number=&quot;2&quot; :button=&quot;false&quot; :head=&quot;false&quot;&gt;&lt;/placeholderContent&gt;</code></pre>
    </div>

      <div class="copy-btn">
        <a class="btn btn-copy container align-items-center jusitfy-content-center" data-clipboard-target="#card4" style="height: 20px">copy</a>
      </div>
    </div>
  </div>

  <div class="example example7">
    <label for="">Fake fetch</label>
    <fakeFetch></fakeFetch>
  </div>



</div>
</template>

<script>
import placeholderContent from '../../node_modules/monk-placeholder-content/src/components/placeholder-content.vue'
import fakeFetch from './testes.vue'

export default {
  name: 'hello',
  data () {
    return {}
  },
  components: {
    placeholderContent,
    fakeFetch
  }
}
</script>


<style scoped>
code,
pre {
  width: 100%
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
  text-align: left;
  position: relative;
}

.example label {
  font-weight: 600;
  padding-bottom: 20px
}
</style>
