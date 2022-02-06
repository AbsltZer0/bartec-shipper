<section class=" w-full h-screen  pt-20  pl-20 bg-gray-900">
	<div class="flex flex-col w-60">
		<label class="text-orange-100" for="make">Make:</label>
		<select
			name="make"
			onchange="form_changed=true;reloadElement('ajax_functions.php?page=newCall2&amp;div=modeldiv&amp;make='+this.value,'modeldiv')"
		>
			<option value="" selected="" />
			<option value="51" />
			<option value="1">Acura</option>
			<option value="44">Aftermarket Kit</option>
			<option value="54">Alfa Romeo</option>
			<option value="65">Alpina</option>
			<option value="47">Aston Martin</option>
			<option value="2">Audi</option>
			<option value="45">Bentley</option>
			<option value="3">BMW</option>
			<option value="4">BMW Cycle</option>
			<option value="62">Bugatti</option>
			<option value="5">Buick</option>
			<option value="6">Cadillac</option>
			<option value="7">Chevrolet</option>
			<option value="8">Chrysler</option>
			<option value="9">Dodge</option>
			<option value="49">Ferrari</option>
			<option value="48">Fiat</option>
			<option value="10">Ford</option>
			<option value="55">Freightliner</option>
			<option value="56">Genesis</option>
			<option value="11">GMC</option>
			<option value="12">Honda</option>
			<option value="13">Honda Cycle</option>
			<option value="14">Hummer</option>
			<option value="15">Hyundai</option>
			<option value="16">Infiniti</option>
			<option value="17">Isuzu</option>
			<option value="18">Jaguar</option>
			<option value="19">Jeep</option>
			<option value="20">Kia</option>
			<option value="63">KTM Motorcycles</option>
			<option value="57">Lamborghini</option>
			<option value="21">Land Rover</option>
			<option value="22">Lexus</option>
			<option value="23">Lincoln</option>
			<option value="24">Lotus</option>
			<option value="25">Maserati</option>
			<option value="26">Maybach</option>
			<option value="27">Mazda</option>
			<option value="58">McLaren</option>
			<option value="28">Mercedes-Benz</option>
			<option value="64">Mercedes-Benz AMG</option>
			<option value="29">Mercury</option>
			<option value="30">Mini</option>
			<option value="31">Mitsubishi</option>
			<option value="32">Nissan</option>
			<option value="46">Oldsmobile</option>
			<option value="59">Plymouth</option>
			<option value="66">Polestar</option>
			<option value="33">Pontiac</option>
			<option value="34">Porsche</option>
			<option value="52">RAM</option>
			<option value="60">Retrofit</option>
			<option value="67">Rivian</option>
			<option value="50">Rolls Royce</option>
			<option value="35">Saab</option>
			<option value="36">Saturn</option>
			<option value="37">Scion</option>
			<option value="38">Smart</option>
			<option value="39">Subaru</option>
			<option value="40">Suzuki</option>
			<option value="53">Tesla</option>
			<option value="41">Toyota</option>
			<option value="42">Volkswagen</option>
			<option value="43">Volvo</option>
			<option value="61">VPG</option>
		</select>
	</div>
	<div class="flex flex-col w-60">
		<label class="text-orange-100" for="Model">Model:</label>
		<select
			name="model"
			onchange="form_changed=true;reloadElement('ajax_functions.php?page=newCall2&amp;div=yeardiv&amp;model='+this.value,'yeardiv,wadiv')"
		>
			<option value="" selected="" />
		</select>
	</div>
	<div class="flex flex-col w-60">
		<label class="text-orange-100" for="year">Year:</label>
		<select name="year" onchange="form_changed=true;" />
	</div>
</section>
