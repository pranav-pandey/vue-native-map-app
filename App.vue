<template>
	<view class="wrapper-view">
		<map-view :initialRegion="initialCoords" class="container">
			<marker :coordinate="initialCoords">
				<callout>
					<view>
						<text class="text-color-primary">Workplace - Geekyants</text>
						<text>The meaning of life is that it stops</text>
					</view>
				</callout>
			</marker>
		</map-view>
		<view class="box-style">
				<text>
					Hey yo wazaaaap
				</text>
			</view>
	</view>
</template>
 <script>
import MapView, { Marker, Callout } from 'react-native-maps';
export default {
	data: function() {
		return {
			initialCoords: {
				latitude: 12.9107,
				longitude: 77.6018,
				latitudeDelta: 0.0122,
				longitudeDelta: 0.0221,
			},
		};
	},
	components: { MapView, Marker, Callout },
};
</script>
 
<style>
.container {
	position: absolute;
	top: 0;
	left: 0;
	right: 0;
	bottom: 0;
	/* background-color: white;
	align-items: center;
	justify-content: center;
	flex: 1; */
}
.wrapper-view {
	position: absolute;
	top: 0;
	left: 0;
	right: 0;
	bottom: 0;
}
.text-color-primary {
	color: blue;
	align-self: center;
	margin: auto;
}
.box-style {
	height: 200;
	position: absolute;
	bottom: 0;
	left: 0;
	right: 0;
	background-color: aqua;
	align-self: center;
	align-items: center;
	justify-content: center;
	margin: 10;
}
</style>
