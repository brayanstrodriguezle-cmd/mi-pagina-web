<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Día del Ingeniero en Colombia y el Mundo</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.6;
      background-color: #f4f4f4;
    }

    header, footer {
      background-color: #004080;
      color: white;
      padding: 1rem 2rem;
      text-align: center;
    }

    section {
      padding: 2rem;
      margin: 1rem auto;
      background-color: white;
      max-width: 900px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h1, h2 {
      color: #003366;
    }

    ul {
      list-style: square;
      padding-left: 1.5rem;
    }

    article {
      margin-bottom: 1.5rem;
    }

    .compare-box {
      margin-top: 2rem;
      padding: 1rem;
      background: #eef;
      border-left: 5px solid #004080;
      border-radius: 5px;
    }

    label {
      font-weight: bold;
    }

    select {
      margin: 0.5rem 0;
      padding: 0.5rem;
      font-size: 1rem;
    }

    #result {
      margin-top: 1rem;
      font-style: italic;
      color: #333;
    }
  </style>
</head>
<body>
  <header>
    <h1>Día del Ingeniero en Colombia y el Mundo</h1>
  </header>

  <section id="introduccion">
    <h2>Introducción</h2>
    <p>El Día del Ingeniero se celebra en diferentes fechas según el país. Esta página explora la historia y controversia sobre su celebración en Colombia y cómo se compara con otros países.</p>
  </section>

  <section id="colombia">
    <h2>Colombia</h2>

    <article id="fecha-popular">
      <h3>17 de agosto – Fecha popular</h3>
      <p>En Colombia, muchas personas celebran el Día del Ingeniero el 17 de agosto, aunque esta fecha no es oficial. Se ha vuelto común en redes sociales y en instituciones educativas.</p>
    </article>

    <article id="fecha-oficial">
      <h3>29 de mayo – Fecha oficial (SCI)</h3>
      <p>La Sociedad Colombiana de Ingenieros (SCI) celebra oficialmente el Día del Ingeniero el 29 de mayo, fecha de su fundación en 1887. Esta es la fecha reconocida institucionalmente.</p>
    </article>

    <article id="conclusion-colombia">
      <h3>Conclusión</h3>
      <p>La coexistencia de ambas fechas refleja la diferencia entre celebraciones sociales y gremiales. Ninguna es inválida, pero la oficial es la del 29 de mayo según la SCI.</p>
    </article>
  </section>

  <section id="otros-paises">
    <h2>Celebración en otros países</h2>
    <ul>
      <li><strong>Uruguay:</strong> 12 de octubre – primera colación de ingenieros (1892).</li>
      <li><strong>Bolivia:</strong> 5 de octubre – fundación de la Sociedad de Ingenieros (1922).</li>
      <li><strong>Argentina:</strong> 6 de junio (Día de la Ingeniería) y 16 de junio (Día del Ingeniero).</li>
      <li><strong>India:</strong> 15 de septiembre – en honor a M. Visvesvaraya.</li>
      <li><strong>México:</strong> 1 de julio.</li>
      <li><strong>Perú:</strong> 8 de junio.</li>
    </ul>
  </section>

  <section class="compare-box">
    <h2>Consulta el Día del Ingeniero en tu país</h2>
    <label for="pais">Selecciona un país:</label>
    <select id="pais">
      <option value="">-- Selecciona --</option>
      <option value="colombia">Colombia</option>
      <option value="argentina">Argentina</option>
      <option value="uruguay">Uruguay</option>
      <option value="bolivia">Bolivia</option>
      <option value="india">India</option>
      <option value="mexico">México</option>
      <option value="peru">Perú</option>
    </select>
    <div id="result"></div>
  </section>

  <footer>
    <p>Autor: [BRAYAN STEVEN RODRIGUEZ LEAL]. Proyecto académico sobre HTML semántico. Agosto 2025.</p>
  </footer>

  <script>
    const fechas = {
      colombia: "29 de mayo (oficial - Sociedad Colombiana de Ingenieros) y 17 de agosto (celebración popular)",
      argentina: "6 de junio (Día de la Ingeniería) y 16 de junio (Día del Ingeniero)",
      uruguay: "12 de octubre (primera colación de ingenieros)",
      bolivia: "5 de octubre (fundación de la Sociedad de Ingenieros)",
      india: "15 de septiembre (en honor a M. Visvesvaraya)",
      mexico: "1 de julio",
      peru: "8 de junio"
    };

    document.getElementById("pais").addEventListener("change", function() {
      const paisSeleccionado = this.value;
      const resultado = fechas[paisSeleccionado] || "Selecciona un país para ver la fecha.";
      document.getElementById("result").textContent = resultado;
    });
  </script>
</body>
</html>

