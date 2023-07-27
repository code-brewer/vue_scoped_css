<template>
  <div class="home">
    <span>首頁的文字</span>
    <Message />
  </div>
</template>

<script>
import Message from "@/components/Message";

export default {
  components: {
    Message,
  },
};
</script>


<style lang="scss" scoped>
span {
  color: red;
}

.home:deep .message {
  color: red;
}

// 以下寫法無法被編釋
/* .home >>> .message {
  color: red;
} */
</style>
