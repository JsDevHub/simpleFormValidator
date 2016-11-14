# Simple Form Validator


Simple html form validator with minimal configurations.

   1. Change the colors of error messages.
   2. easy and simple html attributes to perform vaidations.


Sample Example : 


Simple Validator Code:

      SimpleFormValidator.validate({
     
           formId  : 'check',
           successHandler : function(){
                  alert('success');
           },
           errorHandler : {
               errorBgColor : 'pink',
               errorMsgColor : 'yellow'
            } 

       });
  
 
 
HTML Code;

  &lt;form id=&quot;check&quot; &gt;
  
   &lt;input type='text' name='name' class='form-fields' req='true'  msg='This filed is required' len='20' &gt;
 
   &lt;input type='submit' value='submit' &gt;


