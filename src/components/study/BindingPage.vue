<template>
  <div class="binding-page">
    <h2>学習1：双方向バインディング</h2>

    <!-- 従来のJavaScript -->
    <h3><span>JavaScript</span></h3>
    <input class="form-control" id="name">
    <span id="text">入力された名前はです</span>
    <br>
    <br>
  </div>
</template>

<script>
// 従来のJavaScript
window.onload = function() {
  const nameInput = document.getElementById('name');
  nameInput.oninput = function() {
    const name = nameInput.value;
    const text = document.getElementById('text');
    text.innerHTML = '入力された名前は' + name + 'です';
  }
}

export default {
  
}
</script>

<style scoped>
.binding-page {
  padding: 20px;
}
</style>