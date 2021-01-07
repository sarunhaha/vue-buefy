<template>
    <div class="main"> 
        <ul>
            <li v-for="todo  in todos" :key="todo.time">
                {{todo.text}}
            </li>
        </ul>
        <br><br>
        <!-- v-if , v-else --> 
        <ul>
            <li v-for="todo in todos" :key="todo.time">
                <div v-if="todo.completed == false" >{{todo.text}}</div>
            </li>
            <li></li>
        </ul> 




    </div> 
</template> 

<script>
export default {
    name: 'Main',
    filters: {
        capitalize (val){
            return val.toUpperCase()
        }
    },
    data () {
        return {
            todos: [
                {
                    text: ' Todo 1 ',
                    time: 1070163,
                    completed: true
                },
                {
                    text: ' Todo 2 ',
                    time: 2070163,
                    completed: false
                },
                {
                    text: ' Todo 3 ',
                    time: 3070163,
                    completed: true
                },
                {
                    text: ' Todo 4 ',
                    time: 4070163,
                    completed: true
                }
            ]
        }
    }
}
</script>