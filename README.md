# SwipeControls
------------------------
SwipeControls.js is a script that enables click-and-drag controls in three.js scenes.
This is similar to the touch-and-drag controls on mobile devices with touch screens.

SwipeControls is easy to use:

1.) "import" three.js library
<script src="js/three.js"></script>

2.) "import" SwipeControls.js
<script src="js/SwipeControls.js"></script>

3.) instantiate SwipeControls object ( pass cmaera object )
var controls = new THREE.SwipeControls( camera );

4.) update controls in animate function

function animate() {

	requestAnimationFrame( animate );

	// other things you do..

	controls.update();
	
	render();

}

You can adjust the speed of the swipe with: controls.speed = some_number;
You can adjust the buffer speed of swipe after release with: controls.swipeBuffer = some_number_between_0_and_1;