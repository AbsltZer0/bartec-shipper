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
						data: [12, 19, 3],
						backgroundColor: [
							'rgba(255, 99, 132, 0.2)',
							'rgba(54, 162, 235, 0.2)',
							'rgba(255, 206, 86, 0.2)'
						],
						borderColor: [
							'rgba(255, 99, 132, 1)',
							'rgba(54, 162, 235, 1)',
							'rgba(255, 206, 86, 1)'
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
