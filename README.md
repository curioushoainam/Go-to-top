# Go-to-top
#html
<div>
    <button type="button" class="btn btn-info" id="gototop" title="Go to top"><i class="fa fa-angle-up" aria-hidden="true"></i>
    </button>
</div>

#javascript
<script>
	// Go to top
	window.onscroll = function() {scrollFunction()};

	function scrollFunction() {
	    if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
	        document.getElementById("gototop").style.display = "block";
	    } else {
	        document.getElementById("gototop").style.display = "none";
	    }
	}
	
	$("#gototop").click(function() {
	     $("html, body").animate({ scrollTop: 0 }, "slow");
	     return false;
	});
	//  -/- Go to top

</script>

#css
/*Go to top symbol*/
#gototop {
  display: none;
  position: fixed;
  bottom: 20px;
  right: 30px;
  z-index: 99; 
  border: none;
  outline: none;  
  cursor: pointer;  
  border-radius: 50%;
}

#gototop:hover {
  background-color: lightgrey;
}
/* /Go to top symbol*/
