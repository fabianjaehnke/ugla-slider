UGLA-Slider
===========

using animate() but shall be animated using css-transforms

**DEMO**<br>
<a href="http://ugla-media.vs188017.vserver.de/projekte/">DEMO 1</a><br>
<a href="http://povmedia.de">DEMO 2</a>



Usage:
You need a wrapper called "projects" and put your contents each in a "container"
<code>
	`<div>`<br>
		`<div id="projects">`<br>
			`<div class="container">`<br>
			   `Content Page 1`<br>
			`</div>`<br>
			`<div class="container">`<br>
				`Content Page 2`<br>
			`</div>`<br>
			`<div class="container">`<br>
				`Content Page 3`<br>
			`</div>`<br>
			`<div class="container">`<br>
				`Content Page 4`<br>
			`</div>`<br>
		`</div>`<br>
	`</div>`<br>
	`<div id="slider" style="left:0;"><a class="left" href="#">left</a><a class="right" href="#">right</a></div>`<br>
</code>

Call uglaSlide() on the wrapper "projects" and pass the configuration object

<code>
	$(document).ready(function(){<br>
		$("#projects").uglaSlide({<br>
			'left': $("#slider .left"), //the jQuery Object of the left-link to be clicked<br>
			'right': $("#slider .right"), //the jQuery Object of the right-link to be clicked<br>
			'menu': $('#projectssubmenu li a') //not implmented yet... for navigation menu<br>
		});<br>
	});<br>
</code>

Contents:
*	ugla-slider.js
*	index.html
