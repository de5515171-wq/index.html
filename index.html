<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Histograma de Cosecha - Camaronera</title>
    <!-- Librería para gráficos compatible con web móvil -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 15px;
            background: #f4f7f6;
            color: #333;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        h2 {
            color: #0284c7;
            text-align: center;
            font-size: 1.2rem;
            margin-bottom: 15px;
        }
        canvas {
            width: 100% !important;
            height: auto !important;
            max-height: 300px;
        }
        .stats {
            margin-top: 15px;
            font-size: 0.9rem;
            background: #f0f9ff;
            padding: 12px;
            border-radius: 5px;
            border-left: 4px solid #0284c7;
        }
    </style>
</head>
<body>

    <div class="container">
        <h2>Histograma de Cosecha (Camarón)</h2>
        <canvas id="histogramChart"></canvas>
        <div class="stats" id="statsContainer">
            <!-- Los datos calculados aparecerán aquí -->
        </div>
    </div>

    <script>
        // 1. Tus datos de campo (pesos en gramos de los camarones muestreados)
        const pesosCamarones = [
            5.2, 6.1, 6.8, 7.1, 7.5, 7.8, 8.0, 8.2, 8.5, 8.8,
            9.0, 9.1, 9.3, 9.5, 9.8, 10.1, 10.5, 11.0, 11.5, 12.2,
            6.5, 7.2, 8.1, 8.6, 9.2, 9.6, 10.0, 10.3, 11.1, 12.0
        ];

        // 2. Configuración de intervalos (bins)
        const minPeso = 4.0;
        const maxPeso = 14.0;
        const amplitud = 1.5;

        let bins = [];
        for (let i = minPeso; i < maxPeso; i += amplitud) {
            bins.push({ 
                min: i, 
                max: i + amplitud, 
                count: 0, 
                label: `${i.toFixed(1)} - ${(i + amplitud).toFixed(1)}g` 
            });
        }

        // Distribuir los datos en los intervalos correspondientes
        pesosCamarones.forEach(peso => {
            for (let bin of bins) {
                if (peso >= bin.min && peso < bin.max) {
                    bin.count++;
                    break;
                }
            }
        });

        const labels = bins.map(b => b.label);
        const dataCounts = bins.map(b => b.count);

        // Calcular promedio de la muestra
        const suma = pesosCamarones.reduce((a, b) => a + b, 0);
        const promedio = (suma / pesosCamarones.length).toFixed(2);

        // Mostrar estadísticas en pantalla
        document.getElementById('statsContainer').innerHTML = `
            <b>Total Muestreado:</b> ${pesosCamarones.length} camarones<br>
            <b>Peso Promedio:</b> ${promedio} g
        `;

        // 3. Renderizar el gráfico de barras (histograma)
        const ctx = document.getElementById('histogramChart').getContext('2d');
        new Chart(ctx, {
            type: 'bar',
            data: {
                labels: labels,
                datasets: [{
                    label: 'Frecuencia (Individuos)',
                    data: dataCounts,
                    backgroundColor: 'rgba(31, 119, 180, 0.75)',
                    borderColor: 'rgba(31, 119, 180, 1)',
                    borderWidth: 1,
                    barPercentage: 1.0,     // Barras juntas simulando histograma continuo
                    categoryPercentage: 1.0
                }]
            },
            options: {
                responsive: true,
                plugins: {
                    legend: { display: false }
                },
                scales: {
                    x: { 
                        title: { display: true, text: 'Intervalos de Peso (g)' },
                        grid: { display: false }
                    },
                    y: { 
                        title: { display: true, text: 'Número de Camarones' }, 
                        beginAtZero: true 
                    }
                }
            }
        });
    </script>
</body>
</html>
