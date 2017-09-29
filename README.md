<DOCTYPE html>
<html>
	  <head>
			  <script src="prime.js">
			  </script>
	  </head>
	  <body>
        <input type="number" id="n1"/><span id="s1"  ></span>
        <br><br>
        <input type="button" value="ok" onclick="prime()"/>
		
	  </body>
</html>	
	
	
		



function prime()
{	
    var n=document.getElementById('n1').value;
    if(n==1 || n<=0)
	  {
        //alert(n+" "+"is not a prime number");
        document.getElementById('s1').innerHTML=" "+n+" "+"is not a Prime number";
        return false;
	  }
	    else if(n==2)
	    {
         //alert(n+" "+"is a prime number");
         document.getElementById('s1').innerHTML=" "+n+" "+"is a Prime number";
         return false
	    }
	        else
	        {
		         for(var x=2;x<n;x++)
		         {
			          if(n%x==0)
			           {
                      //alert(n+" "+"is not a prime number");
                      document.getElementById('s1').innerHTML=" "+n+" "+"is not a Prime number";
                      return false;
			            }
			                else
			                {
				                   continue;
				
			                 }
			
	            }
        //alert(n+" "+"is a prime number");
        document.getElementById('s1').innerHTML=" "+n+" "+"is a Prime number";
          }
		
}
