<template>
    
    
    <!-- <i class="bi bi-eye">ojo</i>
    <i class="bi bi-people"></i> -->


    
          <form :state="formstate" @submit.prevent="onSubmit">
            <div class="container" >
                <div class="row">
                         <h3>Formulario</h3>
                     <div>
                         <validate tag="label">
                             <div class="input-group mb-3">
                               <span class="input-group-text" id="basic-addon1"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-people" viewBox="0 0 16 16">
                                  <path d="M15 14s1 0 1-1-1-4-5-4-5 3-5 4 1 1 1 1h8Zm-7.978-1A.261.261 0 0 1 7 12.996c.001-.264.167-1.03.76-1.72C8.312 10.629 9.282 10 11 10c1.717 0 2.687.63 3.24 1.276.593.69.758 1.457.76 1.72l-.008.002a.274.274 0 0 1-.014.002H7.022ZM11 7a2 2 0 1 0 0-4 2 2 0 0 0 0 4Zm3-2a3 3 0 1 1-6 0 3 3 0 0 1 6 0ZM6.936 9.28a5.88 5.88 0 0 0-1.23-.247A7.35 7.35 0 0 0 5 9c-4 0-5 3-5 4 0 .667.333 1 1 1h4.216A2.238 2.238 0 0 1 5 13c0-1.01.377-2.042 1.09-2.904.243-.294.526-.569.846-.816ZM4.92 10A5.493 5.493 0 0 0 4 13H1c0-.26.164-1.03.76-1.724.545-.636 1.492-1.256 3.16-1.275ZM1.5 5.5a3 3 0 1 1 6 0 3 3 0 0 1-6 0Zm3-2a2 2 0 1 0 0 4 2 2 0 0 0 0-4Z"/>
                                  </svg></span>   
                                <input type="text" class="form-control" maxlength="9" placeholder="Ingrese su nombre" name="nombre" id="nombre" aria-label="nombre" aria-describedby="basic-addon1" v-model="nombre" required>
                                <span >&nbsp;* </span>
                                
                              </div>
                             <!-- <div v-if="Error" class="error-message text-danger">{{ Error }}</div> -->
                         </validate>
                     </div>
                     <div>
                         <validate tag="label">
                                <div class="input-group mb-3">
                                  <span class="input-group-text" id="basic-addon2"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-people" viewBox="0 0 16 16">
                                      <path d="M15 14s1 0 1-1-1-4-5-4-5 3-5 4 1 1 1 1h8Zm-7.978-1A.261.261 0 0 1 7 12.996c.001-.264.167-1.03.76-1.72C8.312 10.629 9.282 10 11 10c1.717 0 2.687.63 3.24 1.276.593.69.758 1.457.76 1.72l-.008.002a.274.274 0 0 1-.014.002H7.022ZM11 7a2 2 0 1 0 0-4 2 2 0 0 0 0 4Zm3-2a3 3 0 1 1-6 0 3 3 0 0 1 6 0ZM6.936 9.28a5.88 5.88 0 0 0-1.23-.247A7.35 7.35 0 0 0 5 9c-4 0-5 3-5 4 0 .667.333 1 1 1h4.216A2.238 2.238 0 0 1 5 13c0-1.01.377-2.042 1.09-2.904.243-.294.526-.569.846-.816ZM4.92 10A5.493 5.493 0 0 0 4 13H1c0-.26.164-1.03.76-1.724.545-.636 1.492-1.256 3.16-1.275ZM1.5 5.5a3 3 0 1 1 6 0 3 3 0 0 1-6 0Zm3-2a2 2 0 1 0 0 4 2 2 0 0 0 0-4Z"/>
                                      </svg></span>   
                                  <input type="text" class="form-control" maxlength="9" placeholder="Ingrese su apellido" name="apellido" id="apellido" aria-label="apellido" aria-describedby="basic-addon1" v-model="apellido" required>
                                  <span >&nbsp;* </span>
                                </div>
                                 <!-- <div v-if="Error" class="error-message text-danger">{{ Error }}</div> -->
                            </validate>
                     </div>
                     <div>
                        <validate tag="label">
                                   <div class="input-group mb-3">
                                     <span class="input-group-text" id="basic-addon3">@</span>   
                                     <input type="email" class="form-control"  placeholder="email@email.com" name="correo" id="correo" aria-label="correo" aria-describedby="basic-addon1" v-model="correo"  required>
                                     <span >&nbsp;*</span>
                                   </div>
                                    <!-- <div v-if="Error" class="error-message text-danger">{{ Error }}</div> -->
                            </validate>
                     </div>
                     <div>
                         <validate tag="label">
                               <div class="input-group mb-3">
                                 <span class="input-group-text" id="basic-addon4"><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-unlock" viewBox="0 0 16 16">
                                 <path d="M11 1a2 2 0 0 0-2 2v4a2 2 0 0 1 2 2v5a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V9a2 2 0 0 1 2-2h5V3a3 3 0 0 1 6 0v4a.5.5 0 0 1-1 0V3a2 2 0 0 0-2-2zM3 8a1 1 0 0 0-1 1v5a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1V9a1 1 0 0 0-1-1H3z"/>
                                 </svg></span>   
                                 <input type="password" class="form-control" maxlength="9" name="clave" id="clave" placeholder="Ingrese su clave" aria-label="clave" aria-describedby="basic-addon1" v-model="clave" required>
                                  <span >&nbsp;*</span>
                                </div>
                                 <!-- <div v-if="Error" class="error-message text-danger">{{ Error }}</div> -->
                           </validate>
                     </div>
                </div>
            </div>
             <div class="container">
                    <div class="row">
                        <validate>                    
                               <h4>Selecciona tus curso</h4>
                       <div>
                         <input type="checkbox" id="checkJS" v-model="curso" value="javascript"/>
                         <label for="checkJS">&nbsp;JavaScript</label>
                       </div>
                       <div>
                         <input type="checkbox" id="checkReact" v-model="curso" value="react" />
                         <label for="checkReact">&nbsp;React</label>
                       </div>
                       <div>
                         <input type="checkbox" id="checkNg" v-model="curso" value="angular" />
                         <label for="checkNg">&nbsp;Angular</label>
                       </div>
                       <div>
                         <input type="checkbox" id="checkVue" v-model="curso" value="vue" />
                         <label for="checkVue">&nbsp;Vue</label>
                       </div>
                       </validate>
                      </div>
                      <div v-if="Error" class="error-message text-danger mt-1">{{ Error }}</div> 
         
                    </div>
                        <div class="container">
                            <div >
                           <validate>
                               <button type="submit" @click="enviarDatos"  class="btn btn-dark mb-5 mt-2">Enviar</button>
                           </validate>    
                          
                        </div>
                        </div>
             </form>


</template>

<script>
export default {
  name: 'FormularioWeb',
  props: {

  },
  data() {
    return {
      formstate: {},
      nombre: "",
      apellido: "",
      correo: "",
      clave: "",
      curso: [],
      Error: false,
      vacio: " "
    }
  },
  methods: {
    enviarDatos() {


      if (!this.nombre || !this.apellido || !this.correo || !this.clave || this.curso.length === 0) {
        // Al menos uno de los campos requeridos está vacío
        // Puedes mostrar un mensaje de error o realizar alguna acción aquí
        this.Error = "Este campo es obligatorio"
        return;
      } 


       
      const datos = {
        nombre: this.nombre,
        apellido: this.apellido,
        correo: this.correo,
        clave: this.clave,
        curso: this.curso,          
      };
      
      this.$emit('datos-enviados', datos);
      this.resetearCampos();
     
    },
    resetearCampos() {
    
      this.nombre = ""; 
      this.apellido = "";  
      this.correo = "";
      this.clave = "";
      this.curso = [];  
  
},
  },
}
  

  

      
    

</script>

<style scoped>

button{
  width: 250px;
}
#checkReact{
  margin-left:-34px;
}
#checkNg{
  margin-left: -20px;
}
#checkVue{
  margin-left: -48px;
}
.error-message{
margin-top:-15px ;
}

</style>