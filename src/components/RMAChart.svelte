<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	let ctx;

	onMount(async () => {
		const myChart = new Chart(ctx, {
			type: 'line',
			data: {
				labels: [
					'1',
					'2',
					'3',
					'4',
					'5',
					'6',
					'7',
					'8',
					'9',
					'10',
					'11',
					'12',
					'13',
					'14',
					'15',
					'16',
					'17',
					'18',
					'19',
					'20',
					'21',
					'22',
					'23',
					'24',
					'25',
					'26',
					'27',
					'28',
					'29',
					'30'
				],
				datasets: [
					{
						label: 'RMAs Issued Last 30 Days',
						data: [
							12, 19, 3, 5, 2, 3, 20, 5, 7, 10, 12, 19, 3, 5, 2, 3, 20, 5, 7, 10, 12, 19, 3, 5, 2,
							3, 20, 5, 7, 10
						],
						backgroundColor: ['rgba(153, 102, 255, 0.2)'],
						borderColor: ['rgba(153, 102, 255, 1)'],
						borderWidth: 3
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

<canvas id="myChart" width="400" height="100" bind:this={ctx} />
