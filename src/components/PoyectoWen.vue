<script>
export default {
  data() {
    return {
      input1: false,
      input2: false,
      input3: false,
      input4: false,
      input5: false,
      input6: false,
      numero: null,
      numero2: null,
      numero3: null,
      numero4: null,
      numero5: null, 
      numero6: null,
      resultado: null,
      resultado2: null,
      resultado3: null,
      resultado4: null,
      resultado5: null,
      resultado6: null,
      gly1: false,
      cre1: false,
      aci1: false,
      col1: false,
      tri1: false,
      hdl1: false,

      gly2: null,
      cre2: null,
      aci2: null,
      col2: null,
      tri2: null,
      hdl2: null,

      gly3: null,
      cre3: null,
      aci3: null,
      col3: null,
      tri3: null,
      hdl3: null,

      color: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolor: 'rgb(218, 218, 218)',
      colores: 0,
      color2: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolor2: 'rgb(218, 218, 218)',
      colores2: 0,
      color3: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolor3: 'rgb(218, 218, 218)',
      colores3: 0,
      color4: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolor4: 'rgb(218, 218, 218)',
      colores4: 0,
      color5: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolor5: 'rgb(218, 218, 218)',
      colores5: 0,
      color6: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolor6: 'rgb(218, 218, 218)',
      colores6: 0,
      
      colorg: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolorg: 'rgb(218, 218, 218)',
      coloresg: 0,
      colorc: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolorc: 'rgb(218, 218, 218)',
      coloresc: 0,
      colora: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolora: 'rgb(218, 218, 218)',
      coloresa: 0,
      colorco: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolorco: 'rgb(218, 218, 218)',
      coloresco: 0,
      colort: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolort: 'rgb(218, 218, 218)',
      colorest: 0,
      colorh: ['rgb(218, 218, 218)', 'rgb(34, 34, 34)'],
      botoncolorh: 'rgb(218, 218, 218)',
      coloresh: 0,
    };
  },
  methods: {
    mostrar1() {
      this.input1 = !this.input1;
      this.resultado = null;
      this.numero = null;
      this.colores = 1 - this.colores;
      this.botoncolor = this.color[this.colores];
    },
    mostrar2(){
      this.input2 = !this.input2;
      this.resultado2 = null;
      this.numero2 = null
      this.colores2 = 1 - this.colores2;
      this.botoncolor2 = this.color2[this.colores2];
    },
    mostrar3(){
      this.input3 = !this.input3;
      this.numero3 = null;
      this.resultado3 = null;
      this.colores3 = 1 - this.colores3;
      this.botoncolor3 = this.color3[this.colores3];
    },
    mostrar4(){
      this.input4 = !this.input4;
      this.numero4 = null;
      this.resultado4 = null;
      this.colores4 = 1 - this.colores4;
      this.botoncolor4 = this.color4[this.colores4];
    },
    mostrar5(){
      this.input5 = !this.input5;
      this.numero5 = null;
      this.resultado5 = null;
      this.colores5 = 1 - this.colores5;
      this.botoncolor5 = this.color5[this.colores5];
    },
    mostrar6(){
      this.input6 = !this.input6;
      this.numero6 = null;
      this.resultado6 = null;
      this.colores6 = 1 - this.colores6;
      this.botoncolor6 = this.color6[this.colores6];
    },
    resultados(){
      this.resultado=parseFloat(this.numero)
      this.resultado2=parseFloat(this.numero2)
      this.resultado3=parseFloat(this.numero3)
      this.resultado4=parseFloat(this.numero4)
      this.resultado5=parseFloat(this.numero5)
      this.resultado6=parseFloat(this.numero6)
    },
    gly(){
      this.gly1 = !this.gly1;
      this.gly2 = null;
      this.gly3 = null;
      this.coloresg = 1 - this.coloresg;
      this.botoncolorg = this.colorg[this.coloresg];
    },
    cre(){
      this.cre1 = !this.cre1;
      this.cre2 = null;
      this.cre3 = null;
      this.coloresc = 1 - this.coloresc;
      this.botoncolorc = this.colorc[this.coloresc];
    },
    aci(){
      this.aci1 = !this.aci1;
      this.aci2 = null;
      this.aci3 = null;
      this.coloresa = 1 - this.coloresa;
      this.botoncolora = this.colora[this.coloresa];
    },
    col(){
      this.col1 = !this.col1;
      this.col2 = null;
      this.col3 = null;
      this.coloresco = 1 - this.coloresco;
      this.botoncolorco = this.colorco[this.coloresco];
    },
    tri(){
      this.tri1 = !this.tri1;
      this.tri2 = null;
      this.tri3 = null;
      this.colorest = 1 - this.colorest;
      this.botoncolort = this.colort[this.colorest];
    },
    hdl(){
      this.hdl1 = !this.hdl1;
      this.hdl2 = null;
      this.hdl3 = null;
      this.coloresh = 1 - this.coloresh;
      this.botoncolorh = this.colorh[this.coloresh];
    },
    todo(){
      this.gly3 = parseInt(this.gly2);
      this.cre3 = parseFloat(this.cre2);
      this.aci3 = parseFloat(this.aci2);
      this.col3 = parseInt(this.col2);
      this.tri3 = parseInt(this.tri2);
      this.hdl3 = parseInt(this.hdl2);
    }
  },
};
</script>

<template class="fondo">
  
     <div class="todo"><div class="titulo">
   <h1 style="text-shadow: 4px 2px 4px black; font-style: oblique;">LABORATORIO DE ANÁLISIS CLÍNICO</h1>
   <h2 style="font: serif">(control de conteo de un hemograma y análisis químico sanguíneo)</h2> 
  </div>
  <div class="nav"> 
    <nav>
        <a href="https://elpais.com/noticias/laboratorios/">Noticias</a>
        <a href="https://www.inlasa.gob.bo/divisiones/diagnostico/analisis-clinico/sd\">Más información</a>
        <a href="https://www.youtube.com/watch?v=z2kMOioyRJQ">Video informativo </a>
    </nav>
</div>
    
    <div class="cuadro2">
      <div class="letra">Menú</div>
      <div class="letra">"Hemograma"</div>
      <button @click="mostrar1" :style="{background: botoncolor}" class="boton">
        {{ input1 ? 'Glóbulos rojos' : 'Glóbulos rojos' }}
      </button><br/>
      <button @click="mostrar2" :style="{background: botoncolor2}" class="boton">
        {{ input2 ? 'Glóbulos blanco': 'Glóbulos blancos' }}
      </button><br/>
      <button @click="mostrar3" :style="{background: botoncolor3}" class="boton">
        {{ input3 ? 'Hematocrito' : 'Hematocrito' }}
      </button><br/>
      <button @click="mostrar4" :style="{background: botoncolor4}" class="boton">
        {{ input4 ? 'Hemoglobina' : 'Hemoglobina' }}
      </button><br/>
      <button @click="mostrar5" :style="{background: botoncolor5}" class="boton">
        {{ input5 ? 'V.E.S 1ra hora' : 'V.E.S 1ra hora' }}
      </button><br/>
      <button @click="mostrar6" :style="{background: botoncolor6}" class="boton">
        {{ input6 ? 'Plaquetas' : 'Plaquetas' }}
      </button>
    </div>
    <div class="cuadro1">
      <div style="color: rgb(129, 67, 6); font-size: 20px; text-shadow: 1.5rem rgb(224, 17, 17);"><h3>Elija un componente del hemograma o del análisis químico y introduzca el número o dato del análisis sanguíneo</h3></div>
         <div class="conteo">
        <div v-if="input1">
          <div style="color: rgb(37, 31, 25);"><h3>Glóbulos rojos 'mm^3'</h3></div>
          <input type="number" placeholder="Glóbulos rojos mm^3" v-model="numero"/>
        </div>
        <div v-if="input2">
          <div style="color: rgb(37, 31, 25);"><h3>Glóbulos blanco 'mm^3'</h3></div>
          <input type="number" placeholder="Glóbulos blancos mm^3" v-model="numero2"/>
        </div>
        <div v-if="input3">
          <div style="color: rgb(37, 31, 25);"><h3>Hematocrito '%'</h3></div>
          <input type="number" placeholder="Hematocritos %" v-model="numero3"/>
        </div>
        <div v-if="input4">
          <div style="color: rgb(37, 31, 25);"><h3>Hemoglobina 'gr/%'</h3></div>
          <input type="number" placeholder="Hemoglobina gr/%" v-model="numero4"/>
        </div>
        <div v-if="input5">
          <div style="color: rgb(37, 31, 25);"><h3>V.E.S. 1ra hora 'mm'</h3></div>
          <input type="number" placeholder="V.E.S 1ra hora mm" v-model="numero5"/>
        </div>
        <div v-if="input6">
          <div style="color: rgb(37, 31, 25);"><h3>Plaquetas 'mm^3'</h3></div>
          <input type="number" placeholder="Plaquetas mm^3" v-model="numero6"/>
        </div>
        
            <div v-if="resultado >= 4800000 && resultado <= 5800000" style="color: rgb(37, 31, 25);">Globulos Rojos saludable</div>
            <div v-else-if="resultado2 >= 5000 && resultado2 <= 10000" style="color: rgb(37, 31, 25);">Globulos Blancos saludable</div>
            <div v-else-if="resultado3 >= 46 && resultado3 <= 52" style="color: rgb(37, 31, 25);">Hematocrito Saludable</div>
            <div v-else-if="resultado4 >= 14.5 && resultado4 <= 16.5" style="color: rgb(37, 31, 25);">Hemoglobina saludable</div>
            <div v-else-if="resultado5 < 10 && resultado5 >0" style="color: rgb(37, 31, 25);">V.E.S Saludable</div>
            <div v-else-if="resultado6 >= 150 && resultado6 <= 400" style="color: rgb(37, 31, 25);">Plaquetas Saludable</div>
            <div v-else-if="resultado == null || resultado2 == null || resultado3 == null
            || resultado4 == null || resultado5 == null || resultado6 == null"></div>
            <div v-else="" style="color: rgb(37, 31, 25);">
              <div v-if="resultado < 4800000" style="color: rgb(37, 31, 25);">Globulos Rojos Bajos</div>
              <div v-else-if="resultado2 < 5000" style="color: rgb(37, 31, 25);">Globulos Blancos Bajos</div>
              <div v-else-if="resultado3 < 46" style="color: rgb(37, 31, 25);">Hematocrito Bajos</div>
              <div v-else-if="resultado4 < 14.5" style="color: rgb(37, 31, 25);">Hemoglobina Bajos</div>
              <div v-else-if="resultado5 > 10" style="color: rgb(37, 31, 25);">V.E.S alto</div>
              <div v-else-if="resultado6 < 150" style="color: rgb(37, 31, 25);">Plaquetas Bajos</div>
              <div v-else="">
                <div v-if="resultado > 5800000" style="color: rgb(37, 31, 25);">Globulos Rojos Altos</div>
                <div v-else-if="resultado2 > 10000" style="color: rgb(37, 31, 25);">Globulos Blancos Altos</div>
                <div v-else-if="resultado3 > 52" style="color: rgb(37, 31, 25);">Hematocrito Altos</div>
                <div v-else-if="resultado4 > 16.5" style="color: rgb(37, 31, 25);">Hemoglobina Altos</div>
                <div v-else-if="resultado6 > 400" style="color: rgb(37, 31, 25);">Plaquetas Altos</div>
              </div>
            </div>
            <button @click="resultados" style="color: rgb(39, 36, 36);" class="boton">Calcular</button>
         </div>
        <div class="quimica">
              <div v-if="gly1">
                <div style="color: rgb(37, 31, 25);"><h3>Glycemia</h3></div>
                <input type="number" placeholder="Glycemia" v-model="gly2"/>
              </div>
              <div v-if="cre1">
              <div style="color: rgb(37, 31, 25);"><h3>Creatinna</h3></div>
              <input type="number" placeholder="Creatinna" v-model="cre2"/>
            </div>
            <div v-if="aci1">
              <div style="color: rgb(37, 31, 25);"><h3>Acido Urico</h3></div>
              <input type="number" placeholder="Acido Urico" v-model="aci2"/>
            </div>
            <div v-if="col1">
              <div style="color: rgb(37, 31, 25);"><h3>Colesterol Maximo</h3></div>
              <input type="number" placeholder="Colesterol Maximo" v-model="col2"/>
            </div>
            <div v-if="tri1">
              <div style="color: rgb(37, 31, 25);"><h3>Trigliceridos</h3></div>
              <input type="number" placeholder="Trigliceridos" v-model="tri2"/>
            </div>
            <div v-if="hdl1">
              <div style="color: rgb(37, 31, 25);"><h3>HDL Colesterol</h3></div>
              <input type="number" placeholder="HDL Colesterol" v-model="hdl2"/>
            </div>
            
              <div v-if="gly3 >= 70 && gly3 <= 115" style="color: rgb(37, 31, 25);">Glycemia Saludable</div>
              <div v-else-if="cre3 >= 0.7 && cre3 <= 1.5" style="color: rgb(37, 31, 25);">Creatinna Saludable</div>
              <div v-else-if="aci3 >= 1.5 && aci3 <= 7" style="color: rgb(37, 31, 25);">Acido Urico Saludable</div>
              <div v-else-if="col3 > 0 && col3 <= 240" style="color: rgb(37, 31, 25);">Colesterol Maximo saludable</div>
              <div v-else-if="tri3 >= 60 && tri3 <= 165" style="color: rgb(37, 31, 25);">Trigliceridos Saludable</div>
              <div v-else-if="hdl3 > 45" style="color: rgb(37, 31, 25);">DHL Colesterol Saludable</div>
              <div v-else-if="gly3 == null || cre3 == null || aci3 == null
              || col3 == null || tri3 == null || hdl3 == null"></div>
              <div v-else="" style="color: rgb(37, 31, 25);">
                <div v-if="gly3 < 70" style="color: rgb(37, 31, 25);">Glycemia Bajos</div>
                <div v-else-if="cre3 < 0.7" style="color: rgb(37, 31, 25);">Creatinna Bajos</div>
                <div v-else-if="aci3 < 1.5" style="color: rgb(37, 31, 25);">Acido Urico Bajos</div>
                <div v-else-if="tri3 < 60" style="color: rgb(37, 31, 25);">Trigliceridos Bajos</div>
                <div v-else-if="hdl3 < 45" style="color: rgb(37, 31, 25);">DHL Colesterol Bajos</div>
                <div v-else="">
                  <div v-if="gly3 > 115" style="color: rgb(37, 31, 25);">Glycemia Altos</div>
                  <div v-else-if="cre3 > 1.5" style="color: rgb(37, 31, 25);">Creatinna Altos</div>
                  <div v-else-if="aci3 > 7" style="color: rgb(37, 31, 25);">Acido Urico Altos</div>
                  <div v-else-if="col3 > 240" style="color: rgb(37, 31, 25);">Colesterol Maximo Altos</div>
                  <div v-else-if="tri3 > 165" style="color: rgb(37, 31, 25);">Trigliceridos Altos</div>
                </div>
              </div>
            <button @click="todo" style="color: rgb(39, 36, 36);" class="boton">Calcular</button>
        </div>
    </div>
    <div class="cuadro3">
      <div class="letra">Menú</div>
      <div class="letra">"Estudio químico sanguíneo"</div>
      <button @click="gly" :style="{background: botoncolorg}" class="boton">
        {{ gly1 ? 'Glycemia' : 'Glycemia' }}
      </button><br/>
      <button @click="cre" :style="{background: botoncolorc}" class="boton">
        {{ cre1 ? 'Creatinna': 'Creatinna' }}
      </button><br/>
      <button @click="aci" :style="{background: botoncolora}" class="boton">
        {{ aci1 ? 'Acido Urico' : 'Acido Urico' }}
      </button><br/>
      <button @click="col" :style="{background: botoncolorco}" class="boton">
        {{ col1 ? 'Colesterol Maximo' : 'Colesterol Maximo' }}
      </button><br/>
      <button @click="tri" :style="{background: botoncolort}" class="boton">
        {{ tri1 ? 'Trigliceridos' : 'Trigliceridos' }}
      </button><br/>
      <button @click="hdl" :style="{background: botoncolorh}" class="boton">
        {{ hdl1 ? 'HDL Colesterol Maximo' : 'HDL Colesterol Maximo' }}
      </button>
    </div>
  </div>

    <div class="c2">
        <p v>LIC.MIGUEL DE SEVILLA CHAVES GORDILLO</p>
    </div>
    
    <footer class="c1">
        <p>JHANNET QUISBERT CONDORI___________ISAIAS GUZMAN ERAZO____________MAURICIO ZAMORA RIVAS</p>
    </footer>

</template>

<style scoped>

*{
  background: none;
  margin: 0px;
  padding: 0px;
  
}
.cuadro3{
  display: inline-block;
  margin: 0px 0 0 -260px;
  border: 4px solid rgba(191, 191, 233, 0.945);
  width: 267px;
  height: 550px;
  left: 1390px;
  position: absolute;
  float: right;
  background-image: url(https://us.123rf.com/450wm/lindrik/lindrik1902/lindrik190200227/117290581-vista-de-la-orilla-del-mar-b%C3%A1ltico.jpg?ver=6);
  background-size: 100% 100%;
  background-attachment: fixed;
}
.cuadro2{
  display: inline-block;
  margin: 0 0 0 0;
  border: 4px solid rgba(83, 124, 200, 0.549);
  width: 250px;
  height: 550px;
  position: relative;
  float: left;
  background-image: url(https://us.123rf.com/450wm/lindrik/lindrik1902/lindrik190200227/117290581-vista-de-la-orilla-del-mar-b%C3%A1ltico.jpg?ver=6);
  background-size: 100% 100%;
  background-attachment: fixed;
}
.cuadro1{
  display: inline-block;
  margin: 0 270px 0 0;
  border: 4px solid rgba(83, 124, 200, 0.549);
  width: 740px;
  height: 550px;
  position: relative;

  background-image:url(https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcRXWlDqxcQ9RFRRS7MOWvhkSrib6Eq6oHoW6ADRi6QHMQBJcla9);
  background-size: 100% 100%;
  background-attachment: fixed;
}
.letra{
  font-size: 30px;
  font-weight: 600;

  background: rgb(216, 201, 201);
  color: rgb(37, 31, 25);
  font-family: Helvetica, Arial, sans-serif;
}

.boton {
  margin: 25px 0 10px 0;
  width: 200px;
  font-weight: 800;
  color: rgb(189, 137, 223);
  cursor: pointer;

  background: rgb(255, 232, 207);
}
.titulo{
  border: 4px solid rgb(4, 4, 74);
  width: 100%;
  margin: 0 0 0 0;
  background-image:url(https://us.123rf.com/450wm/lindrik/lindrik1408/lindrik140800110/30789418-d%C3%ADas-de-mar-hermoso-paisaje-marino.jpg?ver=6);
  color: rgb(184, 208, 202);
  background-size:100%;
  background-attachment: fixed;
}

.footer{
  display: block;
  width: 100%;
  height: 100px;
  border: 1px solid red;
  background-color: blue;
  
}
.quimica{
  display: inline-block;
  margin: 0 0 0 75px;
  position: relative;
  color: black;
}
.quimica input{
  color: black;
}
.conteo{
  display: inline-block;
  margin: 0 0 0 0;
  position: relative;
}
.conteo input{
  color: black;
}
.nav{
    width: 1276px;
    height: 30px;
    display: flex;
    flex-direction: row;
    background-color: rgb(161, 209, 193);
    border: 4px solid rgba(83, 124, 200, 0.549);
}
.nav a{
color: black;
padding: 14pc 20px;
text-decoration: none;
}

</style>