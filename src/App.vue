<template>
  <div id="app">
    <!-- <p>{{msg}}</p>
    <main v-if="show">메인</main>-->
    <todo-header></todo-header>
    <!-- TodoInput, TodoList 컴포넌트 등록  -->
    <!-- 1. 컴포넌트 폴더 밑에 vue 파일 생성
    2. vue 파일에서 `vue` 자동 완성 기능으로 기본 코드 생성
    3. 각 template 코드에 `<div>컴포넌트 이름</div>` 기입
    4. 컴포넌트를 모두 App.vue 파일에 등록 후 표시-->
    <todo-input></todo-input>
    <todo-list></todo-list>
  </div>
</template>

<script>
// import 컴포넌트 이름 from '컴포넌트 경로';
// 스니펫 : vim
import TodoHeader from "./components/TodoHeader.vue";
import TodoList from "./components/TodoList.vue";
import TodoInput from "@/components/TodoInput.vue";

export default {
  // 스니펫 : vda
  data() {
    return {
      msg: "hi",
      show: false
    };
  },
  components: {
    // '컴포넌트 이름' : 컴포넌트 내용
    "todo-header": TodoHeader,
    "todo-input": TodoInput,
    "todo-list": TodoList
  }
};
</script>

<style>
</style>
