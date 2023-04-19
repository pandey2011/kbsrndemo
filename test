<html>
<head>

</head>

<body>

<script>

var nums = [4,3,2,1,6,8,0,9];

function doIt() {
	var after = mergeSort( nums );
	document.writeln(after);
}

function mergeSort(arr) {
	var left, right;
	if(arr.length() > 1) {
		var middle = Math.floor( arr.length / 2 );
		left = mergeSort( arr.splice(0, middle) );
		right = mergeSort( arr );
	} else  {
		return arr;
	}
	merge(left, right);
}

function merge( left, right ) {
	var num = left.length + right.length;
	var leftPoint = 0, rightPoint = 0;
	var result = [];
	while( leftPoint < left.length && rightPoint < right.length  ) {
		if(leftPoint >= left.length) {
			result.push( right[rightPoint] )
			rightPoint++;
		} else if( rightPoint >= right.length ) {
			result.push( left[leftPoint] );
			leftPoint++;
		} else {
			if( left[leftPoint] < right[rightPoint] ) {
				result.push( left[leftPoint] );
				leftPoint++;
			} else {
				result.push( right[rightPoint] );
				rightPoint++;
			}
		}
		
	}
}

</script>

<a href='#' onclick='doIt()'>test</a>

</body>

</html>
