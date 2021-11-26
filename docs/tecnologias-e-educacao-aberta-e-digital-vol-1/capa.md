<style>

body { 
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center; 
}
.button {
  border-radius: 4px;
  background-color: #1E90FF;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 22px;
  padding: 10px;
  width: 200px;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}	


#example3 {
  border-radius: 6px;
  padding: 25px;
  background-color: white;
  background-repeat: no-repeat;
  background-origin: content-box;
  background-position: center;
}

</style>



<div id="example3">
<center> 
<img src="../imagens/capa-vol-1-ebook.png" alt="Avatar" style="width:60%">
</center>
</div>


<!-- 
<center>
    <audio controls>
      <source src="../audio/voice5.mp3" type="audio/mpeg">
    Seu navegador não suporta esta aplicação de áudio.
    </audio>
    </center>

-->