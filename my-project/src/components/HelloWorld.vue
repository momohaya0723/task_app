<template>
 <div>
  <p>{{title}}</p>
  <p>{{ total }}</p>
  <!-- incrementと言うイベントを定義。子コンポーネントから$emitされたら、incrementTotal実行される -->
  <hello-child v-on:increment="incrementTotal"/>
 </div>
</template>
 
<script>
import HelloChild from './HelloChild'
export default {
  data: function () {
    return {
      title: 'はろー！わーるど！',
      total: 0
    }
  },
  methods: {
    incrementTotal: function () {
      this.total += 1
    }
  },
  components: {
    HelloChild
  }
}
</script>