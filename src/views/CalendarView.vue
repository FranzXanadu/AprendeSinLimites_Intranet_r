<template>
  <div class="calendar-view">
    <h2 class="mb-4" style="color: #024716;">Calendario de Eventos</h2>

    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <div class="table-responsive">
            <table class="table table-bordered">
              <thead class="thead-light">
                <tr>
                  <th colspan="7" class="text-center" style="color: #024716;">Agosto 2024</th>
                </tr>
                <tr>
                  <th>Lunes</th>
                  <th>Martes</th>
                  <th>Miércoles</th>
                  <th>Jueves</th>
                  <th>Viernes</th>
                  <th>Sábado</th>
                  <th>Domingo</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td>
                    <strong>1</strong><br />
                    <span class="event" style="background-color: #ff8c00;">Entrega de Tareas de Matemáticas</span>
                  </td>
                  <td>
                    <strong>2</strong><br />
                    <span class="event" style="background-color: #b8860b;">Simulacro de Examen de Química</span>
                  </td>
                  <td>
                    <strong>3</strong>
                  </td>
                  <td>
                    <strong>4</strong>
                  </td>
                  <td>
                    <strong>5</strong><br />
                    <span class="event" style="background-color: #ff8c00;">Entrega de Tareas de Física</span>
                  </td>
                  <td>
                    <strong>6</strong><br />
                    <span class="event" style="background-color: #55bf84;">Taller de Biología</span>
                  </td>
                  <td>
                    <strong>7</strong><br />
                    <span class="event" style="background-color: #ff8c00;">Exposición de Proyectos</span>
                  </td>
                </tr>
                <tr>
                  <td>
                    <strong>8</strong><br />
                    <span class="event" style="background-color: #ff8c00;">Entrega de Tareas de Lengua y Literatura</span>
                  </td>
                  <td>
                    <strong>9</strong>
                  </td>
                  <td>
                    <strong>10</strong><br />
                    <span class="event" style="background-color: #55bf84;">Taller de Geografía</span>
                  </td>
                  <td>
                    <strong>11</strong>
                  </td>
                  <td>
                    <strong>12</strong><br />
                    <span class="event" style="background-color: #b8860b;">Simulacro de Examen de Historia Universal</span>
                  </td>
                  <td>
                    <strong>13</strong>
                  </td>
                  <td>
                    <strong>14</strong>
                  </td>
                </tr>
                <tr>
                  <td>
                    <strong>15</strong><br />
                    <span class="event" style="background-color: #ff8c00;">Entrega de Tareas de Biología</span>
                  </td>
                  <td>
                    <strong>16</strong>
                  </td>
                  <td>
                    <strong>17</strong><br />
                    <span class="event" style="background-color: #55bf84;">Taller de Filosofía</span>
                  </td>
                  <td>
                    <strong>18</strong><br />
                    <span class="event" style="background-color: #b8860b;">Simulacro de Examen de Matemáticas</span>
                  </td>
                  <td>
                    <strong>19</strong>
                  </td>
                  <td>
                    <strong>20</strong>
                  </td>
                  <td>
                    <strong>21</strong>
                  </td>
                </tr>
                <tr>
                  <td>
                    <strong>22</strong><br />
                    <span class="event" style="background-color: #ff8c00;">Entrega de Tareas de Lengua y Literatura</span>
                  </td>
                  <td>
                    <strong>23</strong><br />
                    <span class="event" style="background-color: #b8860b;">Simulacro de Examen de Geografía</span>
                  </td>
                  <td>
                    <strong>24</strong>
                  </td>
                  <td>
                    <strong>25</strong><br />
                    <span class="event" style="background-color: #55bf84;">Taller de Química</span>
                  </td>
                  <td>
                    <strong>26</strong>
                  </td>
                  <td>
                    <strong>27</strong>
                  </td>
                  <td>
                    <strong>28</strong>
                  </td>
                </tr>
                <tr>
                  <td>
                    <strong>29</strong><br />
                    <span class="event" style="background-color: #b8860b;">Simulacro de Examen de Filosofía</span>
                  </td>
                  <td>
                    <strong>30</strong>
                  </td>
                  <td>
                    <strong>31</strong><br />
                    <span class="event" style="background-color: #55bf84;">Taller de Matemáticas</span>
                  </td>
                  <td>
                    <strong>1</strong>
                  </td>
                  <td>
                    <strong>2</strong>
                  </td>
                  <td>
                    <strong>3</strong>
                  </td>
                  <td>
                    <strong>4</strong>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>

      <div class="legend">
        <h5 style="color: #024716;">Leyenda:</h5>
        <div><span style="background-color: #55bf84; width: 15px; height: 15px; display: inline-block;"></span> Talleres</div>
        <div><span style="background-color: #ff8c00; width: 15px; height: 15px; display: inline-block;"></span> Entregas de Tareas</div>
        <div><span style="background-color: #b8860b; width: 15px; height: 15px; display: inline-block;"></span> Simulacros de Exámenes</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.calendar-view {
  padding: 20px;
}
.event {
  display: block;
  margin-top: 5px;
  padding: 5px;
  color: white;
  border-radius: 5px;
}
.legend {
  margin-top: 20px;
}
.legend div {
  margin-bottom: 5px;
}
</style>
