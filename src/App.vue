<template>
    <div id="app">
        <div>
            <div class="container">
                <nav class="cyan">
                    <div class="nav-wrapper">
                        <a href="#" class="brand-logo">Groad</a>
                        <a href="#" data-target="nav-mobile" class="sidenav-trigger">
                            <i class="material-icons">menu</i></a>
                        <ul class="right">
                            <li v-for="link in navlinks" :key="link.text">
                            <a :href="link.href">{{link.text}}</a></li>
                        </ul>
                    </div>
                </nav>
            </div>
        </div>
        <!-- 추가 내용 -->
    </div>

  <!-- <div id="app">
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
  </div> -->
</template>
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script src="https://cdnjs/cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css"></script>
    <script src="js/app.js"></script>
    <script src="js/matcon.js"></script>
// <script>
// export default {
//   name:'app',
//   data(){
//     return{
//       books:[
//         {id:1,title:'제목1',pub:'출판사1',aut:'작가1',stock:0},
//         {id:2,title:'제목2',pub:'출판사2',aut:'작가2',stock:1},
//         {id:3,title:'제목3',pub:'출판사3',aut:'작가3',stock:2},
//         {id:4,title:'제목4',pub:'출판사4',aut:'작가4',stock:3},
//         {id:5,title:'제목5',pub:'출판사5',aut:'작가5',stock:4},
//       ]
//     }
//   }
// }
// </script>
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