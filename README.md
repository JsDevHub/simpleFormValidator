# Simple Form Validator


Simple html form validator with minimal configurations.

   1. Change the colors of error messages.
   2. easy and simple html attributes to perform vaidations.


Sample Example : 

<html>
<head>
<title>Sample SFV</title>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="sf-validator-0.1.js"></script>
<script>
$(document).ready(function(){
  
  SimpleFormValidator.validate({
        formId : 'check'
        successHandler : function(){
               alert('success');
        },
        errorHandler : {
            errorBgColor : 'red',
            errorMsgColor : 'orange'
         } 

  })
});
</script>
</head>
<body>

   <form id="check" >
       <input type='text' name='name' class='form-fields' req='true'  msg='This filed is required' len='20' >
       <input type='submit' value='submit' >
  </form>

</body>
</html>



