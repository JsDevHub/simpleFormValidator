# Simple Form Validator


Simple html form validator with minimal configurations.

   1. Change the colors of error messages.
   2. easy and simple html attributes to perform vaidations.


Sample Example : 
&lt;html&gt;
&lt;head&gt;
&lt;title&gt;Sample SFV&lt;/title&gt;
&lt;script src=&quot;https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js&quot;&gt;&lt;/script&gt;
&lt;script src=&quot;sf-validator-0.1.js&quot;&gt;&lt;/script&gt;
&lt;script&gt;
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
&lt;/script&gt;
&lt;/head&gt;
&lt;body&gt;

   &lt;form id=&quot;check&quot; &gt;
       &lt;input type='text' name='name' class='form-fields' req='true'  msg='This filed is required' len='20' &gt;
       &lt;input type='submit' value='submit' &gt;
  &lt;/form&gt;

&lt;/body&gt;
&lt;/html&gt;



