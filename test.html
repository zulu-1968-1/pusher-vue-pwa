<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
	pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<link href="css/font-awesome.min.css" rel="stylesheet">
<script type='text/javascript' src='js/vue.js'></script>
<style>
/*
				Default ScreenItem
			*/
.screenItemWarningHighLight {
	background-color: rgba(255, 130, 0, 0.6);
}

.screenItemWarningHighLight p {
	color: rgb(255, 255, 255) !important;
}

.screenItemDangerHighLight {
	background-color: rgba(255, 0, 0, 0.6);
}

.screenItemDangerHighLight p {
	color: rgb(255, 255, 255) !important;
}

.screenItemDefault {
	border: 1px solid rgb(0, 0, 90);
}

.screenItemDefault p {
	color: rgb(0, 0, 90);
}

.screenItemDefault span {
	border: 1px solid rgb(0, 0, 90);
	background-color: rgba(0, 0, 90, 0.6);
	color: rgb(255, 255, 255);
}

/*
				Info ScreenItem
			*/
.screenItemInfo {
	border: 1px solid rgb(0, 153, 255);
}

.screenItemInfo p {
	color: rgb(0, 153, 255);
}

.screenItemInfo span {
	border: 1px solid rgb(0, 153, 255);
	background-color: rgba(0, 153, 255, 0.6);
	color: rgb(255, 255, 255);
}

/*
				Success ScreenItem
			*/
.screenItemSuccess {
	border: 1px solid rgb(0, 154, 68);
}

.screenItemSuccess p {
	color: rgb(0, 154, 68);
}

.screenItemSuccess span {
	background-color: rgba(0, 154, 68, 0.6);
	border: 1px solid rgb(0, 154, 68);
	color: rgb(255, 255, 255);
}
/*
				Warning ScreenItem
			*/
.screenItemWarning {
	border: 1px solid rgb(255, 130, 0);
}

.screenItemWarning p {
	color: rgb(255, 130, 0);
}

.screenItemWarning span {
	background-color: rgba(255, 130, 0, 0.6);
	border: 1px solid rgb(255, 130, 0);
	color: rgb(255, 255, 255);
}

/*
				Danger ScreenItem
			*/
.screenItemDanger {
	border: 1px solid rgb(255, 0, 0);
}

.screenItemDanger p {
	color: rgb(255, 0, 0);
}

.screenItemDanger span {
	background-color: rgba(255, 0, 0, 0.6);
	border: 1px solid rgb(255, 0, 0);
	color: rgb(255, 255, 255);
}

/*
				ScreenItem
			*/
.screenItem { -
	-width: 120px; -
	-height: 50px;
	padding: 2px;
	float: left;
	margin: 0 10px 10px 0;
	border-radius: 5px;
	position: absolute; -
	-z-index: 1;
	font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}

.screenItem p {
	margin: 0; -
	-background-color: transparent;
	text-align: center;
	font-size: .8em;
}

.screenItem span {
	margin: 0;
	border-radius: 5px;
	text-align: left;
	font-size: .8em;
	font-weight: bold;
	position: absolute;
	width: 100%;
	bottom: -1px;
	left: -1px;
}

/*
	Screen Area
*/
.screen {
	min-height: 500px;
	border: 1px solid #404040;
}

/* context menu */
.context-menu {
	display: none;
	position: absolute;
	z-index: 10;
	padding: 0px;
	width: 180px;
	background-color: #fff;
	border: solid 1px #dfdfdf;
	box-shadow: 1px 1px 2px #cfcfcf;
	font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
	font-size: 0.8em;
}

.context-menu--active {
	display: block;
}

.context-menu__items {
	list-style: none;
	margin: 0;
	padding: 0;
}

.context-menu__item {
	display: block;
	margin-bottom: 4px;
}

.context-menu_hr {
	border-top: 1px solid gray;
	padding-top: 4px;
}

.context-menu__header {
	display: block;
	margin-bottom: 4px;
	padding:3px;
	font-size: 1.0em;
	border-bottom: 1px solid gray;
	
}

.context-menu__item:last-child {
	margin-bottom: 0;
}

.context-menu__link {
	display: block;
	padding: 2px 4px;
	color: #0066aa;
	text-decoration: none;
}

.context-menu__link:hover {
	color: #fff;
	background-color: #0066aa;
}

.screenItemButtons{
	position: absolute;
	top: 10px;
	left: 10px;
	z-index: 10;
}
</style>
</head>

<body>
	<div id="vueApp" class="screen" v-on:click="bodyClickListener" v-on:contextmenu="contextClick" data-ctxmenu="screen-context-menu" data-text="Process Screen">
		<div data-ctxmenu="screen-item-context-menu" v-for="item in screenItems" 
			v-bind:data-link="arrayToCvs(item.parent)" 
			v-bind:data-text="item.title"  
			v-bind:class="['screenItem ' + (item.type == 1 ? 'screenItemSuccess' : item.type == 2 ? 'screenItemWarning' : item.type == 3 ? 'screenItemDanger' : item.type == 4 ? 'screenItemInfo' : 'screenItemDefault')]"
			v-on:mousedown="mouseDown" 
			v-on:click="mouseClick"
			v-on:drop="dropEvent" 
			v-on:dragenter="holdEvent" 
			v-on:dragover="holdEvent" 
			v-on:dragleave="holdEvent" 
			v-bind:id="item.id" 
			v-bind:style="'left:' + item.left + 'px;top:' + item.top + 'px;width:' + item.width + 'px;height:' + item.height + 'px'">
			<div v-bind:data-id="item.id" class="screenItemButtons" v-if="editMode" v-bind:draggable="editMode" title="Drag me to a screen item." xv-on:click="holdEvent" xv-on:mousedown="holdEvent" v-on:dragstart="dragStartEvent" v-on:drag="holdEvent"><i class="fa fa-share-alt-square"></i></div>
			<p>{{item.title}}</p>
			<span>&nbsp;{{item.subTitle}}</span>
		</div>

		<nav id="screen-item-context-menu" v-bind:class="'context-menu ' + (screenItemCtxMenuState == 1 ? 'context-menu--active' : '')">
			<ul class="context-menu__items">
				<!-- Menu Items -->
				<li class="context-menu__header"><b>{{screenItemInContext!=null?screenItemInContext.getAttribute('data-text'):""}}</b></li>
				<li class="context-menu__item" v-for="ctxitem in screenItemCtxMenuItems"><a href="#"
					class="context-menu__link" v-bind:data-action="ctxitem.action" v-bind:data-source="screenItemInContext!=null?screenItemInContext.getAttribute('id'):''" v-on:click="contextMenuItemClicked"><i
						v-bind:class="ctxitem.icon"></i>&nbsp;{{ctxitem.itemText}}</a></li>										
				
				<!-- Linked Items		
				<li class="context-menu__header context-menu_hr" v-if="screenItemInContext != null && screenItemInContext.getAttribute('data-link') != ''"><b><i class="fa fa-share-alt-square"></i>&nbsp;Linked Items</b></li>
					<li  v-if="screenItemInContext != null && screenItemInContext.getAttribute('data-link') != ''" class="context-menu__item" v-for="item in screenItemInContext.parent"><a href="#"
					class="context-menu__link" data-action="deleteLinkAction" v-bind:data-source="screenItemInContext!=null?screenItemInContext.getAttribute('id'):''" ><i
						class="fa fa-trash"></i>&nbsp;{{ctxitem}}</a></li> -->	
			</ul>
		</nav>
		
		<nav id="screen-context-menu" v-bind:class="'context-menu ' + (screenCtxMenuState == 1 ? 'context-menu--active' : '')">
			<ul class="context-menu__items">
				<li class="context-menu__header"><b>{{screenInContext!=null?screenInContext.getAttribute('data-text'):""}}</b></li>
				<li class="context-menu__item" v-for="ctxitem in screenCtxMenuItems"><a href="#"
					class="context-menu__link" v-bind:data-action="ctxitem.action" data-source="screen" v-on:click="contextMenuItemClicked"><i
						v-bind:class="ctxitem.icon"></i>&nbsp;{{ctxitem.itemText}}</a></li>
						
						<li class="context-menu__item context-menu_hr"><a href="#" class="context-menu__link" v-on:click="toggleScreenEdit"><i v-bind:class="editMode?'fa fa-toggle-on':'fa fa-toggle-off'"></i>&nbsp;Screen Edit Mode</a></li>
			</ul>
		</nav>
		
	</div>

	<script type="text/javascript">
			CanvasRenderingContext2D.prototype.clear = 
				CanvasRenderingContext2D.prototype.clear || function (preserveTransform) {
					if (preserveTransform) {
				    	this.save();
				    	this.setTransform(1, 0, 0, 1, 0, 0);
				    }//end if
		
				    this.clearRect(0, 0, this.canvas.width, this.canvas.height);
		
				    if (preserveTransform) {
				    	this.restore();
				    }//end if        
				};
				
			/* Vue Entries */
			var data = {
				//Label texts
				stringResources			: {
											version: "V1.01"
										},
				screenItems_dummy		: [],					
				screenItems				: [
											{//screen item
												id			: "screenItem_1",
												parent		: [],//screenItem id's for drawing lines
												title		: "Title 1", 
												subTitle	: "Status Default", 
												left		: 40,//px 
												top			: 100,//px 
												width		: 125,//px 
												height		: 55,//px 
												type		: 0,//[0:screenItemDefault;1:screenItemSuccess;2:screenItemWarning;3:screenItemDanger;4:screenItemInfo] 
												alarm		: 0//[0:No alarm;1:warning;2:danger]
											},
										   	
											{id: "screenItem_2", parent: ["screenItem_1"], 					title: "Title 2", subTitle: "Status Success", 	left:  40, top: 200, width: 125, height: 55, type: 1, alarm: 1},//warning
										   	{id: "screenItem_3", parent: [], 								title: "Title 3", subTitle: "Status Warning", 	left:  40, top: 300, width: 125, height: 55, type: 2, alarm: 2},//danger
										   	{id: "screenItem_4", parent: ["screenItem_1", "screenItem_2"], 	title: "Title 4", subTitle: "Status Danger", 	left: 240, top: 100, width: 125, height: 55, type: 3, alarm: 3},//no alarm
										   	{id: "screenItem_5", parent: [], 								title: "Title 5", subTitle: "Status Info", 		left: 240, top: 200, width: 125, height: 55, type: 4, alarm: 4}//no alarm
										  ],
				
				//[0:drawArrowConnector; 1:drawLine; 2:drawShortestConnection]
				connectorType			: 0, 
				
				//Current container, the one holding the draw buffer
				container				: null,
				
				//Current modus
				editMode				: true,
				
				//800msec toggle true/false
				cycleTrigger			: false,
				
				screenItemInContext		: null,
				screenItemClassName		: "screenItem",
				//screenItemCtxMenu		: document.querySelector("#screen-item-context-menu"),
				screenItemCtxMenuState	: 0,
				screenItemCtxMenuItems	: [{itemText: "Edit Screen Item", icon: "fa fa-edit", action: "MyEditAction"}, {itemText: "View Screen Item", icon: "fa fa-eye", action: "MyViewAction"}, {itemText: "Delete Screen Item", icon: "fa fa-times", action: "MyDeleteAction"}],

				screenInContext		: null,
				screenClassName		: "screen",
				//screenItemCtxMenu		: document.querySelector("#screen-item-context-menu"),
				screenCtxMenuState	: 0,
				screenCtxMenuItems	: [{itemText: "Edit Screen", icon: "fa fa-edit", action: "MyScreenEditAction"}, {itemText: "View Screen", icon: "fa fa-eye", action: "MyScreenViewAction"}, {itemText: "Delete Screen", icon: "fa fa-times", action: "MyScreenDeleteAction"}],
				
			}//end data
		
			/* Vue Application */
			var vApp = new Vue({
				//current vue binding
				el: '#vueApp',
				
				//define variables under the `data` object
				data: data,

				watch: {
					// whenever connectorType changes, this function will run
					connectorType: function () {
						 //Update draw buffer
						 vApp.drawProcessGroupConnector();
					},
					// whenever screenItems changes, this function will run
					screenItems: function () {
						 //Update draw buffer						 
						 this.$nextTick(() => {
							 vApp.drawProcessGroupConnector();
						})
					}
				},
				
				//define methods under the `methods` object
				methods: {
					arrayToCvs: function(arr_strings){
						var first = true;
						var result = "";
						
						for(var loop = 0; loop < arr_strings.length; loop++){
							if(!first) result += ",";
							result += arr_strings[loop];
							first = false;
						}//end for
						
						return result;
					},//end arrayToCvs()
					
					holdEvent: function(event){
						//Stop event for further propagation
						event.stopPropagation();
						event.preventDefault();
						//console.log("Hold Event", event);
					},
					
					dragStartEvent: function(event){
						event.dataTransfer.setData("text", event.target.getAttribute("data-id"));
						console.log("dragStartEvent", event.target.getAttribute("data-id"));
					},

					dropEvent: function(event){
						event.preventDefault();
						var data = event.dataTransfer.getData("text");
						var child = event.target;

						while(!child.getAttribute("id")){
							child = child.parentNode;
						}//end while
							
						var id = child.getAttribute("id");

						var sio = this.getScreenItem(id);

						if(data != id && sio.parent.indexOf(data) == -1){							
							 sio.parent.push(data);
							 //Update draw buffer						 
							 this.$nextTick(() => {
								 vApp.drawProcessGroupConnector();
							});							
						}//end if
					},
					
					toggleScreenEdit: function(){
						this.editMode = !this.editMode;
						this.drawProcessGroupConnector();
					},
					
					startCycleDriver: function(){
						console.log("Version: " + this.stringResources.version)
						
						const self = this;
						//recursive call as driver for the animation cylce
						(function cycleDriver(){
						  	self.cycle();
						  	window.setTimeout(cycleDriver, 800);
						})();//end cycleDriver()
					},
					
					cycle: function(){
						this.cycleTrigger = !this.cycleTrigger;
						
						for(var loop = 0; loop < this.screenItems.length; loop++){
							var element = document.getElementById(this.screenItems[loop].id);							
							switch(this.screenItems[loop].alarm){
								case 1:
									element.classList.remove("screenItemDangerHighLight");
									if(this.cycleTrigger)
										element.classList.add("screenItemWarningHighLight");									
									else
										element.classList.remove("screenItemWarningHighLight");
									break;
								case 2:
									element.classList.remove("screenItemWarningHighLight");
									if(this.cycleTrigger)
										element.classList.add("screenItemDangerHighLight");									
									else
										element.classList.remove("screenItemDangerHighLight");
									break;
								default:
									element.classList.remove("screenItemDangerHighLight");
									element.classList.remove("screenItemWarningHighLight");
								break;
							}//end switch
						}//end for
					},//end cycle()
					
					/*
						Get ScreenItem by ID
					*/
					getScreenItem: function(id){
						for(item in this.screenItems)
							if(this.screenItems[item].id == id)
								return this.screenItems[item];
					},
					
					mouseClick: function(event){
						console.log(event, event.currentTarget);
					},				
					
					mouseDown: function(event){
						//Event only available when in edit mode
						if(!this.editMode)
							return;
						//Need to patch this !!!
						if(!event.target.getAttribute("data-text"))
							return;
						
						const sourceElement = event.currentTarget;
						const container		= sourceElement.parentNode;		  
						const sourceWidth 	= container.offsetWidth;
						const sourceHeight 	= container.offsetHeight;
						const self 			= this;
						  
						//Stop event for further propagation
						event.stopPropagation();
						event.preventDefault();
						 
						 //Store the current position
						 var originalLeft = sourceElement.offsetLeft - sourceElement.scrollLeft;
						 var originalTop = sourceElement.offsetTop - sourceElement.scrollTop;
						 
						 //Store original mouse position during mouseDown event
						 var mouseDownX = event.clientX;
						 var mouseDownY = event.clientY;
						 
						 //Set new absolute position within the parent
						 sourceElement.style.position = "absolute";
						 sourceElement.style.left = originalLeft + "px";
						 sourceElement.style.top = originalTop + "px";
					
						function mouseMoveEvent(_event){
							sourceElement.style.left = Math.min(sourceWidth - sourceElement.offsetWidth, Math.max(20, (Math.floor( (originalLeft + _event.clientX - mouseDownX)/10)*10))) + "px";
							sourceElement.style.top = Math.min(sourceHeight - sourceElement.offsetHeight, Math.max(20, (Math.floor((originalTop + _event.clientY - mouseDownY)/10)*10)))  + "px";
							 
							 //Update draw buffer
							 self.drawProcessGroupConnector();
							 
							 //Stop event for further propagation
							_event.stopPropagation();
						_event.preventDefault();
						}//end mouseMoveEvent()
					
						//Event handler for 'mouseup' event
						function mouseUpEvent(_event){
							//Remove event handlers after mouseup event
							document.removeEventListener("mousemove", mouseMoveEvent, true);
							document.removeEventListener("mouseup", mouseUpEvent, true);
							 
							//Store current position
							const item = vApp.getScreenItem(sourceElement.getAttribute("id"));
							item.left = sourceElement.style.left;
							item.top = sourceElement.style.top;
							 
							//Stop event for further propagation
							_event.stopPropagation();
							_event.preventDefault();
						}//end mouseUpEvent()	
					  
						//Attach new events to element during 'mousedown' event 
						document.addEventListener("mouseup", mouseUpEvent, true);
						document.addEventListener("mousemove", mouseMoveEvent, true);		  
					},//end mouseDown
					
					findAllConnectedProcessGroups: function (parent){
						const self = this;
						var elements = parent.querySelectorAll("[data-link]");
						var connectors = [];
						for (var loop = 0; loop < elements.length; loop ++){				
							elements[loop].getAttribute("data-link").split(",").forEach(function(linkedScreenItem){
								if(linkedScreenItem){
									var parentScreenItem = parent.querySelector("#"+linkedScreenItem);
									if(parentScreenItem){
										connectors.push(self.findShortestElementConnection(parentScreenItem, elements[loop]));
									}//end if						
								}//end if
							});
						}//end for		
						return connectors;
					},//end findAllConnectors()

					/**
					 * 
					 * @param element
					 * @param parent The parent element
					 * @returns
					 */
					 createConnector: function(element, parent){
						var chld = element.getBoundingClientRect();
						return [
								{'parent':parent, 'id':'b', 'enabled': true,'x':chld.right,'y': chld.top + (chld.height/2)},
						       	{'parent':parent, 'id':'a', 'enabled': true,'x':chld.left + (chld.width/2),'y': chld.top},
								{'parent':parent, 'id':'c', 'enabled': true,'x':chld.left + (chld.width/2),'y': chld.bottom},
								{'parent':parent, 'id':'d', 'enabled': true,'x':chld.left,'y': chld.top + (chld.height/2)},
								{'parent':parent, 'id':'m', 'enabled': false,'x':chld.left + (chld.width/2),'y': chld.top + (chld.height/2)},
								{'parent':parent, 'id':'e', 'enabled': false,'x':chld.right,'y': chld.bottom},
						       	{'parent':parent, 'id':'f', 'enabled': false,'x':chld.right,'y': chld.top},
								{'parent':parent, 'id':'g', 'enabled': false,'x':chld.left,'y': chld.bottom},
								{'parent':parent, 'id':'h', 'enabled': false,'x':chld.left,'y': chld.top}//,
							];
					},//end createConnector()

					findShortestElementConnection: function(parent, child){			
						var pcon = this.createConnector(parent, parent);
						var ccon = this.createConnector(child, parent);
						
						var len = 999999999;
						var lenobj = null;
						var o1 = null;
						var o2 = null;
						
						for(var loop = 0; loop < pcon.length; loop++){				  
							for(var test = 0; test < ccon.length; test++){
								if( pcon[loop].enabled && ccon[test].enabled){
									var l = Math.sqrt(Math.pow(Math.abs(pcon[loop].x-ccon[test].x),2)+Math.pow(Math.abs(pcon[loop].y-ccon[test].y),2));
							  
									if(l < len){
										o1 = pcon[loop];
										o2 = ccon[test];
										len = l;
									}//end if
							 	}//end if
							}//end for
						}//end for
					 
					 	return  {'p': o1,
						 		 'c': o2};
					},//findShortestElementConnection()
					  
					drawProcessGroupConnector: function(parent, selected){
						if(!parent)
							parent = this.container;
						
						if(parent.ctx){
							//clear the draw area
							parent.ctx.clear();
							
							if(this.editMode)
								this.drawGrid(parent.ctx);
							
							//Find connectors to draw
							var con = this.findAllConnectedProcessGroups(parent);
							//Draw the connectors
							for(var loop = 0; loop < con.length; loop++){
								//Highlight current connections when hover above the applicable process group
								if(selected && con[loop].p.parent.id == selected.element.id)
									switch(this.connectorType){
									case 1:
										this.drawLine(parent.ctx, con[loop].p.x, con[loop].p.y, con[loop].c.x, con[loop].c.y, "#FF00FF");
										break;
									case 2:
										this.drawShortestConnection(parent.ctx, con[loop].p, con[loop].c);
										break;
									default:
										this.drawArrowConnector(parent.ctx, con[loop].p.x, con[loop].p.y, con[loop].c.x, con[loop].c.y, "#FF00FF");
										break;
									}//end switch
								else
									switch(this.connectorType){
									case 1:
										this.drawLine(parent.ctx, con[loop].p.x, con[loop].p.y, con[loop].c.x, con[loop].c.y, "#00005A");
										break;
									case 2:
										this.drawShortestConnection(parent.ctx, con[loop].p, con[loop].c);
										break;
									default:
										this.drawArrowConnector(parent.ctx, con[loop].p.x, con[loop].p.y, con[loop].c.x, con[loop].c.y, "#00005A");
										break;
									}//end switch
							}//end for
							
						}//end if					
					  },//end drawProcessGroupConnector()
					  
					  drawGrid: function(ctx) {
						    var w = ctx.canvas.width;
						    var h = ctx.canvas.height;
						    var step = 10;
						    ctx.beginPath(); 
						    for (var x=1;x<=w;x+=step) {
						            ctx.moveTo(x, 0);
						            ctx.lineTo(x, h);
						    }
						    
						    for (var y=1;y<=h;y+=step) {
						            ctx.moveTo(0, y);
						            ctx.lineTo(w, y);
						    }
						    // set the color of the line
						    ctx.strokeStyle = 'rgb(228,228,228)';
						    ctx.lineWidth = 1;
						    // the stroke will actually paint the current path 
						    ctx.stroke(); 
						},
					
					  drawLine: function(ctx, fromx, fromy, tox, toy){
						    var offset = ctx.canvas.getBoundingClientRect();
						    fromx = fromx - offset.left;
						    fromy = fromy - offset.top;
						    tox = tox - offset.left;
						    toy = toy - offset.top;	
						    
							ctx.beginPath();
							ctx.moveTo(fromx, fromy);
							ctx.lineTo(tox, toy);
							ctx.strokeStyle = "#101010";
							ctx.lineWidth = 1;
							ctx.stroke();
							ctx.closePath();
					  },
					  
					  drawArrowConnector: function(ctx, fromx, fromy, tox, toy, color){
						    var offset = ctx.canvas.getBoundingClientRect();
						    fromx = fromx - offset.left;
						    fromy = fromy - offset.top;
						    tox = tox - offset.left;
						    toy = toy - offset.top;	
						     //variables to be used when creating the arrow
						     var headlen = 10;
						     var angle = Math.atan2(toy-fromy,tox-fromx);
						     //starting path of the arrow from the start square to the end square and drawing the stroke
						     ctx.beginPath();
						     ctx.moveTo(fromx, fromy);
						     ctx.lineTo(tox, toy);
						     ctx.strokeStyle = color;
						     ctx.lineWidth = 1;
						     ctx.stroke();
						     //starting a new path from the head of the arrow to one of the sides of the point
						     ctx.beginPath();
						     ctx.moveTo(tox, toy);
						     ctx.lineTo(tox-headlen*Math.cos(angle-Math.PI/7),toy-headlen*Math.sin(angle-Math.PI/7));
						     //path from the side point of the arrow, to the other side point
						     ctx.lineTo(tox-headlen*Math.cos(angle+Math.PI/7),toy-headlen*Math.sin(angle+Math.PI/7));
						     //path from the side point back to the tip of the arrow, and then again to the opposite side point
						     ctx.lineTo(tox, toy);
						     ctx.lineTo(tox-headlen*Math.cos(angle-Math.PI/7),toy-headlen*Math.sin(angle-Math.PI/7));
						     //draws the paths created above
						     ctx.strokeStyle = color;
						     ctx.lineWidth = 3;
						     ctx.stroke();
						     ctx.fillStyle = color;
						     ctx.fill();
						 },//end drawArrow()
					  
						 drawArrow: function (ctx, fromx, fromy, tox, toy, color){
							var offset = ctx.canvas.getBoundingClientRect();
							fromx = fromx - offset.left;
							fromy = fromy - offset.top;
							tox = tox - offset.left;
							toy = toy - offset.top;	
							    
						     //variables to be used when creating the arrow
						     var headlen = 10;
						     var angle = Math.atan2(toy-fromy,tox-fromx);
						     //starting path of the arrow from the start square to the end square and drawing the stroke
						     ctx.beginPath();
						     ctx.moveTo(fromx, fromy);
						     ctx.lineTo(tox, toy);
						     ctx.strokeStyle = color;
						     ctx.lineWidth = 1;
						     ctx.stroke();
						     //starting a new path from the head of the arrow to one of the sides of the point
						     ctx.beginPath();
						     ctx.moveTo(tox, toy);
						     ctx.lineTo(tox-headlen*Math.cos(angle-Math.PI/7),toy-headlen*Math.sin(angle-Math.PI/7));
						     //path from the side point of the arrow, to the other side point
						     ctx.lineTo(tox-headlen*Math.cos(angle+Math.PI/7),toy-headlen*Math.sin(angle+Math.PI/7));
						     //path from the side point back to the tip of the arrow, and then again to the opposite side point
						     ctx.lineTo(tox, toy);
						     ctx.lineTo(tox-headlen*Math.cos(angle-Math.PI/7),toy-headlen*Math.sin(angle-Math.PI/7));
						     //draws the paths created above
						     ctx.strokeStyle = color;
						     ctx.lineWidth = 3;
						     ctx.stroke();
						     ctx.fillStyle = color;
						     ctx.fill();
						 },//end drawArrow()
							 
						 drawShortestConnection: function (ctx, parent, child, drawConnectorId){
							var w = Math.abs(parent.x - child.x)
							var h = Math.abs(parent.y - child.y)
							
							var ptoffsetx = 0;
							var ptoffsety = 0;

							var ctoffsetx = 0;
							var ctoffsety = 0;

							if(parent.id == 'a' && child.id == 'b'){
								ctoffsetx = +10;
								ctoffsety = -10;
								ptoffsetx = +10;
								ptoffsety = -10;
								this.drawLine(ctx, parent.x, parent.y, parent.x, child.y);
								this.drawArrow(ctx, parent.x, child.y, child.x, child.y);
							}
							else if(parent.id == 'a' && child.id == 'c'){
								ctoffsetx = +10;
								ctoffsety = 20;
								ptoffsetx = +10;
								ptoffsety = -10;
								this.drawLine(ctx, parent.x, parent.y,       parent.x, parent.y - h/2);				
								this.drawLine(ctx, child.x, child.y + h/2, parent.x, parent.y - h/2);				
								this.drawArrow(ctx, child.x, child.y + h/2, child.x , child.y);
							}
							
							else if(parent.id == 'a' && child.id == 'd'){
								ctoffsetx = -20;
								this.drawLine(ctx, parent.x, child.y, parent.x, parent.y);
								this.drawArrow(ctx, parent.x, child.y, child.x, child.y);
							}
							
							else if(parent.id  == 'b' && child.id == 'a'){
								ctoffsetx = +10;
								ctoffsety = -10;
								ptoffsetx = +10;
								ptoffsety = -10;
								this.drawLine(ctx, parent.x, parent.y, child.x, parent.y);
								this.drawArrow(ctx, child.x, parent.y, child.x, child.y);
							}
							
							else if(parent.id == 'b' && child.id == 'c'){
								ctoffsetx = +10;
								ptoffsety = -10;
								ptoffsetx = +10;
								ctoffsety = 20;
								this.drawLine(ctx, child.x, parent.y, parent.x, parent.y);
								this.drawArrow(ctx, child.x, parent.y, child.x, child.y);
							}
							
							else if(parent.id == 'b' && child.id == 'd'){
								ctoffsetx = -20;
								ctoffsety = -10;
								ptoffsetx = +10;
								ptoffsety = -10;
								this.drawLine(ctx, parent.x, parent.y, parent.x + w/2, parent.y);
								this.drawLine(ctx, child.x - w/2, child.y, parent.x + w/2, parent.y);				
								this.drawArrow(ctx, child.x - w/2, child.y, child.x, child.y);
							}
							
							else if(parent.id == 'c' && child.id == 'a'){
								ctoffsetx = +10;
								ctoffsety = -10;
								ptoffsetx = +10;
								ptoffsety = 20;
								this.drawLine(ctx, parent.x, parent.y,       parent.x, parent.y + h/2);				
								this.drawLine(ctx, child.x, child.y - h/2, parent.x, parent.y + h/2);				
								this.drawArrow(ctx, child.x, child.y - h/2, child.x , child.y);
							}
							
							else if(parent.id == 'c' && child.id == 'b'){
								ctoffsetx = +10;
								ctoffsety = -10;
								ptoffsetx = +10;
								ptoffsety = 20;
								this.drawLine(ctx, parent.x, child.y, parent.x, parent.y);
								this.drawArrow(ctx, parent.x, child.y, child.x, child.y);
							}
							
							else if(parent.id == 'd' && child.id == 'a'){
								ctoffsetx = +10;
								ctoffsety = -10;
								ptoffsetx = +10;
								ptoffsety = -10;
								this.drawLine(ctx, child.x, parent.y, parent.x, parent.y);
								this.drawArrow(ctx, child.x, parent.y, child.x, child.y);
							}
							
							else if(parent.id == 'd' && child.id == 'b'){
								ctoffsetx = +20;
								ctoffsety = -10;
								ptoffsetx = -20;
								ptoffsety = -10;
								this.drawLine(ctx, parent.x, parent.y      , child.x + w/2, parent.y);
								this.drawLine(ctx, child.x + w/2, parent.y, child.x + w/2, child.y);				
								this.drawArrow(ctx, child.x + w/2, child.y, child.x, child.y);
							}
							
							else if(parent.id == 'd' && child.id == 'c'){
								ptoffsetx = -20;
								ctoffsety = +20;
								this.drawLine(ctx, parent.x, parent.y      , parent.x - w/2, parent.y);				
								this.drawArrow(ctx, child.x - w/2, child.y, child.x, child.y);
							}
							
							if(drawConnectorId){
								ctx.fillStyle    = '#00F';
					            ctx.font         = 'Italic 16px Sans-Serif';            
					            ctx.textBaseline = 'Top';
					            ctx.fillText  (parent.id, parent.x + ptoffsetx, parent.y + ptoffsety);
					            ctx.fillText  (child.id, child.x + ctoffsetx, child.y + ctoffsety);
							}
						 },//end  drawShortestConnection()
						 
						 /**
						 * Create Process Screen draw buffer.
						 * 
						 * To be able to draw on the process screen we need a canvas to draw on. This canvas is layered behind all
						 * process group objects.
						 * 
						 * @param parent The parent object where to place the draw buffer, normally a DIV element.
						 * @param width The width of the Canvas object
						 * @param height The height of the Canvas object.
						 * @returns A Canvas object (Also appended to the parent element).
						 */
						 createProcessScreenDrawBuffer: function(parent, width, height){
							//Create a Canvas element to draw on.
							var cvs = document.createElement("CANVAS");
							
							//Set placement details for Canvas element
							cvs.setAttribute("style","position:absolute;z-index:-1;background-color:transparent;");
							
							//Set dimension details for Canvas element
							cvs.style.width 	= width+"px";
							cvs.style.height 	= height+"px";
							cvs.top 			= 0;
							cvs.left 			= 0;
							cvs.width 			= width;
							cvs.height 			= height;
							
							//Append the Canvas to parent element
							parent.appendChild(cvs);
							
							//Add draw context to parent
							parent.ctx = cvs.getContext("2d");
						},//end createProcessScreenDrawBuffer()
						
						invertColor: function(rgb) {
						  rgb = Array.prototype.join.call(arguments).match(/(-?[0-9\.]+)/g);
						  for (var i = 0; i < rgb.length; i++) {
						    rgb[i] = (i === 3 ? 1 : 255) - rgb[i];
						  }
						  return rgb;
						},
						
					 	/**
					   	* Function to check if we clicked inside an element with a particular class
					   	* name.
					   	* 
					   	* @param {Object} e The event
					   	* @param {String} className The class name to check against
					   	* @return {Boolean}
					   	*/
					   	clickInsideElement: function(e) {
						    var el = e.srcElement || e.target;
						    
						    if ( el.getAttribute("data-ctxmenu") ) {
						      return el;
						    } else {
						      while ( el = el.parentNode ) {
						        if ( el.getAttribute("data-ctxmenu")  ) {
						          return el;
						        }
						      }
						    }

						    return false;
						},

						/**
						* Get's exact position of event.
						* 
						* @param {Object} e The event passed in
						* @return {Object} Returns the x and y position
						*/
						getPosition: function(e) {
						    var posx = 0;
						    var posy = 0;

						    if (!e) var e = window.event;
						    
						    if (e.pageX || e.pageY) {
						      posx = e.pageX;
						      posy = e.pageY;
						    } else if (e.clientX || e.clientY) {
						      posx = e.clientX + document.body.scrollLeft + document.documentElement.scrollLeft;
						      posy = e.clientY + document.body.scrollTop + document.documentElement.scrollTop;
						    }

						    return {
						      x: posx,
						      y: posy
						    }
						  },

					/**
					* Positions the menu properly.
					* 
					* @param {Object} e The event
					* @param {Object} screenItemCtxMenu The object the user clicked on
					*/
					positionContextMenu: function(e, screenItemCtxMenu) {
						clickCoords = this.getPosition(e);
						clickCoordsX = clickCoords.x;
						clickCoordsY = clickCoords.y;
						
						menuWidth = screenItemCtxMenu.offsetWidth + 4;
						menuHeight = screenItemCtxMenu.offsetHeight + 4;
						
						windowWidth = window.innerWidth;
						windowHeight = window.innerHeight;
						
						if ( (windowWidth - clickCoordsX) < menuWidth ) {
							screenItemCtxMenu.style.left = windowWidth - menuWidth + "px";
						}//end if
						else {
							screenItemCtxMenu.style.left = clickCoordsX + "px";
						}//end else
						
						if ( (windowHeight - clickCoordsY) < menuHeight ) {
							screenItemCtxMenu.style.top = windowHeight - menuHeight + "px";
						}//end if
						else {
							screenItemCtxMenu.style.top = clickCoordsY + "px";
						}//end else
					},//end positionContextMenu()						  

					/**
					* Turns the screenItem context menu on.
					*/
					showContextMenu: function (screenItemInContext) {						
						if(screenItemInContext && screenItemInContext.getAttribute("data-ctxmenu") == "screen-item-context-menu"){
							this.screenItemInContext = screenItemInContext;
							this.screenItemCtxMenuState = 1;
							this.screenCtxMenuState = 0;
						}//end if
						else if(screenItemInContext && screenItemInContext.getAttribute("data-ctxmenu") == "screen-context-menu"){
							this.screenInContext = screenItemInContext;
							this.screenCtxMenuState = 1;
							this.screenItemCtxMenuState = 0;							
						}//end else
					},//end showContextMenu()

					/**
					* Turns the screenItem context menu off.
					*/  
					hideContextMenu: function () {
						this.screenItemCtxMenuState = 0;
						this.screenCtxMenuState = 0;
					},//end hideContextMenu()
					
					/*
						Called when user clicks on a context-menu item.
					*/
					contextMenuItemClicked: function(event){
						const source = this.getScreenItem(event.currentTarget.getAttribute("data-source"));
						const action = event.currentTarget.getAttribute("data-action");
						console.log("Context Item Clicked", source, action, event.currentTarget);
					},//end contextMenuItemClicked()
					
					/*
						Called when user right clicks on mouse, open context menu.
					*/
					contextClick: function(event){	
						const screenItemInContext = this.clickInsideElement(event);
					
						if (screenItemInContext) {
							event.preventDefault();
							
							this.showContextMenu(screenItemInContext);
							this.positionContextMenu(event, document.getElementById(screenItemInContext.getAttribute("data-ctxmenu")));      
						}//end if
						else {
							this.hideContextMenu();
						}//end else
					},//end contextClick()

					/**
					* Turns the screenItem context menu off when clicked outside applicable elements.
					*/ 
					bodyClickListener: function(event){
						this.hideContextMenu();
					},
				},//end methods
				
				//define methods under the `computed` object	
				computed :{
				},//end computed
				
				mounted: function(){
					console.log("Mounted vApp " + this.stringResources.version);
					this.container		= document.getElementById("vueApp");
					const sourceWidth	= this.container.offsetWidth;
					const sourceHeight	= this.container.offsetHeight;	
					//Create the draw-buffer
					this.createProcessScreenDrawBuffer(this.container, sourceWidth, sourceHeight);
					//Draw the applicable connectors
					this.drawProcessGroupConnector();
					//Reference to methods
					this.startCycleDriver();
				}//end mounted()
			});//end vApp()
			
			function load(src){
				console.log(src);
			}
		</script>
</body>
</html>