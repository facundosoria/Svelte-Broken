<script lang="ts">
	let numero = [1 ,2 ,3 ,4 ,5];

	function addNumero() {
		numero =[...numero , numero.length+1];
	}

	$: suma= numero.reduce((a ,b) => a + b ,0);

  </script>

  <p>{numero.join(" * ")} = {suma}</p>
  <button on:click={addNumero}>Poner 1 numero mas</button>






	
 