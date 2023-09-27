<html>
  <div>
    <h1>Modelo de Von Neuman</h1>
  </div>

  <span>
  <strong>Modelo extendido de Von Neumann</strong>
  </span>

<dl>
   <dt>CI</dt>
        <dd>
            Es el conjunto de instrucciones que se llevan a cabo en realizacion de una instrucción. Consta de dos fases búsqueda y ejecución 
            es decir tendra que almacenar el programa en memoria central y el procesador toma  una a una las instrucciones para realizar las tareas. 
        </dd>
  
   <dt>CP</dt>
        <dd>Contador de Programas</dd>
   <dt>RDM</dt>
        <dd>Registro de Memoria</dd>
    <dt>RIM</dt>
        <dd>Registro de intercambio de memoria</dd>
    <dt>ALU</dt>
        <dd>Unidad aritmética lógica</dd>
     <dt>RI</dt>
         <dd>Registo de instrucciones</dd>
    <dt>REN</dt>
        <dd>Registro de entrada</dd>
     <dt>RA</dt>
        <dd>Registro Acumulador</dd>
    
</dl>

<h3>Fase de Búsqueda</h3>
    <ol>
      <li> La unidad de control envía una microorden para que el contenido del CP, sea transferido al RDM</li>
      <li>El selector de memoria utiliza la posición de memoria del RDM y transfiere su contenido <strong>(instrucción)</strong> al RIM</li>
      <li>Se transfiere la instrucción desde el RIM al RI</li>
      <li>El decodificador interpreta la instrucción, se activa la ALU y se informa al secuenciador </li>
      <li>El CP se autoincrementa a través de la ALU con un valor 1, apuntando a la proxima instrucción consecutiva. En el caso de salto 
      se procedera segun la dirección que corresponda</li>
    </ol>
    
    
<h3>Fase de ejecución</h3>
    <ol>
      <li>Se transfiere la dirección del 1º operando desde el RI al RDM</li>
      <li>El selector extrae el dato y lo deposita en el RIM</li>
      <li>Se lleva el operando desde el RIM al REN1 de la ALU</li>
      <li>Repetimos los pasos <strong>1, 2,3 </strong> para el dato del REN2</li>
      <li>El secuenciador envía una microorden a la ALU para que ejecute la operación,
          el resultado lo almacena en el RA</li>
      <li>El resultado se envía desde el RA al RIM</li>
      <li>Se transfiere desde el RI al RDM la dirección del resultado</li>
      <li>Se transfiere el resultado desde el RIM a la dirección de memoria indicada en el RDM</li>
    </ol>

   <img width="601" alt="VonNeumannExt" src="https://github.com/aburcas/smr/assets/84635858/bf659087-3216-4ada-a4ab-088b81b49a3f">


</html>
