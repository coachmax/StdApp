<template>  
    <div>   
        <h1>Hello {{name}}</h1> 
        <input type="text" v-model="name">
        <button @click = "addStudent"> Add </button>
    <h1>Student List</h1>    
         <ul>      
             <li class="big" :class="{red:st.name.length <=3}" v-for="st in student" :key="st.code">        
                <span>{{ st.code }}</span>       
                <span>{{ st.name }}</span>     
             </li>    
         </ul>  
    </div> 
</template>
<script>
export default {
    data() {
        return {
            name: 'Kitphokhin',
        student: [
         { code: '001', name: 'Name1' },
        { code: '002', name: 'Name2' },
        { code: '003', name: 'Name3' },
        { code: '004', name: 'Name4' },
     ],
    }
 },//data
    methods:{
        addStudent(){
            this.student.push({
               code: this.student.length + 1,
               name: this.name, 
            })
        }
    }
}
</script>
<style scoped>
.big {
    font-size: 24px;
}
.red {
    color: red;
}
</style>
