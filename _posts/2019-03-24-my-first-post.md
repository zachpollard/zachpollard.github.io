---
layout: post
title: My Firt Post
---

#this is a title

(equivelent of h1)

##this is smaler

(equivelent of h2)

'''python
print("hello")
'''


a|b|c
---|---|---
1|2|3
4|5|6
7|8|9

$$
\sigma = \sigma \\

\LaTeX
$$

{% raw %}
<script src="https://cdn.jsdelivr.net/npm/frappe-charts@1.1.0/dist/frappe-charts.min.iife.js"></script>
{% endraw %}

{% raw %}
<div id="mychart"></div>

<script>
let chart = new frappe.Chart( "#frost-chart", { // or DOM element
	data: {
	labels: ["12am-3am", "3am-6am", "6am-9am", "9am-12pm",
		"12pm-3pm", "3pm-6pm", "6pm-9pm", "9pm-12am"],

	datasets: [
		{
			name: "Some Data", chartType: 'bar',
			values: [25, 40, 30, 35, 8, 52, 17, -4]
		},
		{
			name: "Another Set", chartType: 'bar',
			values: [25, 50, -10, 15, 18, 32, 27, 14]
		},
		{
			name: "Yet Another", chartType: 'line',
			values: [15, 20, -3, -15, 58, 12, -17, 37]
		}
	],

	yMarkers: [{ label: "Marker", value: 70,
		options: { labelPos: 'left' }}],
	yRegions: [{ label: "Region", start: -10, end: 50,
		options: { labelPos: 'right' }}]
	},

	title: "My Awesome Chart",
	type: 'axis-mixed', // or 'bar', 'line', 'pie', 'percentage'
	height: 300,
	colors: ['purple', '#ffa3ef', 'light-blue'],

	tooltipOptions: {
		formatTooltipX: d => (d + '').toUpperCase(),
		formatTooltipY: d => d + ' pts',
	}
  });
</script>
{% endraw %}
