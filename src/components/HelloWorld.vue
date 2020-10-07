<template>
<div>
  <div class="pill"/>
  <div class="cube">
<div class="square"/>
  </div>
  <div class="hello">
    test
  </div>
  <div class="hello1">
    test
  </div>
  <div class="hello2">
    test
  </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">

@color1 : #a89b35;
@color2 : #3786ff;
@color3 : #0946ee;
@color4 : #d45f10;
@color5 : #46606d;
@color6 : #aca98a;
@color7 : #d0956a;
@color8 : #ce9812;
@color9 : #8bdbfe;
@black: #000;
@size: 20em;
@marginSize: .2em;
@pillHeight: 15em;
page {
  background-color: @black;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.hello {
  background-color: @color1;
  height: 10em;
  border-top-left-radius: 2em;
  border-bottom-left-radius: 2em;
  color: @black;
  display: inline-block;
  width: 6em;
  margin: @marginSize;
  text-align: right;
  vertical-align: bottom;
}
.hello1 {
  background-color: @color1;
  height: 10em;
  color: @black;
  display: inline-block;
  width: 6em;
  margin: @marginSize;
}
.hello2 {
  background-color: @color1;
  height: 10em;
  color: @black;
  display: inline-block;
  width: 6em;
  margin: @marginSize;
}
.cube{
  margin: 1em auto;
  width: @size;
  height: @size;
  background-color: pink;
}
.square{
  width: @size/3;
  height: @size/3;
  box-sizing: border-box;
  border: @marginSize solid black;
  background-color: red;
}
.pill{
  width: 15em;
  height: @pillHeight;
  border-top-left-radius: @pillHeight/2;
  background-color: @color9;
}
</style>
