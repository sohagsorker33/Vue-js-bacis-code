  
 <script setup>
import Ref from './components/Ref.vue';
import Loop from './components/Loop.vue';
import Function from './components/Function.vue';
import Hocks from './Hocks.vue';
 
 
 

    let msg="Welcomome to our vue js 3 composition"
    let userId=2
    let userName=true
    
    let obj={
      class:"container",
      id:"row"
    }
    let seen=true
    let google="https://www.google.com/"
    let clickMe=()=>{
      console.log("click");
    }

    // number auto increment 

    import { ref } from 'vue'

    
   let number=ref(0)
   let count=ref(0)
    setInterval(() => {
      number.value++
    },200);
 
    
 </script>
 
 <template>
  
 <h1 v-text="msg"></h1>
 <hr>
  <div v-bind:num="userId"></div>
  <hr>
 <button :disabled="userName">button</button>
 <hr>
 <div :="obj">object</div>
 <hr>
 <div v-if="seen">amar soner bangla ami tomai valobasi</div>
 <hr>
  <a :href="google">Google</a>
  <hr>
 <button @click="clickMe">ClickMe {{ number }}</button>
 <hr>
 <button @click="count++"> clicked{{ count }}</button>
 <hr>
  
<Ref/>
<hr>
<Loop/>
<hr>
<Function/>
 <hr>
 <Hocks/>


 

</template>
