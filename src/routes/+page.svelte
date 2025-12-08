<script>
	import { asset } from '$app/paths';

	import regionProjects from '$lib/assets/graphs/viz1 (0).jpg';
	import provinceProjects from '$lib/assets/graphs/viz1 (1).jpg';
	import regionProjectCosts from '$lib/assets/graphs/viz1 (2).jpg';
	import provinceProjectCosts from '$lib/assets/graphs/viz1 (3).jpg';

	import budgetCasualtyDamage from '$lib/assets/graphs/viz2.jpg';

	import nutshellDamage from '$lib/assets/graphs/nutshell_damage.jpg';
	import nutshellBudget from '$lib/assets/graphs/nutshell_budget.jpg';
	import nutshellCasualties from '$lib/assets/graphs/nutshell_casualties.jpg';

	import hypothesis from '$lib/assets/graphs/hypothesis.png';

	import ListIcon from './(ui)/ListIcon.svelte';
	import Member from './(ui)/Member.svelte';
</script>

<div class="mx-10">
	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">
			Research Questions/Problems
		</h2>
		<ul class="flex flex-col items-center justify-center text-center lg:flex lg:flex-row">
			<ListIcon icon="material-symbols:flood-outline">
				What provinces and regions have the most flood control projects in terms of number and cost?
			</ListIcon>
			<ListIcon icon="material-symbols:money-bag-outline">
				How does the amount of budget allocated to a particular area correlate with damage, such as
				casualties, injuries, and infrastructure damage, caused by flooding?
			</ListIcon>
		</ul>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Objectives</h2>
		<ul class="flex flex-col items-center justify-center text-center lg:flex lg:flex-row">
			<ListIcon icon="material-symbols:location-on-outline">
				Identify areas in which flood control projects are concentrated in terms of number and
				budget
			</ListIcon>
			<ListIcon icon="material-symbols:folder-copy-outline-rounded">
				Determine whether flood control projects are effective in truly curbing different forms of
				damages
			</ListIcon>
		</ul>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Proposed Solutions</h2>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			The group aims to analyze flood control projects from a data-driven perspective using the
			public dataset released by the government and correlate these to reports from the National
			Disaster Risk Reduction and Management Council (NDRRMC) to determine the potential tangible
			effect of these completed projects. These insights may be used not just to support calls for
			government accountability if the data shows that projects have been effective, but they may
			also provide next steps on what the government should invest into to truly improve disaster
			resilience.
		</p>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Background</h2>
		<div class="px-0 *:text-2xl md:px-15 lg:px-25">
			<p>
				The Philippines consistently ranks among the most disaster prone countries in the world. The
				2025 World Risk Report listed the nation as the highest in disaster risk, particularly due
				to heavy exposure to river and coastal flooding across the entire archipelago (Bündnis
				Entwicklung Hilft, 2025).
			</p>
			<br />
			<p>
				Disasters cannot necessarily be prevented, but their impact on people can be mitigated
				through infrastructure, planning, and other measures. The government has supposedly invested
				in flood control projects to improve river control, water drainage and storage, sediment
				control, and other forms of protection from flooding (Du, 2025). However, these projects
				have been mired with corruption, with the government admitting that many of these are
				“ghost” projects which have never actually been completed (Bacelonia, 2025).
			</p>
			<br />
			<p>
				Actual experiences of citizens this rainy season also point to these projects’
				ineffectiveness, leading to intensifying calls for accountability both online in social
				media and through major protests in the streets in recent months.
			</p>
			<br />
			<p>
				As public pressure toward truly effective flood control mounts, it is essential to gain
				data-driven insights on how completed projects affect statistics such as casualties,
				injuries, and amount of damage to infrastructure.
			</p>
		</div>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Hypotheses</h2>
		<ul class="flex flex-col items-center justify-center text-center lg:flex lg:flex-row">
			<ListIcon icon="material-symbols:chart-data-outline">
				Null Hypothesis: There is a positive correlation between damage reduction and flood control
				budget allocated per province.
			</ListIcon>
			<ListIcon icon="material-symbols:money-off-rounded">
				Alternative Hypothesis: A greater flood control budget does not have a positive correlation
				to damage reduction after flooding.
			</ListIcon>
		</ul>
	</section>
</div>

<div class="mx-10">
	<section class="my-18">
		<h1 class="p-12 text-center font-specialelite text-6xl font-bold">
			<a
				target="_blank"
				href="https://docs.google.com/spreadsheets/d/1L5P4t8nBkBhUKDnGK6RVSqPo_8ItdH7pC6P_bCUHJoY/edit?gid=0#gid=0"
				class="rounded-lg border-2 border-rhino-500 px-24 py-12 text-rhino-500 underline decoration-4 shadow-xl hover:bg-rhino-300"
				>Click to go to dataset</a
			>
		</h1>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Data Sources</h2>
		<ul class="flex flex-col items-center justify-center text-center lg:flex lg:flex-row">
			<ListIcon icon="material-symbols:road-rounded">
				<div class="text-left">
					<p>
						Department of Public Works and Highways <a
							target="_blank"
							href="http://kaggle.com/datasets/bwandowando/dpwh-flood-control-projects"
							class="text-rhino-500 underline">Flood Control Projects (Kaggle)</a
						>
					</p>

					<ul class="ml-6 list-inside list-disc">
						<li>
							The dataset is taken from the <a
								target="_blank"
								href="https://sumbongsapangulo.ph/"
								class="text-rhino-500 underline">flood control project list</a
							> recently released by the government.
						</li>
						<li><b>Dataset Size</b>: 9855 data points/projects</li>
					</ul>
				</div>
			</ListIcon>
			<ListIcon icon="material-symbols:landslide-outline-rounded">
				<div class="text-left">
					<p>Situational Reports for the Combined Effects of Various Typhoons</p>

					<ul class="ml-6 list-inside list-disc">
						<li>
							These reports are from <a
								target="_blank"
								href="https://ndrrmc.gov.ph/disaster-reports.html"
								class="text-rhino-500 underline">NDRRMC</a
							>, but are searched via the
							<a
								href="https://www.adrc.asia/latest_disaster.php?country%5B%5D=608&event%5B%5D=8&event%5B%5D=10&event%5B%5D=11&event%5B%5D=21&event%5B%5D=22&event%5B%5D=28&event%5B%5D=30&event%5B%5D=31&event%5B%5D=32&word=&duration_start=&duration_end=&order=1&per_page=25"
								class="text-rhino-500 underline">Asian Disaster Reduction Center</a
							> since the Situational Reports webpage in NDRRMC is inaccessible.
						</li>
						<li>
							<b>Dataset Size</b>
							<ul class="ml-12 list-inside list-disc">
								<li>Casualties, Injuries, or Missing: 719 entries</li>
								<li>Infrastructure Damage: 5030 entries</li>
							</ul>
						</li>
					</ul>
				</div>
			</ListIcon>
		</ul>

		<p class="my-12 px-0 text-2xl md:px-15 lg:px-25">
			The project mainly utilized two data sets. The first data set was recently released by the
			Department of Public Works and Highways that contains completed flood control projects from
			July 2022 to May 2025. For every project, there are fields that describe its (1) address and
			location, (2) associated district engineering office, (3) name and description, (4) allocated
			budget, (5) assigned contractors, (6) date of commencement, and (7) date of completion. The
			second data set is from the NDRRMC which contains typhoon census data from 2021 to 2025. Each
			data point has fields that describe the typhoon’s total casualties and damage to
			infrastructure.
		</p>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Data Collection Process</h2>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			The data set released by the Philippine government through sumbongsapangulo.ph, and
			reformatted into a spreadsheet format in Kaggle, was downloaded directly. On the other hand,
			the second data set was processed by retrieving typhoon reports in PDF format from the
			National Risk Reduction and Management Council through the Asian Disaster Reduction Center.
			The group used iLovePDF to extract data of the (1) casualties and (2) damage to infrastructure
			in the form of a spreadsheet. Each spreadsheet is then combined into one main spreadsheet to
			be used by the group for processing. Some cleanup is also done as after conversion, some
			errors exist, such as headers being repeated or text being broken up into multiple cells.
		</p>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Sampling Methods</h2>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			Only typhoon and flooding data from 2021 to 2025 were considered because the data is most in
			line with the available flood control project data. Further, only the typhoon and flooding
			data which were available via the Asian Disaster Reduction Center and released by NDRRMC were
			considered due to their availability.
		</p>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Preprocessing</h2>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			The data sets were checked for any irrelevant or invalid data (e.g. removing data on class
			suspensions). Further, improper formatting resulting from the iLovePDF processing were also
			fixed (e.g. empty rows or columns being created).
		</p>
	</section>
</div>

<div class="mx-10">
	<h1 class="p-12 text-center font-specialelite text-6xl font-bold">Exploratory Data Analysis</h1>

	<h2 class="p-12 text-center font-specialelite text-4xl font-bold">
		<a
			href="https://colab.research.google.com/drive/1uX7GBssEao7SHqv7T1yaMRJQNvfv3msl"
			class="rounded-lg border-2 border-rhino-500 px-24 py-12 text-rhino-500 underline decoration-4 shadow-xl hover:bg-rhino-300"
		>
			Click here to go to Google Colab notebook
		</a>
	</h2>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">
			Flood Control Projects Matter More for Certain Provinces Over Others
		</h2>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			Billions are spent toward flood control projects nationwide, but creating more projects does
			not always correlate to tangible effects. The nutshell plot is a map of correlations
			describing the scale and severity of the following indicators: casualties, budget spent
			towards flood control projects, and monetary value of infrastructure damages. These
			correlations were colored in per region on a gradient of cold to warm, with cold having the
			least correlations and warm being the greatest correlations.
		</p>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Nutshell Plots</h2>
		<p class="px-0 text-center text-2xl md:px-15 lg:px-25">
			How does the amount of budget allocated to a particular area correlate with damage, such as
			casualties, injuries, and infrastructure damage, caused by flooding?
		</p>

		<section class="my-18 flex flex-col justify-center">
			<h3 class="mb-6 text-center font-specialelite text-3xl font-bold">
				Correlation between Budget and Number of Projects
			</h3>

			<div class="items-center justify-center xl:flex">
				<img
					src={asset(nutshellBudget)}
					alt="Correlation between Budget and Number of Projects"
					class="h-screen w-fit"
				/>
				<div>
					<p class="px-0 text-2xl md:px-15 lg:px-25">Notable Areas: Bulacan, NCR, and Cebu</p>
					<br />
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						Shared Trait: High density and urban economic areas
					</p>
					<br />
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						Although it is a reasonable expectation that an increase in budget would correlate with
						an increase in the number of projects within a given area, Bulacan, NCR, and Cebu stand
						out as areas with comparatively more projects in proportion to the budget given. Given
						that these areas are densely populated workplaces, the large number of projects may
						indicate smaller and more incremental projects, or alternatively, signs of embezzlement
						or corruption.
					</p>
				</div>
			</div>
		</section>

		<section class="my-18 flex flex-col justify-center">
			<h3 class="mb-6 text-center font-specialelite text-3xl font-bold">
				Correlation between Casualties and Number of Projects
			</h3>

			<div class="items-center justify-center xl:flex">
				<img
					src={asset(nutshellCasualties)}
					alt="Correlation between Casualties and Number of Projects"
					class="h-screen w-fit"
				/>

				<div>
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						Notable Areas: Benguet, Ilocos Sur, Nueva Ecija, Bulacan, Laguna, Antique, Leyte
					</p>
					<br />
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						Shared Trait: Susceptible to either floods or landslides
					</p>
					<br />
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						Most of these provinces are mountainous areas, with an increased risk of landslides
						during heavy rains. Combined with low-lying areas like Bulacan and Laguna which are
						susceptible to flash floods, these areas show a higher than average mortality rate
						compared to other provinces. Thus, these places stand out with higher correlation since
						the graph is normalized. However, the raw data does not seem to indicate that there is a
						causal relationship between the casualties and project count.
					</p>
				</div>
			</div>
		</section>

		<div class="mb-4 flex flex-col justify-center">
			<h3 class="mb-6 text-center font-specialelite text-3xl font-bold">
				Correlation between Damage and Number of Projects
			</h3>

			<div class="items-center justify-center xl:flex">
				<img
					src={asset(nutshellDamage)}
					alt="Correlation between Budget and Number of Projects"
					class="h-screen w-fit"
				/>

				<div>
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						Notable Areas: Northern Samar, Ilocos Norte, Bulacan, Batangas, Camarines Sur, Ilocos
						Sur, and La Union
					</p>
					<br />
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						Shared Trait: Are either economic areas or exit/entry points of typhoon pathways
					</p>
					<br />
					<p class="px-0 text-2xl md:px-15 lg:px-25">
						In the map, the provinces most affected in terms of damages are provinces which are
						affected by storms driven by the winds during both Amihan and Habagat. Provinces in both
						the eastern and western seafront are most affected by this along with those that are
						located more to the center of the Philippines.
					</p>
				</div>
			</div>
		</div>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Visualization I</h2>
		<p class="px-0 text-center text-2xl md:px-15 lg:px-25">
			What provinces and regions have the most flood control projects in terms of number and cost?
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			Bar charts were made to display which provinces and regions had the most flood control
			projects in terms of number and cost.
		</p>

		<section class="my-18">
			<h3 class="mb-6 text-center font-specialelite text-3xl font-bold">Number of Projects</h3>

			<div class="mb-4 flex flex-col justify-center">
				<div class="my-6 flex flex-col items-center">
					<img src={asset(regionProjects)} alt="Number of Projects per Region" />
					<p class="px-0 text-center text-xl md:px-15 lg:px-25">
						<b>Figure</b>: Number of Projects per Region
					</p>
				</div>

				<div class="my-6 flex flex-col items-center">
					<img src={asset(provinceProjects)} alt="Number of Projects per Province" />
					<p class="px-0 text-center text-xl md:px-15 lg:px-25">
						<b>Figure</b>: Number of Projects per Province
					</p>
				</div>

				<p class="px-0 text-2xl md:px-15 lg:px-25">
					In terms of number, the province with the most flood control projects is Bulacan with a
					total of 668 projects issued from 2022 to 2025. It is followed by Cebu with 414 and
					Isabela with 337. The region with the most flood control projects is Region III with a
					total of 1617 projects with over a third of its projects allocated towards Bulacan. It is
					followed by the National Capital Region with 1056 and Region V with 860.
				</p>
			</div>
		</section>

		<section class="my-18">
			<h3 class="mb-6 text-center font-specialelite text-3xl font-bold">Total Cost of Projects</h3>

			<div class="mb-4 flex flex-col justify-center">
				<div class="my-6 flex flex-col items-center">
					<img src={asset(regionProjectCosts)} alt="Total Cost of Projects per Region" />
					<p class="px-0 text-center text-xl md:px-15 lg:px-25">
						<b>Figure</b>: Total Cost of Projects per Region
					</p>
				</div>

				<div class="my-6 flex flex-col items-center">
					<img src={asset(provinceProjectCosts)} alt="Total Cost of Projects per Province" />
					<p class="px-0 text-center text-xl md:px-15 lg:px-25">
						<b>Figure</b>: Total Cost of Projects per Province
					</p>
				</div>

				<p class="px-0 text-2xl md:px-15 lg:px-25">
					In terms of cost, the province with the most flood control budget allocation is Bulacan
					with P43.7 billion allocated from 2022 to 2025. It is followed by Cebu with P26.7 billion
					and Isabela with P22.7 billion. The region with the most flood control budget allocation
					is Region III with approximately P98 Billion allocated. It is followed by the National
					Capital Region with P53.4 billion and Region V with P49.2 billion.
				</p>
			</div>
		</section>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Visualization II</h2>
		<p class="px-0 text-center text-2xl md:px-15 lg:px-25">
			How does the amount of budget allocated to a particular area correlate with damage, such as
			casualties, injuries, and infrastructure damage, caused by flooding?
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			A scatter plot was created to compare casualties, infrastructure damage, and the cumulative
			budget which has been allocated to each province, with each circle representing one province,
			and the size of the circle representing casualties.
		</p>
		<br />

		<img
			src={asset(budgetCasualtyDamage)}
			alt="Damages (in PHP) vs Budget, per Province, Emphasized Size via Casualty"
		/>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			The scatter plot has three dimensions. The x-axis represents the total budget allocated to the
			province in billions of pesos. The y-axis represents the total damages in the province in
			billions of pesos. The size of the circle represents the relative amount of casualties in that
			particular province.
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			If we look at the plot, Most of the provinces are located at the lower left portion of the
			plot. This implies that they have less budget and have less total damage and that the ratio of
			these two dimensions are close to 1. Looking further, it appears that the less budget that is
			allocated to a particular province, the more likely it will have cases of property damage
			and/or casualties. It is worth noting that despite having about the same amount of damage as
			Iloilo and Ilocos Sur, Bulacan has significantly more allocated budget and is located at the
			furthest end of the x-axis. This can be attributed to the province's increased susceptibility
			to flooding due to its geography.
		</p>
	</section>

	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Hypothesis Testing</h2>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			Linear regression was used for hypothesis testing because the independent variable, cumulative
			budget allocated to flood control projects, and the dependent variable, infrastructure damage,
			are both quantitative. Regression was done where the budgets and infrastructure damage across
			all provinces were aggregated. In total, there were also 12 data points here corresponding to
			the 12 weather incidents. Regression found a p-value of 0.1996 which led to the hypothesis NOT
			being rejected.
		</p>
		<br />
		<img
			src={asset(hypothesis)}
			alt="Cost of Infrastructure Damage vs Cumulative Budget for All Provinces"
		/>
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			Though the null hypothesis was not rejected, this does not necessarily mean that it does not
			stand, as failing to reject the null hypothesis does not mean the original hypothesis is true.
			The actual result is hence more nuanced. Real life experiences of Filipinos, in particular,
			point to typhoons and flooding perhaps worsening over time. Moreover, the above graph visually
			shows that some of the most extreme weather events actually occurred when the cumulative
			budget had already reached its current peak. Thus, even if projects do reduce damage and
			casualties, the researchers believe that the actual effect is insufficient for how much budget
			is put in.
		</p>
	</section>
</div>

<div class="mx-10">
	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">
			Connection to Socio-economic Impacts of the Philippines
		</h2>

		<p class="px-0 text-2xl md:px-15 lg:px-25">
			As discussed previously, the Philippines is one of the most disaster-prone countries in the
			world. In theory, flood control projects should be a necessary component of a comprehensive
			disaster plan of the nation. But the data gathered by the group point to anomalies which bar
			these projects from being effective.
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			Particularly, the data from the nutshell plot points to some provinces having high
			correlations between number of projects and damages or casualties, which is the reverse of
			what is expected. Similarly, the graph for visualization 2 shows that some outliers like
			Bulacan have high total project budgets while still maintaining high casualties.
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			The fact that these data points are anomalous may point to corruption or ghost projects, which
			are well-documented in the news. At the very least, if these projects are real projects, then
			the data point to them being ineffective and failing to achieve their expected results despite
			being allocated millions to billions in budget.
		</p>
	</section>
</div>

<div class="mx-10">
	<section class="my-18">
		<h2 class="mb-6 text-center font-specialelite text-4xl font-bold">Conclusion</h2>

		<p class="px-0 text-2xl md:px-15 lg:px-25">
			With the data gathered in the project, money alone cannot resolve the vulnerabilities present
			within the different regions of the Philippines. And despite an increase in the number of
			projects to address this yearly, the amount of damage remains the same proportionally. It
			shows that the country is either stuck in a process of rebuilding and recovering from storms,
			or that the money put in the projects are not at all effective in abating the effects of
			natural disasters.
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			The study faces limitations. Although the flood control project data is extensive, it only
			covers projects from 2022 to 2025. Similarly, the typhoon and flooding data only covered 12
			major weather events from 2021 to 2025. Extending the data to cover smaller weather events and
			increasing the duration will give a better picture of how they relate to each other.
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			Additionally, flooding and typhoons are complex phenomena which are influenced by many
			factors. Future studies can also take into human activities like mining, reclamation, and
			urban planning as well as other phenomena like climate change and pollution to give a more
			nuanced picture.
		</p>
		<br />
		<p class="px-0 text-2xl md:px-15 lg:px-25">
			For Filipinos nationwide, this points to a greater need for transparency and accountability
			from the government itself to answer how exactly the budget is being used and why these
			projects fail. Only through this can genuine disaster preparation and responses be achieved in
			the country.
		</p>
	</section>
</div>

<div class="mx-10">
	<section class="my-18">
		<h1 class="p-12 text-center font-specialelite text-6xl font-bold">About Us</h1>

		<div class="flex items-center justify-center">
			<Member
				name="Eriene Galinato"
				github="galierie"
				description="Eriene is a 3rd year computer science student from UP Diliman's Department of Computer Science who loves software development."
			></Member>
			<Member
				name="Sidney Lance Fernando"
				github="slcfernando"
				description="Lance is a 3rd year computer science student interested in software dev, writing, and running."
			></Member>
			<Member
				name="Daniel Dean Ognita"
				github="Orion2304"
				description="Dean is a 3rd year student of BS Computer Science with interests in the following fields: Gaming, Optimization, and The Fine Arts."
			></Member>
			<Member
				name="Gabriel Ian Carl Matias"
				github="geybb"
				description="Gabe is a 3rd year in the BS Computer Science degree program who loves music, gaming, and everything in between."
			></Member>
		</div>
	</section>
</div>

<div class="mx-10">
	<section class="my-18">
		<h1 class="p-12 text-center font-specialelite text-6xl font-bold">References</h1>

		<div class="pl-6">
			<p class="-indent-6">
				Castro, P. (2024, October 24). <i
					>Philippines races to reach stranded as storm's death toll rises</i
				>. Phys.org.
				<a
					target="_blank"
					href="https://phys.org/news/2024-10-philippines-stranded-storm-death-toll.html"
					class="text-rhino-500 underline"
					>https://phys.org/news/2024-10-philippines-stranded-storm-death-toll.html</a
				>
			</p>
			<p class="-indent-6">
				Bacelonia, W. (2025, August 19). <i
					>Senate probe on flood control bares ghost projects, favoritism.</i
				>
				Philippine News Agency.
				<a
					target="_blank"
					href="https://www.pna.gov.ph/articles/1256868"
					class="text-rhino-500 underline">https://www.pna.gov.ph/articles/1256868</a
				>
			</p>
			<p class="-indent-6">
				Bündnis Entwicklung Hilft. (2025, September 25). <i>The WorldRiskReport.</i>
				WeltRisikoBericht.
				<a
					target="_blank"
					href="https://weltrisikobericht.de/worldriskreport/"
					class="text-rhino-500 underline">https://weltrisikobericht.de/worldriskreport/</a
				>
			</p>
			<p class="-indent-6">
				Du, S. (2025, August 18). <i>What's a flood control project, anyway?</i> Rappler.
				<a
					target="_blank"
					href="https://www.rappler.com/newsbreak/iq/what-is-flood-control-project/"
					class="text-rhino-500 underline"
					>https://www.rappler.com/newsbreak/iq/what-is-flood-control-project/</a
				>
			</p>
			<br />
		</div>
	</section>
</div>
