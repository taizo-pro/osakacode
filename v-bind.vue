<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>

  <style>
    .error {
      color: red;
    }
    .success {
      color: blue;
    }
  </style>
</head>
<body>
  <div id="app">
    <!-- マスタッシュはHTMLの中でしか使えない -->
    <p v-bind:class="error_class">エラーです</p>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/vue@2.6.14/dist/vue.js"></script>

  <script>
    var app = new Vue({
      el: '#app', // element
      data: {
        error_class: "success"
      } // objectの形にして、この中にさらにオブジェクトを投入する
    })
  </script>
</body>
</html>