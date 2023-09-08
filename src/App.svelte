<script>
	let isPressed = false;
	let pos = {x: 0, y: 0};

  function handleMouseDown(event) {
		isPressed = true;
  }
	function handleMouseMove(event) {
		if (isPressed == true) {
			pos.x = event.clientX - 37;
		  pos.y = event.clientY - 37;
		}
	}
  function handleMouseUp() {
    isPressed = false;
  }
</script>

{@html '<!-- Container for the draggable rectangle -->'}
<div
	class = "box"
	role="presentation"
	style="width: 50px; 
				 height: 50px;
				 background-color: #000000;
				 position: relative;
				 top:{pos.y}px;
				 left:{pos.x}px"
	on:mousedown={handleMouseDown}
	on:mousemove={handleMouseMove}
	on:mouseup={handleMouseUp}
></div>
{@html '<!-- Print the coordinates of the rectangle -->'}
x: {pos.x}; y: {pos.y}

