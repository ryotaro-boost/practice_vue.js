<template>
  <div class="directive-page">
    <h2> 学習2：ディレクティブ</h2>

    <!-- 従来のJavaScript -->
    <h3><span class="badge badge-secondary">JavaScript</span></h3>
    <input id="check" type="checkbox" checked="checked">
    <span id="text">チェック時のみ表示</span>
    <br>
    <br>
  </div>
</template>

<script>
// 従来のJavaScript
window.onload = function() {
  const checkbox = document.getElementById('check');
  checkbox.onchange = function(event) {
    const checked = event.target.checked;
    const text = document.getElementById('text');
    if (checked) {
      text.style.visibility = 'visible';
    } else {
      text.style.visibility = 'hidden';
    }
  };
}

export default {
  
}
</script>

<style scoped>
.directive-page {
  padding: 20px;
}
</style>