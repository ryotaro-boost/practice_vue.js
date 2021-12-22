<template>
  <div class="event-page">
    <h2> 学習3：イベント</h2>

    <!-- 従来のJavaScript -->
    <h3><span class="badge badge-secondary">JavaScript</span></h3>
    <span id="countText">クリックされた回数は0回です</span>
    <button id="button" class="btn btn-sm btn-info">Click Me</button>
    <br>
    <br>
  </div>
</template>

<script>
// 従来のJavaScript
let count = 0;
window.onload = function() {
  const button = document.getElementById('button');
  button.onclick = function() {
    count++;
    const countText = document.getElementById('countText');
    countText.innerHTML = 'クリックされた回数は' +  count + '回です ';
  }
}

export default {
  
}
</script>

<style scoped>
.event-page {
  padding: 20px;
}
</style>