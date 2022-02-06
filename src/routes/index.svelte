<script>
	import '../app.css';
	import Chart from '../components/chart.svelte';
	import WeekCalls from '../components/weeklyCalls.svelte';
	import ThirtyDayCalls from '../components/30DayCalls.svelte';
	import RMAChart from '../components/RMAChart.svelte';
</script>

<section class="bg-gray-900 flex flex-col w-screen h-full">
	<div class="flex flex-row w-9/12 justify-between m-10">
		<div
			class="flex flex-col justify-between w-80 h-full rounded-md m-3 p-2 text-white bg-gray-700 bg-opacity-40 text-center place-items-center res"
		>
			<Chart />
			<a href="/">
				<p>TODAY</p>
			</a>
		</div>
		<div
			class="flex flex-col justify-between w-80 h-full rounded-md m-3 p-2 text-white bg-gray-700 bg-opacity-40 text-center place-items-center"
		>
			<WeekCalls />
			<a href="/">
				<p>THIS WEEK</p>
			</a>
		</div>
		<div
			class="flex flex-col justify-between w-80 h-full rounded-md m-3 p-2 text-white bg-gray-700 bg-opacity-40 text-center place-items-center max-h-full"
		>
			<ThirtyDayCalls />
			<a href="/">
				<p>PAST 30 DAYS</p>
			</a>
		</div>
	</div>
	<div class="flex flex-row w-9/12 justify-center m-10">
		<div
			class="flex flex-row justify-around w-full h-80 rounded-md m-3 p-2 text-white bg-gray-700 bg-opacity-40 text-center align-middle place-items-center"
		>
			<RMAChart />
		</div>
	</div>
	<div class="flex flex-row w-9/12 justify-between m-10">
		<div
			class="flex flex-col justify-between w-full h-full rounded-md m-3 p-2 text-white bg-gray-700 bg-opacity-40 text-center place-items-center"
		>
			<Chart />
			<a href="/">
				<p>TODAY</p>
			</a>
		</div>
		<div
			class="flex flex-col justify-between w-full h-full rounded-md m-3 p-2 text-white bg-gray-700 bg-opacity-40 text-center place-items-center"
		>
			<Chart />
			<a href="/">
				<p>TODAY</p>
			</a>
		</div>
	</div>
</section>
