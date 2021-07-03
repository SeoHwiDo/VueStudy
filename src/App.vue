<template>
  <div id="app">
    <h1>vfor 테스트</h1>
    <table>
      <thead>
        <tr>
          <th>도서번호</th><th>도서제목</th><th>출판사</th><th>작가</th><th>재고</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in books" v-bind:key="item.id">
          <td>{{item.id}}</td>
          <td>{{item.title}}</td>
          <td>{{item.pub}}</td>
          <td>{{item.aut}}</td>
          <td>{{item.stock}}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>


<style>
  table{
    width: 100%;
    border-collapse: collapse;
  }
  tr:nth-of-type(odd){
    background: #eee;
  }
  th{
    background: #333;
    color:white;
    font-weight: bold;
  }
  td,th{
    padding: 6px;
    border: 1px solid #ccc;
    text-align: left;
  }
</style>