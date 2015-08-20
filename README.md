A jQuery plugin to submit a form asynchronouly without reloading the entire page.
It can be used to submit data to a different domain, which is not possible with AJAX.

examples:
#Example 1 -  Get Request

	$.asyncForm(
		 {
		 	action: 'google.com',
		 	params: {
			 	param1 : value1,
			 	param2 : value2
		 	},
		 	
		 	method:'get',
		 	
		 	onLoadFinished: function(response) {
			 	console.log(response);
		 	}
			 
	});
#Example 2 - Post Request 

	$.asyncForm(
		 {
		 	action:'google.com',
		 	params: {
			 	param1 : value1,
			 	param2 : value2
		 	},
		 	
		 	method:'post',
		 	
		 	onLoadFinished: function(response) {
			 	console.log(response);
		 	}
			 
	});
