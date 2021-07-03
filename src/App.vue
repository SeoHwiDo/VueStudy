<template>
  <div id="app">
    <div>
      <div class="container">
        <nav class="cyan">
          <div class="nav-wrapper">
            <a href="#" class="brand-logo">
              Groad
            </a>
              <ul class="right">
                <li v-for="link in navlinks" :key="link.text">
                  <a :href="link.href">
                    {{link.text}}
                  </a>
                </li>
              </ul>
          </div>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
    new Vue({
        el:'#app',
        data:{
            navlinks:[
                {text:'마음의 순례길',href:'#pilgrimage'},
                {text:'여행 도우미',href:'#triphelp'},
                {text:'순례길 이야기',href:'#story'},
                {text:'여행정보',href:'#tripinfo'},
                {text:'커뮤니티',href:'#cummunity'}
            ]
        }
    })
</script>
