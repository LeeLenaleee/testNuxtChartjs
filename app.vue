<template>
  <canvas id="ff"></canvas>
</template>

<script setup lang="ts">
import { Chart, registerables } from "chart.js";

  Chart.register(...registerables);
  new Chart("ff", {
    type: "doughnut",
    data: {
      labels: ["chart", "js"],
      datasets: [
        {
          data: [2, 5],
        },
      ],
    },
  });
</script>