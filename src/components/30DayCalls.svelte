<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	let ctx;

	onMount(async () => {
		const myChart = new Chart(ctx, {
			type: 'bar',
			data: {
				labels: ['DT', 'Walmart', 'TS'],
				datasets: [
					{
						label: 'Total Calls',
						data: [122, 205, 120],
						backgroundColor: [
							'rgba(54, 162, 235, 0.2)',

							'rgba(75, 192, 192, 0.2)',

							'rgba(255, 159, 64, 0.2)'
						],
						borderColor: [
							'rgba(54, 162, 235, 1)',

							'rgba(75, 192, 192, 1)',

							'rgba(255, 159, 64, 1)'
						],
						borderWidth: 2
					}
				]
			},
			options: {
				scales: {
					y: {
						beginAtZero: true
					}
				}
			}
		});
	});
</script>

<canvas id="myChart" width="400" height="400" bind:this={ctx} />
