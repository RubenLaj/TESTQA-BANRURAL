Las correcciones y errores encontrados fueron los siguientes

 <!DOCTYPE html>
<html>
  
<script>



    Error
  let randomNumber = Math.random() * 10;
    La solución 
  let randomNumber = Math.floor(Math.random() * 100) + 1; //En esta parte lo que permite en poder incrementar la cantidad de datos los cuales se le indica que tiene que llegar hasta 
                                                          //el número 100



    El error 
  const ATTEMPS = 5;
    La solución
  const ATTEMPS = 10; //En esta parte se modificó, ya que anteriormente era un 5, pero esto se refiere a la cantidad de datos que se pueden ingresar en el programa, en este caso    
                      //buscamos ingresar 10 datos al programa
  

    El error
  const lowOrHi = document.querySelector('lowOrHi');
    La solución
  const lowOrHi = document.querySelector('.lowOrHi'); //Hizo falta un punto en lowOrHi para que se pueda ejecutar la operación de manera correcta
 




    El error
    guesses.textContent += userGuess + ' ';
    La solución
    guesses.textContent += userGuess + ','; //Acá se encontro un campo vacio, por lo cual pude ver que en ese espacio, en medio de las comillas hacia falta un simbolo, el cual es una coma, la cual lo que hará es separar los números al ingresarlos


    Los errores 

      lastResult.textContent = '!!!Pérdistes!!!';
      lastResult.style.backgroundColor = 'black';
      lowOrHi.textContent = '';
      setGameOver();
    } else if(guessCount === ATTEMPS) {
      lastResult.textContent = 'Felicitaciones! adivinaste el número!';
      lastResult.style.backgroundColor = 'red';
      setGameOver();
    } else {
      lastResult.textContent = 'Incorrecto! ';
      lastResult.style.backgroundColor = 'green';
      if(userGuess < randomNumber) {
        lowOrHi.textContent = 'El número es mayor!';
      } else if(userGuess > randomNumber) {
        lowOrHi.textContent = 'El número es menor!';
      }
    }


    Las solucion y correcciones
      lastResult.textContent = '¡Felicitaciones! ¡Adivinaste el número!'; //Este mensaje se estaba mostrando al terminar el juego y no al ganar, también después de un signo de exclamación se empieza con mayuscula y también hizo falta el otro signo de exclamación al principio
      lastResult.style.backgroundColor = 'black';
      lowOrHi.textContent = '';
      setGameOver();
    } else if(guessCount === ATTEMPS) {
      lastResult.textContent = '¡¡¡Perdiste!!!';   //Por ortografía, no se usa s al terminar la palabra Perdiste y la e no lleva tilde y los signos de exclamación al principio estaban mal 
      lastResult.style.backgroundColor = 'red';
      setGameOver();
    } else {
      lastResult.textContent = '¡Incorrecto! '; //El signo de exclamación al principio hizo falta
      lastResult.style.backgroundColor = 'green';
      if(userGuess < randomNumber) {
        lowOrHi.textContent = '!El número ingresado es muy pequeño! Intenta con otra cantidad'; //Esta instrucción en el programa puede llegar a confundir al usuario, ya que decia que el número es menor, pero tendría que referirse a que el número esta próximo o referirse a que pruebe con un número mas grande, de igual manera los signos de exclamación al principio
      } else if(userGuess > randomNumber) { //Los simbolos <> tambien estaban invertidos para referirse a los números mayores y menores
     
        lowOrHi.textContent = '!El número ingresado es muy mayor! Intenta con otra cantidad'; //Esta instrucción en el programa puede llegar a confundir al usuario, ya que decia que el número es mayor, pero tendría que referirse a que el número esta próximo o referirse a que pruebe con un número mas pequeño, de igual manera los signos de exclamación al principio

      }
    }




    El error 
    guessSubmit.addeventListener('click', checkGuess);
    La solución
    guessSubmit.addEventListener('click', checkGuess);  //El addEventListener poseeía una E minúscula, por lo cual no realizaba su acción 



    El error
      resetButton.addeventListener('click', resetGame);
     La solución
	  resetButton.addEventListener('click', resetGame); //El addEventListener poseeía una E minúscula, por lo cual no realizaba su acción 



    El error
    randomNumber = Math.floor(Math.random()) + 1;
   La solución
	  randomNumber = Math.floor(Math.random() *100) + 1;   //En la parte de acá la operación estaba mal ejecutada, ya que lo que permite es poder incrementar la 
                                                        //cantidad de datos los cuales se le indica que tiene que llegar hasta  el número 100
                                                       
  


