# autoTooltip
Tooltip plugin

<h1>Documentation :</h1>

<h3>How to initialize this component ?</h3>
	<code>
		$(".tooltip-trigger").tooltip();
	</code>
<p>You must put a "data-tooltip-text" attribute with your tooltip message</p>
	<button class="tooltip-trigger">Trigger me !</button>

You can also chose the side of your tooltip by the attribute "data-tooltip-position", but this system is automatic because it will look if there is enough space and then it will place the tooltip in an optimized space (side). <br />
							<b>bottom</b>, <b>top</b>, <b>right</b>, <b>left</b>
	</p>
<h3>Example with top position tooltip</h3>
	<button class="tooltip-trigger" data-tooltip-text="my tooltip text here" data-tooltip-position="top">trigger me !</button>

<h3>Event parameter</h3>
<p>Now the event trigger have two options: "hover" and "click"</p>
	$(".tooltip-trigger").tooltip({
	     event: "hover" // is the default
	});
<h3>Parameters table</h3>
<table>
							<tr>
								<th>Parameters</th>
								<th>Type</th>
								<th>Default value</th>
								<th>Values</th>
								<th>Description</th>
							</tr>
							<tr>
								<td>event</td>
								<td>string</td>
								<td>"hover"</td>
								<td>"hover", "click"</td>
								<td>Choose the event handler for the tooltip .</td>
							</tr>
							<tr>
								<td>animation</td>
								<td>string</td>
								<td>"scale"</td>
								<td>"scale", "fade", "slide"</td>
								<td>Choose the animation</td>
							</tr>
							<tr>
								<td>space</td>
								<td>int</td>
								<td>20</td>
								<td>[0 ; +]</td>
								<td>Chose a number that will respresent the space between the trigger and the tooltip</td>
							</tr>
						</table>
