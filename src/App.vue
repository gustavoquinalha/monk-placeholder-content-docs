<template>
  <div id="app">
    <headerMenu></headerMenu>
      <transition name="fade">
        <router-view></router-view>
      </transition>

    <rodape></rodape>
  </div>
</template>

<script>
import headerMenu from './components/menu'
import rodape from './components/rodape'

export default {
  name: 'app',
  components: {
    headerMenu,
    rodape
  }
}
</script>

<style>
@import '../node_modules/the-grid-flexbox/css/the-grid.min.css';
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.hljs {
  padding: 20px;
  box-sizing: border-box;
  background: #2a2d4d
}
.hljs-attr {
  color: rgb(80, 250, 123)
}
.hljs-keyword,
.hljs-name {
  color: #ff79c6
}
.hljs-tag {
  color: #fff
}
.hljs-string {
  color: #fcff80
}
.fade-enter-active {
   transition: all .3s cubic-bezier(.37, .61, .58, .86);
 }
 .fade-leave-active {
   transition: all .3s cubic-bezier(.37, .61, .58, .86);
 }
 .fade-enter,
 .fade-leave-to {
   transform: translateY(-100vh);
 }
pre {
  width: 100%;
  margin: 0;
}
pre, code {
  border-radius: 4px;
  overflow: hidden;
  padding-top: 20px;
  padding-bottom: 20px;
}
.copy-btn {
  /*background: red;*/
  position: absolute;
  right: 0
}
a {
  text-decoration: none;
  color: #2c3e50
}
* {
  margin: 0;
  padding: 0
}
.btn {
  background: #ccc;
  height: 60px;
  line-height: 60px;
  padding: 10px 25px 10px 25px ;
  margin: 10px;
  border: 1px solid #4fc08d;
  color: #4fc08d;
  text-decoration: none;
  background: transparent;
  font-size: 14px;
  font-weight: 700;
  border-radius: 20px;
  transition: all 0.15s ease;
  cursor: pointer;
}
.relative {
  position: relative;
}
.btn:hover {
  background: #449872;
  color: #fff;
  border-color: #449872;
}
.btn.start {
  background: #4fc08d;
  color: #fff;
}
.btn.start:hover {
  background: #449872;
  color: #fff;
}
</style>
