
<!DOCTYPE HTML>
<html>
	<head>
		<title>Demo #1 - jquery.touch.js</title>
		<meta http-equiv="content-type" content="text/html; charset=utf-8" />
		<script src="http://code.jquery.com/jquery-1.11.1.min.js"></script>
		<script src="../jquery.dropotron.js"></script>
		<style>
		
			body { font-family: sans-serif; font-size: 12pt; color: #444; line-height: 1.5em; } 
			h1 { font-size: 1.5em; } 
			#wrapper { max-width: 600px; margin: 0 auto; text-align: center; } 
			#main-nav ul { list-style: none; margin: 0; padding: 0; }
			#main-nav ul li { display: inline-block; margin: 0 1em 0 1em; padding: 0.35em 0.75em 0.35em 0.75em; border-radius: 0.5em; }
			#main-nav ul li.active { background: #999; }
			#main-nav ul li.active a { color: #fff; text-decoration: none; }
		
			/* A single menu */
			.dropotron { background: #444; border-radius: 0.5em; list-style: none; margin: 0; min-width: 10em; padding: 0.75em 1em 0.75em 1em; }
			.dropotron > li { border-top: solid 1px #555; margin: 0; padding: 0; }
			.dropotron > li:first-child { border-top: 0; }
			.dropotron > li > a { color: #ccc; display: block; padding: 0.5em 0 0.5em 0; text-decoration: none; }
			.dropotron > li.active > a, .dropotron > li:hover > a { color: #fff; }
			
			/* Only applies to top level ("level-0") menus */
			.dropotron.level-0 { margin-top: 1.25em; }
			.dropotron.level-0:before { content: ''; position: absolute; border-bottom: solid 0.5em #444; border-left: solid 0.5em transparent; border-right: solid 0.5em transparent; top: -0.5em; }
		
		</style>
		<script>
			$(function() {
				
				// Note: make sure you call dropotron on the top level <ul>
				$('#main-nav > ul').dropotron({ 
					offsetY: -10 // Nudge up submenus by 10px to account for padding
				});
			
			});
		</script>
	</head>
	<body>
		<div id="wrapper">
			<h1>Demo #1</h1>
			<nav id="main-nav">
				<ul>
					<li><a href="/">Home</a></li>
					<li>
						<!--
							
							Links with submenus can point to actual URLs:
							
								<a href="/skills">Skills</a>
							
							or just a "#":
							
								<a href="#">Skills</a>							
							
						-->
						<a href="#">Skills</a>
						<ul>
							<li><a href="/skills/nunchuks">Nunchuks</a></li>
							<li><a href="/skills/bow-hunting">Bow Hunting</a></li>
							<li><a href="/skills/computer-hacking">Computer Hacking</a></li>
							<li><a href="/skills/disco">Disco</a></li>
						</ul>
					</li>
					<li>
						<a href="#">Enemies</a>
						<ul>
							<li><a href="/enemies/don">Don</a></li>
							<li><a href="/enemies/uncle-rico">Uncle Rico</a></li>
							<li>
								<a href="#">Rogue AIs ...</a>
								<ul>
									<li><a href="/enemies/rogue-ais/shodan">SHODAN</a></li>
									<li><a href="/enemies/rogue-ais/wintermute">Wintermute</a></li>
									<li><a href="/enemies/rogue-ais/neuromancer">Neuromancer</a></li>
									<li><a href="/enemies/rogue-ais/deus">Deus</a></li>
									<li><a href="/enemies/rogue-ais/megaera">Megaera</a></li>
								</ul>
							</li>
							<li><a href="/enemies/chickens">Chickens</a></li>
						</ul>
					</li>
					<li><a href="/art">Art</a></li>
					<li><a href="/contact">Contact</a></li>
				</ul>
			</nav>
			<p>
				Amet non nec donec nisi aenean malesuada. Tincidunt fermentum orci adipiscing morbi ac nec curae auctor vivamus imperdiet blandit pretium. Feugiat nascetur nisi eleifend nunc nisl etiam duis curae malesuada scelerisque dignissim rhoncus. Placerat lobortis amet volutpat blandit auctor mollis condimentum. Porttitor dictum nunc arcu est fermentum sapien sociis parturient fusce lacus tincidunt.
			</p>
		</div>
	</body>
</html>
