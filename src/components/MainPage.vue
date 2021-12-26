<template>
    <div class="main-page">
        <div class="left-menu">
            <!-- ノート追加ボタン -->
            <button class="transparent" @click="onClickButtonAdd">
                <i class="fas fa-plus-square"></i>ノートを追加
            </button>
        </div>
        <div class="right-view">
            右メニュー
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            notelist : [],
        }
    },
    methods: {
        onClickButtonAdd : function() {
            this.notelist.push({
                id : new Date().getTime().toString(16),
                name : '新規ノート',
            })
        },
    },
}
</script>

<style scoped lang="scss">
.main-page {
    display: flex;
    height: calc(100vh - 60px);
    .left-menu {
        width: 350px;
        background-color: #f7f6f3;
    }
    .right-view {
        flex-grow: 1;
        padding: 10px;
    }
}
</style>