# skola
nejake veci


function pocitac(){
 //var src = "https://media.novinky.cz/023/610234-top_foto1-rqbcg.jpg?1504857601";
  //document.getElementById("obrazek").src="https://media.novinky.cz/023/610234-top_foto1-rqbcg.jpg?1504857601";
  var pocitac = "https://media.novinky.cz/023/610234-top_foto1-rqbcg.jpg?1504857601";
    
  
  if(document.getElementById("obrazek").src == pocitac){
    alert("Pocitac byl zvolen");
  }
  else{
    document.getElementById("obrazek").src = pocitac;
  }
 
}


function zelva(){
  var zelva = "https://www.rybarskyrozcestnik.cz/wp-content/uploads/2016/02/trachemys-scripta-zelva-nadherna2.jpg";    
  
  if(document.getElementById("obrazek").src == zelva){
    alert("už bylo");
  }
  else{
    document.getElementById("obrazek").src = zelva;
  }
  
}

function jablko(){
 var jablko = "https://www.biovara.cz/images/clanky/jablko.jpg";
  
  if(document.getElementById("obrazek").src == jablko){
    alert("zvolil jsi jablko");
  }
  else{
  document.getElementById("obrazek").src = jablko;
  }
  
}


function zmena(){
 var zelva = "https://www.rybarskyrozcestnik.cz/wp-content/uploads/2016/02/trachemys-scripta-zelva-nadherna2.jpg";
 var pocitac = "https://media.novinky.cz/023/610234-top_foto1-rqbcg.jpg?1504857601";
 var jablko = "https://www.biovara.cz/images/clanky/jablko.jpg";
 
 
 if(document.getElementById("obrazek").src == zelva){
   document.getElementById("obrazek").src = pocitac;
 }
 
  else if(document.getElementById("obrazek").src == pocitac){
   document.getElementById("obrazek").src = jablko;
 }
  
  else if(document.getElementById("obrazek").src == jablko){
   document.getElementById("obrazek").src = zelva;
 }
  
  
}




function potvrd(){
  text = document.getElementById("vstup").value;
  document.getElementById("vypis").innerHTML=text;
}

function seznam(){
 document.getElementById("vypis").innerHTML= "želva, počítač, jablko";
}


function prevzit(){
  var slovo;
  var seznam;
  
  var zelva = "https://www.rybarskyrozcestnik.cz/wp-content/uploads/2016/02/trachemys-scripta-zelva-nadherna2.jpg";
  var pocitac = "https://media.novinky.cz/023/610234-top_foto1-rqbcg.jpg?1504857601";
  var jablko = "https://www.biovara.cz/images/clanky/jablko.jpg";
  
  
  slovo = document.getElementById("vstup").value;
  seznam = document.getElementById("historie").innerHTML;
  
  if(slovo == "zelva"){
    document.getElementById("obrazek").src = zelva;
    seznam = seznam + " zelva";
  }
  
  else if(slovo == "pocitac"){
    document.getElementById("obrazek").src = pocitac;
    seznam = seznam + " pocitac";
  }
  
  else if(slovo == "jablko"){
    document.getElementById("obrazek").src = jablko;
    seznam = seznam + " jablko";
  }
  
  else{
    alert("toto není v seznamu");
    seznam = seznam + " " + slovo;
  }
  document.getElementById("historie").innerHTML = seznam;
}

function smaz(){
  document.getElementById("historie").innerHTML= " ";
}

------------------------------------------------------end-----------------------------------------------------

<!-- <div>
  <button onClick="zmena()">ZMĚNIT</button>
  <button onClick="zelva()">ŽELVA</button>
  <button onClick="pocitac()">POČÍTAČ</button>
  <button onClick="jablko()">JABLKO</button>  
</div>  -->

<!--<div>
  <img id="obrazek" src="https://www.rybarskyrozcestnik.cz/wp-content/uploads/2016/02/trachemys-scripta-zelva-nadherna2.jpg">
</div>  -->

<!--<div>
  <button onClick="seznam()">Zobrazit seznam </button><br>
  <p id="vypis"></p>
</div>  -->

<!--<div>
  <input id="vstup"></input>
<button onClick="prevzit()">Převzít</button>
<button onClick="smaz()">Smaž</button>
<p>Historie hledání</p>
<p id="historie"></p>
</div>  -->
