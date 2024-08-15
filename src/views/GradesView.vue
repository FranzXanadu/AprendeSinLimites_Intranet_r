<template>
    <div class="grades-view">
      <h2 class="mb-4" style="color: #024716;">Calificaciones</h2>
      
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="table-responsive">
              <table class="table table-bordered">
                <thead class="thead-light">
                  <tr>
                    <th>Asignatura</th>
                    <th>Calificación</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>Matemáticas</td>
                    <td><span class="grade" :class="getGradeClass(18)">18</span></td>
                  </tr>
                  <tr>
                    <td>Aritmética</td>
                    <td><span class="grade" :class="getGradeClass(9)">9</span></td>
                  </tr>
                  <tr>
                    <td>Geometría</td>
                    <td><span class="grade" :class="getGradeClass(12)">12</span></td>
                  </tr>
                  <tr>
                    <td>Biología</td>
                    <td><span class="grade" :class="getGradeClass(14)">14</span></td>
                  </tr>
                  <tr>
                    <td>Química</td>
                    <td><span class="grade" :class="getGradeClass(19)">19</span></td>
                  </tr>
                  <tr>
                    <td>Historia Universal</td>
                    <td><span class="grade" :class="getGradeClass(16)">16</span></td>
                  </tr>
                  <tr>
                    <td>Historia del Perú</td>
                    <td><span class="grade" :class="getGradeClass(11)">11</span></td>
                  </tr>
                  <tr>
                    <td>Geografía</td>
                    <td><span class="grade" :class="getGradeClass(15)">15</span></td>
                  </tr>
                  <tr>
                    <td>Lengua y Literatura</td>
                    <td><span class="grade" :class="getGradeClass(13)">13</span></td>
                  </tr>
                  <tr>
                    <td>Comunicación</td>
                    <td><span class="grade" :class="getGradeClass(10)">10</span></td>
                  </tr>
                  <tr>
                    <td>Filosofía</td>
                    <td><span class="grade" :class="getGradeClass(17)">17</span></td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      getGradeClass(grade) {
        if (grade <= 10) {
          return 'text-danger'; // Color rojo
        } else if (grade === 11 || grade === 12) {
          return 'text-warning'; // Color naranja
        } else {
          return 'text-success'; // Color verde
        }
      }
    }
  }
  </script>
  
  <style scoped>
  .grades-view {
    padding: 20px;
  }
  
  .grade {
    font-weight: bold;
  }
  </style>
  