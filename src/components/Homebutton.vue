<template>
    <div class="homebutton">
        <v-btn rounded @click="roundBtnClick">Round버튼</v-btn>
        <v-btn class="teal white-text">기본버튼</v-btn>
        <v-btn color="teal" text>기본버튼</v-btn>
        <v-btn color="teal" dark>
            <v-icon>mdi-bluetooth</v-icon>
            <span>bluetooth</span>
        </v-btn>
        <v-btn fab color="teal" dark>
            <v-icon>mdi-bluetooth</v-icon>
        </v-btn>
    </div>
</template>
<script>
export default {
    mounted(){console.log(this.$vuetify.breakpoint)},
    methods:{roundBtnClick(){console.log("round button");}}
}
</script>