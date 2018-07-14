# Conditional-Accept-Terms-and-Conditions
A Conditional Accept Terms and Conditions Checkbox, if checkbox is selected submit button will enable and if don't checked submit button will disable 

# Here is he code

	<input type="checkbox" id="ctaggery" checked="checked"> 
	<label for="ctaggery">I Accept Terms and Conditions</label>
	<br>

	<button id="ctSubmitbtn" class="ct-register-btn">Register</button>

	<script type="text/javascript">
		$('#ctaggery').change(function(){
		  if($(this).is(":not(:checked)")){
		    $('.ct-register-btn').attr("disabled","disabled");
		  } else if($(this).is(":checked")){
		    $('.ct-register-btn').removeAttr("disabled");
		  }
		});
	</script>
