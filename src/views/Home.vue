<template>
 <div class="flex">
   <div class ="left">
     <!-- <div class ="left-padding">
       <img class ="logo" src="../assets/home.png" />
       <div class="flex icon-field">
         <img class="icon" src="../assets/profile.png" />
         <p>ホーム</p>
       </div>
       <div class="flex icon-field">
         <img class="icon" src="../assets/logout.png" />
         <p>ログアウト</p>
       </div>
     </div>
     <hr />
    <div class="share">
      <p>シェア</p>
      <textarea></textarea>
      <div>
        <button>シェアする</button>
      </div>
    </div> -->
    <SideNavi />
   </div>
   <div class="right">
     <div class="title">
       <p>ホーム</p>
     </div>
     <!-- <div v-for="(value,index) in shares" :key="index">
       <div class="message">
         <div class="flex">
           <p class="name">{{value.name}}</p>
           <img class="icon" src="../assets/heart.png"/>
           <p class="number">{{value.like.length}}</p>
           <img class="icon" src="../assets/cross.png"/>
           <img class="icon detail" src="../assets/detail.png"/>
         </div>
         <p class="text">{{value.share}}</p>
       </div>
     </div> -->
     <Message />
   </div>
 </div>
</template>


<script>
import SideNavi from "../components/SideNavi";
import Message from "../components/Message";
export default {
  components:{
    SideNavi,
    Message
  }
};
</script>

<style scoped>
.left {
  width: 22%;
  height: 100vh;
}
.right {
  width: 78%;
  height: 100vh;
}
.flex {
  display: flex;
}
.title {
  border-bottom: 1px solid white;
  border-left: 1px solid white;
  padding: 15px;
}
.title p {
  font-size: 20px;
  font-weight: bold;
}
 </style>
