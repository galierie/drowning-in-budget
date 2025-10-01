<h1 class="mb-8 text-center text-3xl">
	Drowning in Budget: How Flood Control Budget Correlates to Damage Caused by Flooding
</h1>
<p class="text-center">Submitted by: CS 132 25.1 WFV Group 1</p>
<p><b>Topic</b>: Flood Control Projects</p>
<p>
	<b>Sustainable Development Goal</b>: (11) Sustainable Cities and Communities: Urban Planning,
	Infrastructure Resilience, Environmental Sustainability
</p>
<br />

<h2 class="mb-6 text-2xl">Research Questions/Problems</h2>
<ol class="list-inside list-decimal">
	<li>
		What provinces and regions have the most flood control projects in terms of number and cost?
	</li>
	<li>
		How does the amount of budget allocated to a particular area correlate with damage, such as
		casualties, injuries, and infrastructure damage, caused by flooding?
	</li>
</ol>
<br />

<h2 class="mb-6 text-2xl">Proposed Solutions</h2>
<p>
	The group aims to analyze flood control projects from a data-driven perspective using the public
	dataset released by the government and correlate these to reports from the National Disaster Risk
	Reduction and Management Council (NDRRMC) to determine the potential tangible effect of these
	completed projects. These insights may be used not just to support calls for government
	accountability if the data shows that projects have been effective, but they may also provide next
	steps on what the government should invest into to truly improve disaster resilience.
</p>
<br />

<h2 class="mb-6 text-2xl">Background</h2>
<p>
	The Philippines consistently ranks among the most disaster prone countries in the world. The 2025
	World Risk Report listed the nation as the highest in disaster risk, particularly due to heavy
	exposure to river and coastal flooding across the entire archipelago (Bündnis Entwicklung Hilft,
	2025).
</p>
<p>
	Disasters cannot necessarily be prevented, but their impact on people can be mitigated through
	infrastructure, planning, and other measures. The government has supposedly invested in flood
	control projects to improve river control, water drainage and storage, sediment control, and other
	forms of protection from flooding (Du, 2025). However, these projects have been mired with
	corruption, with the government admitting that many of these are “ghost” projects which have never
	actually been completed (Bacelonia, 2025).
</p>
<p>
	Actual experiences of citizens this rainy season also point to these projects’ ineffectiveness,
	leading to intensifying calls for accountability both online in social media and through major
	protests in the streets in recent months.
</p>
<p>
	As public pressure toward truly effective flood control mounts, it is essential to gain
	data-driven insights on how completed projects affect statistics such as casualties, injuries, and
	amount of damage to infrastructure.
</p>
<br />

<h2 class="mb-6 text-2xl">Hypotheses</h2>
<ul class="list-inside list-disc">
	<li>
		Null Hypothesis: There is a positive correlation between damage reduction and flood control
		budget allocated per province.
	</li>
	<li>
		Alternative Hypothesis: A greater flood control budget does not have a positive correlation to
		damage reduction after flooding.
	</li>
</ul>
<br />

<h1 class="mt-8 mb-4 text-center text-3xl">
	<a
		target="_blank"
		href="https://docs.google.com/spreadsheets/d/1L5P4t8nBkBhUKDnGK6RVSqPo_8ItdH7pC6P_bCUHJoY/edit?gid=0#gid=0"
		class="text-blue-400 underline">Dataset</a
	>
</h1>
<br />

<p>From:</p>
<ul class="list-inside list-disc">
	<li>
		Department of Public Works and Highways <a
			target="_blank"
			href="http://kaggle.com/datasets/bwandowando/dpwh-flood-control-projects"
			class="text-blue-400 underline">Flood Control Projects (Kaggle)</a
		>

		<ul class="ml-6 list-inside list-disc">
			<li>
				The dataset is taken from the <a
					target="_blank"
					href="https://sumbongsapangulo.ph/"
					class="text-blue-400 underline">flood control project list</a
				> recently released by the government.
			</li>
		</ul>
	</li>
	<li>
		Situational Reports for the Combined Effects of Various Typhoons

		<ul class="ml-6 list-inside list-disc">
			<li>
				These reports are from <a
					target="_blank"
					href="https://ndrrmc.gov.ph/disaster-reports.html"
					class="text-blue-400 underline">NDRRMC</a
				>, but are searched via the
				<a
					href="https://www.adrc.asia/latest_disaster.php?country%5B%5D=608&event%5B%5D=8&event%5B%5D=10&event%5B%5D=11&event%5B%5D=21&event%5B%5D=22&event%5B%5D=28&event%5B%5D=30&event%5B%5D=31&event%5B%5D=32&word=&duration_start=&duration_end=&order=1&per_page=25"
					class="text-blue-400 underline">Asian Disaster Reduction Center</a
				> since the Situational Reports webpage in NDRRMC is inaccessible.
			</li>
		</ul>
	</li>
</ul>
<p>
	The project mainly utilized two data sets. The first data set was recently released by the
	Department of Public Works and Highways that contains completed flood control projects from July
	2022 to May 2025. For every project, there are fields that describe its (1) address and location,
	(2) associated district engineering office, (3) name and description, (4) allocated budget, (5)
	assigned contractors, (6) date of commencement, and (7) date of completion. The second data set is
	from the NDRRMC which contains typhoon census data from 2021 to 2025. Each data point has fields
	that describe the typhoon’s total casualties and damage to infrastructure.
</p>
<br />

<h2 class="mb-6 text-2xl">Data Collection Process</h2>
<p>The data set released by the Philippine government through sumbongsapangulo.ph, and reformatted into a spreadsheet format in Kaggle, was downloaded directly.  On the other hand, the second data set was processed by retrieving typhoon reports in PDF format from the National Risk Reduction and Management Council through the Asian Disaster Reduction Center. The group used iLovePDF to extract data of the (1) casualties and (2) damage to infrastructure in the form of a spreadsheet.  Each spreadsheet is then combined into one main spreadsheet to be used by the group for processing. Some cleanup is also done as after conversion, some errors exist, such as headers being repeated or text being broken up into multiple cells.</p>
<br />

<h2 class="mb-6 text-2xl">Sampling Methods</h2>
<p>Only typhoon and flooding data from 2021 to 2025 were considered because the data is most in line with the available flood control project data. Further, only the typhoon and flooding data which were available via the Asian Disaster Reduction Center and released by NDRRMC were considered due to their availability.</p>
<br />

<h1 class="my-8 text-center text-3xl">References</h1>
<div class="pl-6">
	<p class="-indent-6">
		Bacelonia, W. (2025, August 19). <i
			>Senate probe on flood control bares ghost projects, favoritism.</i
		>
		Philippine News Agency.
		<a
			target="_blank"
			href="https://www.pna.gov.ph/articles/1256868"
			class="text-blue-400 underline">https://www.pna.gov.ph/articles/1256868</a
		>
	</p>
	<p class="-indent-6">
		Bündnis Entwicklung Hilft. (2025, September 25). <i>The WorldRiskReport.</i> WeltRisikoBericht.
		<a
			target="_blank"
			href="https://weltrisikobericht.de/worldriskreport/"
			class="text-blue-400 underline">https://weltrisikobericht.de/worldriskreport/</a
		>
	</p>
	<p class="-indent-6">
		Du, S. (2025, August 18). <i>What's a flood control project, anyway?</i> Rappler.
		<a
			target="_blank"
			href="https://www.rappler.com/newsbreak/iq/what-is-flood-control-project/"
			class="text-blue-400 underline"
			>https://www.rappler.com/newsbreak/iq/what-is-flood-control-project/</a
		>
	</p>
	<br />
</div>
