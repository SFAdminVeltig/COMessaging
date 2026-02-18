<html>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			
		window.addEventListener("onEmbeddedMessagingReady", () => {            
			console.log( "Inside Prechat API!!" );
			embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( {'QueueName' : 'Country Outfitters Messaging' } );
			});
			embeddedservice_bootstrap.init(
				'00DOt000002m0EL',
				'Country_Outfitters_Messaging',
				'https://bootbarn--uat.sandbox.my.site.com/ESWCountryOutfittersMes1770066167469',
				{
					scrt2URL: 'https://bootbarn--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://bootbarn--uat.sandbox.my.site.com/ESWCountryOutfittersMes1770066167469/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
</html>
