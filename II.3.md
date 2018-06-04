<!DOCTYPE html>
<html>
	<head>
        <meta charset="utf-8" />
        <title>LeBitcoin</title>
		<style>
			img 
			{
			border: solid 8px green      <!-- Traitement de la partie II.2  -->
			}
		</style
	</head>
	<body>
		<h1> LeBitcoin </h1> 
		<img src=https://courscryptomonnaies.ams3.digitaloceanspaces.com/contents-assets/BTC%201.png />
		<a href="https://courscryptomonnaies.com/bitcoin" >Lien vers le site </a>
		<!-- J'ai utilisé le moteur de recherche google avec le mot-clé "bitcoin" pour trouver cette image -->
	
		<form id="myForm" method="post" >																<!-- formulaire avec notes de 0 à 5 --->
			<p> Quel note attribueriezez vous à ce site ?</p>											<!-- II.3 traitée -->
			<label><input type="radio" name="check" value="0" />  0</label><br />
			<label><input type="radio" name="check" value="1" />  1</label><br />
			<label><input type="radio" name="check" value="2" />  2</label><br />
			<label><input type="radio" name="check" value="3" />  3</label><br />
			<label><input type="radio" name="check" value="4" />  4</label><br />
			<label><input type="radio" name="check" value="5" />  5</label><br  />
			
		</form>
		<script>
			function check() {																			<!-- Vérification des données  --->
				var inputs = document.getElementByTagName('input')
				inputsLength = inputs.length;
				var myForm = document.getElementById('myForm');
				var j=0;
				for (var i=0; i < 6; i++) {
					if(inputs[i].type === 'radio' && inputs[i].checked) {
						var j++;
					}
				if  (j===1){
					myForm.submit();
				else {
					alert ('Une erreur est survenue lors de l''enregistrement de votre note')}
		myForm.check();		
		</script>	
		
	</body>
</html>
