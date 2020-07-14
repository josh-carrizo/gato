<template>
<div class="cont">
    <form action="" class="form">
        <h3>My Form</h3>
        <p class="item-form">Your Name: <input type="text" v-model="nombre" ></p>
        <p class="item-form">Dojo location:
            <select v-model="categoria" >
            <option value="LAX">Los Ángeles</option>
            <option value="CHI">Chicago</option>
            <option value="DFW">Dallas</option>
            <option value="OAK">Oakland</option>
            </select>
        </p>
        <p class="item-form">Favorite Languaje:
            <select v-model="categoria" >
            <option value="python">Python</option>
            <option value="js">Javascript</option>
            <option value="c++">C++</option>
            <option value="java">Java</option>
            </select>
        </p>
        <p class="item-form">Comentaries: <textarea v-model="descripcion" ></textarea></p>
        <p class="item-form"><input  type="checkbox"  v-model="toggle"  true-value="yes"  false-value="no">I agree w/terms and conditions </p>
    
        <p><input type="radio" id="one" value="One" v-model="picked">
            <label for="one">Deseo tener información</label>
            <br>
            <input type="radio" id="two" value="Two" v-model="picked">
            <label for="two">No deseo tener información</label>
            <br>
            <span>Picked: {{ picked }}</span>
            </p>
        <button>Submit</button>
    </form>
</div>
</template>

<script>
export default {
  name: 'FormMenu',
  data: function() {
    return {
      nombre: '',
      categoria: '',
      descripcion: '',
      picked:'',
    }
  }
}
</script>

<style scoped>
* {
  font-family: 'Prompt', sans-serif;
}
.cont{
    padding: 2rem;
    display: inline-block;
    border: 2px black solid;
    border-radius: 1rem;
}
</style>