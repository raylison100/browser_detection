<template>
  <div class="hello">
    <h1> Detection Browser </h1>
    <!-- <ul>
      <li><b>Internet Chrome: </b> {{$browserDetect.isChrome}}</li>
      <li><b>Internet Firefox: </b> {{$browserDetect.isFirefox}}</li>
      <li><b>Internet Opera: </b> {{$browserDetect.isOpera}}</li>
      <li><b>Internet Safari: </b> {{$browserDetect.isSafari}}</li>
      <li><b>Internet Edge: </b> {{$browserDetect.isEdge}}</li>
      <li><b>Internet ChromeIOS: </b> {{$browserDetect.isChromeIOS}}</li>
      <li><b>Internet IOS: </b> {{$browserDetect.isIOS}}</li>
      <li><b>Internet Explorer: </b> {{$browserDetect.isIE}}</li>
    </ul> -->
    <div class="center">
      <div class="example" :class="$browserDetect.meta.name"></div>
    </div>    
  </div>
</template>

<script>
  export default {
    name: 'Detections',
  }
</script>

<style scoped>
  .center{
      align-items: center;
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: center;
  }

  .example{
      width: 100px;
      width: 100px;
      height: 100px;
      border: 1px solid black;
  }

  .IE {
    background-color: rgb(73, 188, 255)
  }
  .Chrome {
    background-color: rgb(10, 94, 55)
  }
  .Firefox {
    background-color: rgb(219, 129, 26)
  }
  .Opera {
    background-color: rgb(255, 0, 0)
  }
  .Safari {
    background-color: rgb(38, 13, 146)
  }
  .Edge {
    background-color: rgb(147, 155, 177)
  }
  .ChromeIOS {
    background-color: rgb(37, 38, 39)
  }
  .IOS {
    background-color: rgb(176, 111, 206)
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: block;
    margin: 0 10px;
  }
</style>
