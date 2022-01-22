<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <div id="app">
    <p>{{now}}</p>
    <button v-on:click="time">現在時刻を表示</button>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/vue@2.6.14/dist/vue.js"></script>

  <script>
    var app = new Vue({
      el: '#app', // element
      data: {
        now: new Date()
      }, // objectの形にして、この中にさらにオブジェクトを投入する
      methods: {
        time: function(e) {
          this.now = new Date()
        }
      },
    })
  </script>
</body>
</html>