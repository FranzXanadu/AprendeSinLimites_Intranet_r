<template>
  <div class="schedule">
    <h2 class="mb-4" style="color: #024716;">Horario de Clases</h2>

    <div class="table-responsive">
      <table class="table table-bordered shadow-sm">
        <thead style="background-color: #55bf84; color: white;">
          <tr>
            <th>Día</th>
            <th>08:00 - 09:00</th>
            <th>09:00 - 10:00</th>
            <th>10:00 - 11:00</th>
            <th>11:00 - 12:00</th>
            <th>12:00 - 13:00</th>
            <th>13:00 - 14:00</th>
            <th>14:00 - 15:00</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Lunes</td>
            <td class="biology">Biología</td>
            <td></td>
            <td class="arithmetic">Aritmética</td>
            <td></td>
            <td class="literature">Lengua y Literatura</td>
            <td></td>
            <td class="history-universal">Historia Universal</td>
          </tr>
          <tr>
            <td>Martes</td>
            <td class="mathematics">Matemáticas</td>
            <td></td>
            <td class="biology">Biología</td>
            <td></td>
            <td class="geography">Geografía</td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td>Miércoles</td>
            <td class="history-peru">Historia del Perú</td>
            <td></td>
            <td class="arithmetic">Aritmética</td>
            <td></td>
            <td class="philosophy">Filosofía</td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td>Jueves</td>
            <td></td>
            <td class="mathematics">Matemáticas</td>
            <td class="history-universal">Historia Universal</td>
            <td></td>
            <td class="literature">Lengua y Literatura</td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td>Viernes</td>
            <td class="arithmetic">Aritmética</td>
            <td></td>
            <td class="biology">Biología</td>
            <td></td>
            <td class="physics">Física</td>
            <td></td>
            <td class="chemistry">Química</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style scoped>
.schedule {
  margin-top: 20px;
}

.table th,
.table td {
  text-align: center;
}

/* Colores para cada materia */
.biology {
  background-color: #ffcc99; /* Amarillo pálido */
}

.arithmetic {
  background-color: #ff9999; /* Rojo pálido */
}

.literature {
  background-color: #99ccff; /* Azul claro */
}

.history-universal {
  background-color: #66ffcc; /* Verde agua */
}

.history-peru {
  background-color: #ffb3e6; /* Rosa claro */
}

.geography {
  background-color: #c2f0c2; /* Verde pálido */
}

.mathematics {
  background-color: #ffcc66; /* Amarillo */
}

.philosophy {
  background-color: #d9d9d9; /* Gris claro */
}

.physics {
  background-color: #ffb3b3; /* Rojo claro */
}

.chemistry {
  background-color: #ffccff; /* Rosa */
}
</style>

