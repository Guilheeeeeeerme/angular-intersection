# angular-intersection

An angular version of Intersection (https://github.com/rook2pawn/node-intersection)


use like this
===============

	var app = angular.module('app',['ngIntersection']);

	app.controller('appController', appController);

	appController.$inject = ["$scope", "$intersection"];

	function appController($scope, $intersection){

		  var seg2 = {start:{x:-1,y:2}, end:{x:5,y:2}};
		  var seg3 = {start:{x:1,y:-1}, end:{x:4,y:4}};

		  $intersection.intersect(seg2,seg3);
		  // {x:2.8,y:2}
	}


There are more methods.
Please check https://github.com/rook2pawn/node-intersection README.md for more information.
