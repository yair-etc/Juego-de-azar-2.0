# Juego-de-azar-2.0
es codigo HTML donde devulve el valor despues de 3 intentos erroneos
<meta charset="UTF-8">
<h1>JUEGO DE AZAR</h1>
<script>
  function saltoLinea()  {
    document.write("<br>");
    document.write("<br>");
}
  function imprimir(frase) {
    document.write(frase);  
    saltoLinea();
  }
// ***codigo que si funciona**
  var contador = 1;
  var intentos = 3;
  var numeroPensado = Math.round(Math.random()*10);

    while (contador <= intentos ){
     
      var numeroIngresado = parseInt(prompt("Ingrese un número entero entre 0 y 10."));
     
    if (numeroPensado == numeroIngresado) {
    alert("Usted acertó, en el intento  " + intentos + ", el numero pensado era " + numeroPensado);
    break;
       }
    else {
      alert("Usted erró.");
          }
      contador++;
  }
     
     if (numeroPensado == numeroIngresado) {
    
      imprimir("Usted acertó, en el intento" + intentos + ", el numero pensado era " + numeroPensado);
     }
     else {
               imprimir("Usted erró el numero pensado era  " + numeroPensado);
          }
                contador++;
        imprimir ("fin");

</script>

