---
layout: post
title: Which V/Line train type is the most reliable?
date: 2018-04-10 07:30
author: wongm
comments: true
canonical: https://wongm.com/2018/04/vline-trains-which-type-most-reliable/
categories: [locomotive hauled trains, Public Transport Victoria, reliability, Sprinter trains, train, Trains, transport, V/Line, VLocity]
---
V/Line operates a real mixed bag of rolling stock to provide train services across Victoria - but which type of train is the most reliable?

<a href="http://railgallery.wongm.com/vline-workshops-yards/F119_3710.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-workshops-yards/F119_3710_500.jpg" alt="A66 now visible among the stabled trains at Dudley Street" /></a>

<strong>V/Line fleet overview</strong>

The newest trains in the V/Line fleet are the <a href="https://en.wikipedia.org/wiki/V/Line_VLocity" target="_blank" rel="noopener">VLocity diesel multiple units</a>. Each train is made up of three carriages, each with a diesel engine beneath.

The first units entered service in 2004, with additional trains rolling out of the Bombardier factory at Dandenong every few months.

<a href="http://railgallery.wongm.com/vline-melbourne/F115_1956.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-melbourne/F115_1956_500.jpg" alt="VLocity VL05 arrives into Flinders Street Station on an up service" /></a>

Next up are the <a href="https://en.wikipedia.org/wiki/V/Line_Sprinter" target="_blank" rel="noopener">Sprinter diesel multiple units</a>. Mechanically similar to the newer VLocity trains, the Sprinter fleet was built between 1993 and 1995, so are now approaching 25 years of age.

<a href="http://railgallery.wongm.com/vline-workshops-yards/F123_5870.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-workshops-yards/F123_5870_500.jpg" alt="Solo Sprinter 7002 sitting in the platform at Southern Cross" /></a>

But the oldest part of the V/Line fleet is what they call their 'classic fleet', carriages hauled by diesel locomotives.

The <a href="https://en.wikipedia.org/wiki/V/Line_N_class" target="_blank" rel="noopener">N class</a> are the core of the V/Line locomotive fleet, with 25 units built between 1985 and 1987.

<a href="http://railgallery.wongm.com/vline-geelong/F123_9324.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-geelong/F123_9324_500.jpg" alt="N469 leads a mixed liveried consist on an up Warrnambool service at Manor" /></a>

Along with a single <a href="https://en.wikipedia.org/wiki/V/Line_A_class" target="_blank" rel="noopener">A class locomotive</a> - built in 1985 on the frame of a <a href="https://en.wikipedia.org/wiki/Victorian_Railways_B_class_(diesel)" target="_blank" rel="noopener">B class locomotive</a> built way back in 1952.

<a href="http://railgallery.wongm.com/vline-bacchus-marsh/F120_7428.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-bacchus-marsh/F120_7428_500.jpg" alt="A66 crosses the Melton Weir on an up Bacchus Marsh service" /></a>

While V/Line's carriage fleet fall into three classes.

The newest are the <a href="https://en.wikipedia.org/wiki/VicRail_N_type_carriage" target="_blank" rel="noopener">'N' type carriages</a>, built in the early 1980s and used on long distance services.

<a href="http://railgallery.wongm.com/vline-new-mk4-livery/F119_0913.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-new-mk4-livery/F119_0913_500.jpg" alt="Economy class carriage with buffet compartment BRN34" /></a>

The <a href="https://en.wikipedia.org/wiki/V/Line_H_type_carriage" target="_blank" rel="noopener">'H' type carriages</a> used on commuter trains are younger, having been built in 1984-1992, but using the bodies of retired <a href="https://en.wikipedia.org/wiki/Harris_(train)" target="_blank" rel="noopener">'Harris' suburban trains</a> from the 1950s.

<a href="http://railgallery.wongm.com/vline-workshops-yards/F120_6712.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-workshops-yards/F120_6712_500.jpg" alt="Five H sets stabled for the weekend at Dudley Street" /></a>

While the oldest are the <a href="https://en.wikipedia.org/wiki/Victorian_Railways_Z_type_carriage" target="_blank" rel="noopener">'Z' type carriages</a> used on long distance services - built way back in the 1950s, and the subject to <a href="https://www.ptv.vic.gov.au/about-ptv/media-centre/media-releases/v-line-to-remove-z-carriages-for-inspection/" target="_blank" rel="noopener">cracked bogies back in 2013</a>.

<a href="http://railgallery.wongm.com/vline-workshops-yards/F117_6939.jpg.html"><img src="http://railgallery.wongm.com/cache/vline-workshops-yards/F117_6939_500.jpg" alt="BZN276 and BZN273 stabled in the carriage sidings at Dudley Street" /></a>

<strong>So which train is more reliable?</strong>

One would expect something brand new should be more reliable than something old, and that a simple piece of machinery is less likely to break down than a complicated one.

Using that logic, a carriage is a simple box with doors on wheels, a locomotive is something complicated with an engine that can break down, and a diesel multiple unit is the most complex, putting all of the above into a tight space.

So which ones breaks down the most? The <a href="https://corporate.vline.com.au/getattachment/acc863ea-7212-48ec-bb58-cce1a7cdda18/Annual-Report-2016-17" rel="noopener" target="_blank">V/Line annual report for 2016-17</a> has the answer.

<div id="vlineFaultGraph" style="width: 500px; height: 300px; margin: 10px 0;"></div>
<script src="//code.highcharts.com/highcharts.js"></script>
<script>
jQuery(document).ready(function () {
    jQuery('#vlineFaultGraph').highcharts({
        chart: {
		type: 'bar'
	},
	title: {
		text: 'V/Line fleet reliability'
	},
	xAxis: {
		categories: ['Carriages', 'VLocity', 'Sprinter', 'Locomotives'],
		title: {
			text: null
		}
	},
	yAxis: {
		min: 0,
		title: {
			text: 'Kilometres between faults',
		},
		labels: {
			overflow: 'justify'
		}
	},
	tooltip: {
		enabled: false
	},
	plotOptions: {
		bar: {
			dataLabels: {
				enabled: true,
				format: "{y} km"
			}
		}
	},
	credits: {
		enabled: false
	},
	legend: {
		enabled: false
	},
	series: [{
		data: [162895, 157805, 42533, 22957]
	}]
    });
});
</script>

New trains are more reliable than old ones, and simple trains break down less than complicated ones.

The annual report explains further:

<blockquote><strong>VLocity</strong>

Each VLocity carriage travelled an average of 157,805 kilometres between faults in 2016-17 compared with 155,082 kilometres during 2015-16.

The average availability of VLocity carriages during scheduled service periods, which includes maintenance and operational issues, was 91.7 per cent against a target of 86.5, the percentage of the fleet that is required to meet timetable requirements.

<strong>Sprinters</strong>

This year, Sprinters travelled an average of 42,533 kilometres between faults, against a target of 30,259 kilometres. This compares with 40,066 kilometres between faults in 2016-17, a six per cent reliability improvement. 

The average availability of Sprinters was 85 per cent against the target of 84.6 per cent. This decrease from 90.3 per cent availability in 2016-17 was due to In Cab Equipment (ICE) radio installation and fire damage to a Sprinter, effectively reducing the fleet size by one for most of the year.

<strong>Carriages</strong>

Classic fleet carriages travelled an average of 162,895 kilometres between faults against a target of 130,000 kilometres.

Average carriage availability of 74.3 per cent is measured against a target of 73.2 per cent and was down from 81.4 per cent the previous year. This was due to carriages being unavailable after the Pirron Yallock level crossing collision and structural assessment to enable life extension until 2025.

<strong>Locomotives</strong>

Locomotives travelled an average of 22,957 kilometres between faults, against a target of 29,962 kilometres, compared with 27,049 kilometres in 2016-17. This represents a 15 per cent decrease. 

Average availability was 70.2 per cent, against a target of 69 per cent, compared with 82.1 per cent in the previous year due to the repair of the locomotive involved in the Pirron Yallock level crossing incident.</blockquote>

Some interesting data - the performance of an increasing elderly carriage fleet being a stand out.

<strong>So how old is the V/Line fleet</strong>

In August 2017 the Victorian Auditor-General's Office released their <a href="https://www.audit.vic.gov.au/sites/default/files/2017-08/20170809-VLine-Passenger-Services.pdf" rel="noopener" target="_blank">report into V/Line Passenger Services</a> - Figure 4D detailed the average age of rolling stock.

<table style="border-collapse: collapse; width: 500px; height: 276px;" border="0" width="192" cellspacing="0" cellpadding="0"><colgroup> <col style="width: 48pt;" span="3" width="64" /> </colgroup>
<tbody>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt; width: 48pt;" width="64" height="17">Asset type</td>
<td style="width: 48pt; text-align: right;" width="64">Average age (years)</td>
<td style="width: 48pt; text-align: right;" width="64">Design life (years)</td>
</tr>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt;" height="17">VLocity DMU</td>
<td align="right">6.8</td>
<td align="right">30</td>
</tr>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt;" height="17">Sprinter DMU</td>
<td align="right">20.9</td>
<td align="right">30</td>
</tr>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt;" height="17">N class locomotive</td>
<td align="right">32.8</td>
<td align="right">30</td>
</tr>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt;" height="17">N type carriages</td>
<td align="right">32.8</td>
<td align="right">30</td>
</tr>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt;" height="17">H type carriages</td>
<td align="right">52.4</td>
<td align="right">30</td>
</tr>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt;" height="17">Z type carriages</td>
<td align="right">56</td>
<td class="xl22" style="width: 48pt;" align="right" width="64">30</td>
</tr>
<tr style="height: 12.75pt;">
<td style="height: 12.75pt;" height="17">Power Vans</td>
<td align="right">54</td>
<td align="right">30</td>
</tr>
</tbody>
</table>
<small>VAGO, based on V/Line ACCRI Project, 2015</small>

As well as V/Line's historical neglect, of both infrastructure and rolling stock.

<blockquote>Asset management

In the past, major periodic maintenance funding has not kept pace with the levels of funding required to maintain a fully operational and reliable passenger network. This has resulted in a deterioration of the network.

Until recently V/Line did not have a comprehensive understanding of the condition of its assets. It was therefore unable to develop sound long-term asset management strategies or to make evidence-based decisions on how it funded and prioritised maintenance and renewal work.

In 2015, V/Line changed its asset management approach from ‘fix on fail’ to ‘predict and prevent’, based on known asset condition. V/Line has now identified its maintenance backlog and has prioritised investments according to criticality and risk. The scale of funding required to address the maintenance backlog is significant—approximately $534.8 million across the entire V/Line network.

Asset failures limit V/Line’s ability to deliver agreed service levels, resulting in customer delays and service cancellations. Many of the vehicles in V/Line’s rolling stock fleet have been in service beyond their expected life, which is typically 30 years. Consequently they have a high failure rate and require significant investment in replacement and refurbishment.</blockquote>

Given V/Line's difficulty in <a href="https://wongm.com/2017/08/vline-cater-for-future-growth-longer-high-capacity-trains/" rel="noopener" target="_blank">merely keeping up with patronage growth</a>, I don't see the retirement of life expired rolling stock happening any time soon.
