FUNCIONES DEL TIC TAC TOE


Square : es una función que representa las casillas en el tablero del juego. Toma dos valores: el valor que contiene el cuadrado (ya sea "X" o "O") y la función que se ejecuta cuando se da click en la casilla. Retorna un buton

Board: es una función que representa el tablero del juego. Toma tres valores: el valor booleano que indica si es el turno del jugador "X" o del jugador "O", un array que representa el estado actual de los cuadrados en el tablero y la función que se ejecuta cuando se da click en una casilla.

handleClick: esta función esta dentro de la funcion Board y se ejecuta cuando se hace click en una casilla en el tablero. Toma el numero de la casilla que se ha hecho click. Verifica si ya hay un ganador o si la casilla ya ha sido marcada, en cuyo caso no hace nada. Si la casilla no ha sido marcada y no hay un ganador, actualiza el estado de laas casillas con el nuevo valor ("X" o "O") y llama a la función onplay pasando el nuevo estado como argumento.

winner: esta variable contiene el resultado de la función calculateWinner, que verifica si hay un ganador en el tablero y devuelve el valor del ganador ("X" o "O") o null si no hay ganador. Ademas, esta función toma el estado actual de los cuadrados en el tablero y verifica si hay un ganador. Comprueba todas las combinaciones posibles de tres cuadrados que podrían llevar a un ganador ya sea horizontal |, vertical --- o cruzado / . Si encuentra una combinación en la que todos los cuadrados son iguales devuelve el valor del ganador ("X" o "O"). Si no hay ganador, devuelve null.

Game(): esta función es la principal de todo el juego. Contiene el estado actual del juego, el historial de movimientos y el movimiento actual. Tambien, las funciones que se ejecutan cuando se juega (handlePlay) y se hace clic en un movimiento anterior (JumpTo). El estado se gestiona con la función "useState" de React. La función "handlePlay" se ejecuta cuando se hace clic en un cuadrado y actualiza el historial y el movimiento actual. La función "jumpTo" se ejecuta cuando se hace clic en un movimiento anterior y actualiza el movimiento actual..
