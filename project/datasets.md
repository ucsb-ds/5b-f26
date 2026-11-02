---
layout: default
title: "Project"
nav_order: 9
has_children: true
---

# **Data Sources for Independent Data Science Projects**

Disclosure: I (Phill Conrad) used Claude AI to produce the first draft of the lists of data sources below; I then hand edited it and
did further curation.   The prompts I used are listed at the end of the page.

# **Before you start: authenticity and provenance**

Your project must use **authentic, real-world data** (not synthetic or simulated data made for teaching), and you must be able to state its **provenance**: who collected it, how, when, and where you got it.

For any dataset, you should be able to answer these questions in your write-up:

1. **Who collected it?** Name an agency, organization, or research team, not "Kaggle" or "the internet."

2. **How was it collected?** For example a survey, sensors, administrative records, or web scraping.

3. **When does it cover, and when did you download it?** Portals update and revise data, so record your download date (and the version, if there is one).

4. **What is the exact URL** of the file or API you used?

5. **Is there documentation?** Look for a data dictionary, codebook, or methodology page. If you can't find one, treat that as a warning sign.

6. **Is it original or a copy?** If it was reposted (Kaggle, GitHub, a class website), trace it back to the original publisher and cite that.

**Legend used below**

* ✅ **Primary source**: the organization that collected the data publishes it, and provenance is usually easy to establish.

* ⚠️ **Provenance caveat**: an aggregator, a repost, or user-contributed. Trace each dataset back to its original source before you use it.

* 🔒 **Free registration required**: plan for possible approval delays and data-use agreements.

# **Finding data (search tools and aggregators)**

* ⚠️ [Kaggle](https://www.kaggle.com/datasets): A large data science community. Beyond hosting thousands of datasets, it includes Notebooks (code samples) showing how others cleaned and analyzed the same data. **Caution:** anyone can upload to Kaggle. Many datasets are unattributed reposts, scraped data with no stated method, or **synthetic data** (often labeled "synthetic," "generated," "simulated," or "for practice"). Prefer datasets uploaded by the original organization, or ones that link to an original source you can download yourself. A high "usability" score measures how complete the metadata is, **not** whether the data is authentic.

* ⚠️ **AI assistants (Claude, Gemini, ChatGPT, etc.)**: Useful for brainstorming project ideas, suggesting which agency might collect a given kind of data, and helping you navigate a confusing government site. **However:**

  * **Do not use AI to generate data for this project.** AI-generated data is synthetic and does not meet the authenticity requirement.

  * AI tools can **invent URLs, dataset names, and variable definitions** that sound plausible but don't exist. Visit and verify every link and every claim about the data yourself.

  * Never cite the AI as the source of your data. Cite the original publisher.

* [Google Dataset Search](https://datasetsearch.research.google.com/): A search engine for datasets across the web. It's a good place to start, but check where each result actually comes from.

* ✅ [TidyTuesday](https://github.com/rfordatascience/tidytuesday): A weekly real-world dataset from the R community. Each one is already cleaned, comes with a data dictionary, and **links to its original source**, which makes provenance easy. The data is good for Python users too.

* ⚠️ [Data Is Plural](https://www.data-is-plural.com/): A long-running newsletter by a journalist that collects unusual, real datasets, with a searchable archive. It links to the original sources.

* **Your campus library.** Research data librarians can help you find and get access to datasets, including licensed ones your university already pays for, such as ICPSR (below).

# **Global and academic repositories**

* ⚠️ [UCI Machine Learning Repository](https://archive.ics.uci.edu/): A classic resource in academia. It hosts curated, well-documented datasets labeled for classification, regression, and clustering. **Caveats:** many datasets are decades old and heavily overused (Iris, Adult, Wine). Some are **simulated or artificially constructed** (check each dataset's description), and some have weak documentation about how they were collected. Read the "Dataset Information" and citation sections carefully, and favor datasets that cite a paper or an originating organization.

* ⚠️ [Our World in Data](https://ourworldindata.org/): Focuses on "large-scale global problems." The data is very clean, frequently updated, and gives deep historical context on health, energy, and poverty. **Note:** OWID is an **aggregator**. Every chart has a "Sources" tab that names the underlying data (World Bank, WHO, UN, and so on). Cite both OWID and the original source, and be aware that some series are OWID's own estimates or combinations of several sources.

* ✅🔒 [Pew Research Center](https://www.pewresearch.org/datasets/): Excellent for students interested in how demographics and attitudes (on politics, technology, religion) shift over time. You need a free account to download. Datasets are usually released **months or years after** the reports. You must use the **survey weights** in the codebook to get correct results, and the raw files are often in SPSS format (pyreadstat or R's haven can read them).

* ⚠️ [UN Data](https://data.un.org/): A large clearinghouse of international statistics. A good place for country-level comparisons on trade, education, and human rights. Each series cites the UN agency it comes from. For the most current data, it's often better to go directly to that agency (see below).

* ✅ [data.europa.eu (official portal for European data)](https://data.europa.eu/en): Gives access to open data published by EU institutions and national governments, covering everything from economics to geography. Quality varies a lot because it's a catalog of many publishers.

* ✅ [Eurostat](https://ec.europa.eu/eurostat/data/database): The EU's official statistics office. Comparable statistics across EU member states, with good metadata.

* ✅ [World Bank Open Data](https://data.worldbank.org/): The World Development Indicators cover about 1,400 indicators for 200+ countries back to 1960\. There are easy Python and R packages (wbgapi, WDI). Watch for missing years in low-income countries.

* ✅ [OECD Data Explorer](https://data-explorer.oecd.org/): High-quality comparisons among wealthier countries on education, health, wages, taxes, and the environment.

* ✅ [IMF Data](https://data.imf.org/): Macroeconomics, exchange rates, government debt, and the World Economic Outlook.

* ✅ [WHO Global Health Observatory](https://www.who.int/data/gho): Global health statistics such as life expectancy, disease burden, and immunization.

* ✅ [FAOSTAT](https://www.fao.org/faostat/): The UN Food and Agriculture Organization's data on agriculture, food production, land use, and food security.

* ✅ [UNESCO Institute for Statistics](https://uis.unesco.org/): Global education data on enrollment, literacy, and spending.

* ✅ [ILOSTAT](https://ilostat.ilo.org/): International labor statistics on employment, wages, and working conditions.

* ✅ [World Values Survey](https://www.worldvaluessurvey.org/): Survey of attitudes and values in about 100 countries over several decades. Download requires a short registration form. It's a good complement to Pew for international students.

* ✅ [V-Dem](https://v-dem.net/): Expert-coded measures of democracy for every country back to 1789, with extensive codebooks.

* ✅ [GBIF](https://www.gbif.org/): Over a billion biodiversity occurrence records (where species were observed). Every download gets a **DOI**, which makes provenance excellent. Note that observations are collected opportunistically and cluster near cities and roads.

* ✅ [USGS Earthquake Catalog](https://earthquake.usgs.gov/earthquakes/search/): Every recorded earthquake worldwide, downloadable as CSV. There are many California events.

* ✅ [NASA Earthdata](https://www.earthdata.nasa.gov/) and [Copernicus Climate Data Store](https://cds.climate.copernicus.eu/) 🔒: Satellite and climate data. Powerful, but the file formats (NetCDF, HDF) have a learning curve. They're best for students comfortable with gridded data.

* ⚠️ [OpenStreetMap](https://www.openstreetmap.org/) (via [Overpass Turbo](https://overpass-turbo.eu/) or the Python package osmnx): Crowd-sourced map data covering roads, buildings, and points of interest. It's real data, but completeness varies by location, so acknowledge that in your project.

* ✅🔒 [ICPSR](https://www.icpsr.umich.edu/): A huge archive of social science research data with excellent codebooks and citation information. Many universities (including the UC system) are members, so sign in with your campus account. Some datasets are restricted.

* ⚠️ [Harvard Dataverse](https://dataverse.harvard.edu/) and [Zenodo](https://zenodo.org/): Repositories where researchers deposit the data behind published papers. Each deposit has a DOI and usually a link to the paper, which is good for provenance. Quality and documentation vary from one deposit to the next.

* ✅🔒 [IPUMS](https://www.ipums.org/): Harmonized census and survey microdata (individual-level records) for the U.S. and more than 100 other countries. It's free for students after registration, and it's one of the best sources for studying population, migration, and work.

* **National statistics offices (good for international students).** Most countries publish official data, sometimes in English. Examples: [Statistics Canada](https://www.statcan.gc.ca/), [UK ONS](https://www.ons.gov.uk/), [India Open Government Data](https://www.data.gov.in/), [China National Bureau of Statistics](https://www.stats.gov.cn/english/), [Japan e-Stat](https://www.e-stat.go.jp/en), [Korea KOSIS](https://kosis.kr/eng/), [Mexico INEGI](https://www.inegi.org.mx/), and [Brazil IBGE](https://www.ibge.gov.br/en/). A project that compares your home country with California can be very compelling.

# **U.S. government and public portals**

* ⚠️ [Data.gov](https://data.gov/): The U.S. government's catalog of open data. It lists hundreds of thousands of datasets, ranging from climate sensor logs to Small Business Administration loans. **Note:** Data.gov is mostly a **catalog**. Follow the link to the agency that publishes the data, and cite that agency. Some links are dead or point to outdated versions.

* ✅ [U.S. Census Bureau (data.census.gov)](https://data.census.gov/) and the [Census API](https://www.census.gov/data/developers.html): Demographics, income, housing, and commuting data down to the census-tract level. The **American Community Survey (ACS)** is the workhorse. **Tip:** ACS estimates come with **margins of error**, and for small areas (individual tracts, small towns) those margins can be large, so report them. The Python package censusdata and the R package tidycensus make access much easier.

* ✅ [Bureau of Labor Statistics](https://www.bls.gov/data/): Employment, wages, prices (CPI), and occupations.

* ✅ [FRED (St. Louis Fed)](https://fred.stlouisfed.org/): More than 800,000 economic time series, each clearly attributed to its original source agency. Very easy to download, and there's an API.

* ✅ [CDC data portal](https://data.cdc.gov/) and [CDC WONDER](https://wonder.cdc.gov/): Mortality, births, and disease surveillance. Note that WONDER **suppresses small counts** (fewer than 10\) for privacy.

* ✅ [NHANES](https://www.cdc.gov/nchs/nhanes/): A national health and nutrition survey that includes physical exam and lab measurements. It requires correct use of survey weights.

* ✅ [College Scorecard](https://collegescorecard.ed.gov/data/) and [IPEDS](https://nces.ed.gov/ipeds/): Data on every U.S. college, including costs, graduation rates, and earnings after graduation. Students tend to find this topic engaging.

* ✅ [EPA Air Quality Data](https://www.epa.gov/outdoor-air-quality-data): Daily measurements from air monitors, including many California stations.

* ✅ [NOAA Climate Data Online](https://www.ncei.noaa.gov/cdo-web/): Historical weather station data. Requesting large orders requires a free token.

* ✅ [Bureau of Transportation Statistics](https://www.transtats.bts.gov/): Flight on-time performance for every domestic flight (LAX, SFO, and SAN included). These are large files, which makes them good practice for working with big data.

* ✅ [NHTSA FARS](https://www.nhtsa.gov/research-data/fatality-analysis-reporting-system-fars): Every fatal traffic crash in the U.S. since 1975\.

* ✅ [FBI Crime Data Explorer](https://cde.ucr.cjis.gov/): National crime statistics. **Caveat:** the FBI switched to a new reporting system (NIBRS) in 2021, and many agencies did not report that year, so comparisons across that transition are tricky.

* ✅ [FEC campaign finance](https://www.fec.gov/data/): Federal political contributions and spending.

* ✅ [U.S. Energy Information Administration](https://www.eia.gov/opendata/): Electricity generation, energy prices, and fuel use by state.

* ✅ [USDA NASS Quick Stats](https://quickstats.nass.usda.gov/): Agricultural data by county. California is the country's top agricultural state.

* ⚠️ [FiveThirtyEight data (GitHub archive)](https://github.com/fivethirtyeight/data): Notable because it provides the raw data behind data journalism, so students can try to replicate the results of published news articles. **Note:** ABC News shut down FiveThirtyEight in March 2025\. The GitHub archive is no longer updated, and the old data.fivethirtyeight.com address may not work. Each folder's README describes the source. Similar repositories from active newsrooms include [The Pudding](https://github.com/the-pudding/data), [BuzzFeed News](https://github.com/BuzzFeedNews) (also archived), and the [LA Times Data Desk](https://github.com/datadesk), which has a lot of California data.

# **California: state agencies**

* ✅ [California Open Data (data.ca.gov)](https://data.ca.gov/): The central hub for state-level data, such as electric vehicle registrations, water quality reports, and state park usage. Each dataset lists its publishing department, so cite the department as well as the portal.

* ✅ [CalHHS Open Data](https://data.chhs.ca.gov/): Health and human services data covering hospitals, births and deaths, Medi-Cal, and COVID-19.

* ✅ [HCAI (Department of Health Care Access and Information)](https://hcai.ca.gov/data/): Hospital finances, utilization, and patient outcomes.

* ✅ [CalEnviroScreen (OEHHA)](https://oehha.ca.gov/calenviroscreen): Pollution burden and population vulnerability scores for every census tract in California. A very good dataset for environmental justice projects, with excellent documentation.

* ✅ [California Department of Education: DataQuest](https://dq.cde.ca.gov/dataquest/) and [downloadable files](https://www.cde.ca.gov/ds/): Enrollment, test scores, graduation rates, and chronic absenteeism by school and district. Note that values are suppressed for small groups.

* ✅ [UC Information Center](https://www.universityofcalifornia.edu/about-us/information-center): University of California admissions, enrollment, and graduation data by campus and demographic group. Students relate easily to this data.

* ✅ [CA Department of Finance: Demographics](https://dof.ca.gov/forecasting/demographics/): Official state population estimates and projections by county and city.

* ✅ [EDD Labor Market Information](https://labormarketinfo.edd.ca.gov/): California employment, unemployment, and wages by county and industry.

* ✅ [CA DOJ OpenJustice](https://openjustice.doj.ca.gov/): Crime, arrests, deaths in custody, use of force, and **RIPA police stop data**, which records every stop by large agencies with demographics. This is a large, rich dataset.

* ✅ [CAL FIRE incidents](https://www.fire.ca.gov/incidents) and [FRAP fire perimeters](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program): Wildfire history, with GIS perimeters going back more than a century.

* ✅ [California Air Resources Board (AQMIS)](https://www.arb.ca.gov/aqmis2/aqmis2.php): Air quality monitoring data from across the state.

* ✅ [California Data Exchange Center (CDEC)](https://cdec.water.ca.gov/): Reservoir levels, snowpack, river flows, and precipitation. Good for drought and water projects.

* ✅🔒 [CIMIS](https://cimis.water.ca.gov/): Weather stations aimed at agriculture, with evapotranspiration data.

* ✅ [California Energy Commission](https://www.energy.ca.gov/data-reports): Zero-emission vehicle sales, EV chargers, power plants, and energy use.

* ✅🔒 [Caltrans PeMS](https://pems.dot.ca.gov/): Traffic sensor data at 5-minute resolution for California freeways. These are very large datasets.

* ✅🔒 [TIMS (UC Berkeley Transportation Injury Mapping System)](https://tims.berkeley.edu/): Geocoded crash data derived from California Highway Patrol records. Crash data is also on data.ca.gov.

* ✅ [CA Secretary of State: election results](https://www.sos.ca.gov/elections/prior-elections/statewide-election-results) and [Cal-Access campaign finance](https://www.sos.ca.gov/campaign-lobbying/cal-access-resources): Statewide results by county. **Warning:** raw Cal-Access data is very messy, which makes it a good data-cleaning challenge.

* ✅🔒 [California Health Interview Survey (CHIS)](https://healthpolicy.ucla.edu/our-work/california-health-interview-survey-chis): The largest state health survey in the U.S., run by UCLA. Public-use files are free after registration, and the AskCHIS tool makes quick tables. It requires the use of survey weights.

# **California: city, county, and regional portals**

* ✅ [Open Data LA](https://data.lacity.org/): Detailed city data for Los Angeles, including 311 service requests, building permits, and LAPD crime data. **Caveat:** LAPD changed its crime-reporting system in 2024, so the long-running "Crime Data from 2020 to Present" dataset stopped being updated consistently. Read the dataset notes before you analyze trends.

* ✅ [LA County Open Data](https://data.lacounty.gov/): County-wide data on health, public safety, property assessment, and more.

* ✅ [DataSF (San Francisco)](https://datasf.org/opendata/): One of the most mature city portals in the world, with very high-quality data on transit (Muni), housing, and urban forestry. Also see SF Police incident reports and building permits.

* ✅ [San Diego Open Data](https://data.sandiego.gov/): A great resource for Southern California analysis, including parking meter data, fire incidents, and business licenses. Also see [SANDAG](https://www.sandag.org/data-and-research) for regional demographics and transportation.

* ✅ Other city portals: [San José](https://data.sanjoseca.gov/), [Oakland](https://data.oaklandca.gov/), [Sacramento](https://data.cityofsacramento.org/), and [Long Beach](https://data.longbeach.gov/).

* ✅ Transit ridership: [BART](https://www.bart.gov/about/reports/ridership) (station-to-station trips by hour) and [LA Metro](https://opa.metro.net/MetroRidership/).

* **Tip:** Many city portals run on the same platform (Socrata), which provides a uniform API. The Python package sodapy works across all of them, and the same code often works for several cities. Comparing cities can make for a strong project.

# **Other real data with California coverage (read the caveats)**

* ⚠️ [Inside Airbnb](https://insideairbnb.com/): Scraped Airbnb listings for Los Angeles, San Francisco, San Diego, Oakland, Santa Clara County, Santa Cruz, and many cities worldwide. The data is real and the methodology is documented, but it comes from an advocacy project rather than Airbnb, and it captures snapshots in time. Say so in your write-up.

* ⚠️ [Zillow Research Data](https://www.zillow.com/research/data/) and [Redfin Data Center](https://www.redfin.com/news/data-center/): Housing prices and rents by ZIP code and metro area. **Note:** indices such as the Zillow Home Value Index are **modeled estimates**, not raw sale prices. They are fine to use, but describe them accurately and cite the methodology page.

# **More sources by topic: sports, entertainment, health, and more**

The same legend applies: ✅ primary source, ⚠️ provenance caveat, 🔒 free registration required.

**Three extra cautions for these topics:**

* **Terms of service.** Many sports and entertainment websites prohibit automated scraping. Use an official download or API when one exists, and read the site's terms before writing a scraper. "I scraped it" is not a complete provenance statement. Say which pages you scraped, when, and with what tool.

* **APIs change.** Companies often restrict or shut down their APIs. (For example, Reddit and X/Twitter sharply limited free data access in 2023, and Spotify removed its "audio features" data for new apps in late 2024.) Confirm that an API works for you before building a project around it.

* **Data about people.** Analyzing **your own** personal data, such as fitness tracker or streaming history, is authentic and has clear provenance, because you are the source. Collecting new data from **other people** (for example, surveying classmates) may require approval from your campus Institutional Review Board (IRB), so ask your instructor first.

# **Sports**

* ✅ [Baseball Savant (MLB Statcast)](https://baseballsavant.mlb.com/): Official pitch-by-pitch and batted-ball tracking data, including exit velocity and spin rate. The Python package pybaseball makes downloading easy. Good for Dodgers, Giants, Angels, and Padres fans.

* ✅ [Lahman Baseball Database](https://sabr.org/lahman-database/): Season-level baseball statistics back to 1871, now maintained by SABR (the Society for American Baseball Research). Well documented and easy to cite.

* ✅ [Retrosheet](https://www.retrosheet.org/): Play-by-play records for historical MLB games, compiled by volunteers from official scoresheets. Retrosheet requires a specific citation notice, which is posted on the site.

* ⚠️ [nflverse](https://github.com/nflverse): NFL play-by-play data back to 1999, maintained by a community of analysts. It's widely used and well documented, but it isn't official NFL data, so cite the nflverse project and its stated sources. Works in Python (nfl\_data\_py) or R (nflreadr).

* ⚠️ [nba\_api](https://github.com/swar/nba_api): A Python package that pulls data from NBA.com's statistics site. It's an **unofficial** interface and sometimes breaks when NBA.com changes. Cite NBA.com as the data source.

* ⚠️ [Sports Reference sites](https://www.sports-reference.com/) ([Basketball](https://www.basketball-reference.com/), [Pro Football](https://www.pro-football-reference.com/), [FBref soccer](https://fbref.com/), [Hockey](https://www.hockey-reference.com/), and [College](https://www.sports-reference.com/cbb/)): Huge, reliable statistics archives. **However,** their terms limit bulk scraping and they block heavy automated traffic. Use the built-in "Share & Export → Get table as CSV" option to copy individual tables. Some data shown on these sites is licensed from third parties and can change or disappear.

* ✅ [StatsBomb Open Data](https://github.com/statsbomb/open-data): Free, detailed event data (every pass, shot, and tackle) for selected soccer competitions, including men's and women's World Cups, the Champions League, and many seasons featuring Lionel Messi. Strong appeal for international students. Requires attribution to StatsBomb (now part of Hudl).

* ⚠️ [Tennis Abstract Match Charting Project](https://github.com/JeffSackmann/tennis_MatchChartingProject): Shot-by-shot records of thousands of men's and women's professional matches, charted by volunteers. It covers a selected set of matches rather than every match, and it's licensed for non-commercial use (CC BY-NC-SA), which is fine for class projects. **Note:** the same author's widely copied ATP and WTA match-results repositories are no longer on GitHub. Kaggle copies of them now lack a live original source to cite, so check carefully before using them.

* ✅ [Cricsheet](https://cricsheet.org/): Ball-by-ball data for international and franchise cricket, including the IPL. Very appealing to students from South Asia, the UK, Australia, and the Caribbean.

* ⚠️ [Jolpica F1 API](https://github.com/jolpica/jolpica-f1) and the [FastF1](https://docs.fastf1.dev/) Python package: Formula 1 results back to 1950, plus lap times and car telemetry for recent seasons. Jolpica is the community replacement for the Ergast API, which shut down at the end of 2024\. Both are community projects, so cite them along with Formula 1 as the original source.

* ✅ [Olympedia](https://www.olympedia.org/): The most complete historical record of Olympic athletes and results, maintained by Olympic historians. Many Kaggle "Olympics" datasets are older scrapes of this kind of data, so cite Olympedia instead.

* ✅ [Lichess Open Database](https://database.lichess.org/): Every rated game played on Lichess, billions of chess games in total, released monthly under a public domain license. These are very large files and need careful handling, which makes them good practice for working with big data.

* **Tip:** Your own campus athletics website usually publishes season statistics and results for each team. That can make a fun, local project.

# **Movies, TV, music, books, and games**

* ✅ [IMDb Non-Commercial Datasets](https://developer.imdb.com/non-commercial-datasets/): Official files from IMDb covering titles, ratings, cast and crew, and episodes for millions of titles. They may be used for personal and non-commercial purposes, which covers class projects.

* ⚠️ [TMDB (The Movie Database) API](https://developer.themoviedb.org/): Free with an API key. Covers budgets, revenue, genres, and posters for movies worldwide. The data is user-contributed, so budget and revenue figures are often missing or unverified. TMDB's terms require attribution.

* ✅ [Netflix Top 10](https://www.netflix.com/tudum/top10): Official weekly Top 10 lists for films and TV, globally and **by country**, downloadable as files. Netflix also publishes twice-yearly "What We Watched" engagement reports covering nearly every title. Good for comparing tastes across countries.

* ✅ [MusicBrainz](https://musicbrainz.org/doc/MusicBrainz_Database): An open encyclopedia of music with artists, releases, and recordings, placed in the public domain. It's maintained by volunteers, so coverage varies.

* ⚠️ [Spotify Charts](https://charts.spotify.com/): Daily and weekly top songs by country, downloadable as CSV after a free login. **Note:** the Spotify Web API no longer gives new apps "audio features" (danceability, energy, and so on). Older Kaggle datasets with those columns came from before the change, so trace and cite their original collection date and method.

* ✅ **Your own streaming history.** Spotify, Netflix, YouTube/Google, Apple, and most other services let you request a copy of your personal data. The right to request it comes from privacy laws such as California's CCPA and the EU's GDPR, and requests take anywhere from a few days to a few weeks. This is authentic data with perfect provenance. Just remember a sample of one person limits what you can conclude.

* ✅ [Open Library data dumps](https://openlibrary.org/developers/dumps): Bulk data on millions of books and authors from the Internet Archive.

* ✅ [UCSD Book Graph (Goodreads)](https://mengtingwan.github.io/data/goodreads.html) and [Julian McAuley's datasets at UC San Diego](https://cseweb.ucsd.edu/~jmcauley/datasets.html): Research datasets of real reviews and ratings from Goodreads, Amazon, Steam (video games), beer and wine sites, and more. They were collected by a UC research lab and come with published papers to cite. Each page asks that you cite a specific paper.

* ⚠️ [SteamSpy](https://steamspy.com/): Ownership and playtime estimates for video games on Steam. These are **statistical estimates**, not Steam's own numbers, so describe them that way. Avoid VGChartz-style sales figures, which are largely unverified estimates.

* ⚠️ [Jikan (MyAnimeList API)](https://jikan.moe/): An unofficial API for anime and manga ratings, popularity, and genres. It has strong international appeal, but the scores are user ratings from one website's community.

* ✅ Museum collections: [The Met Open Access](https://github.com/metmuseum/openaccess) and the [Art Institute of Chicago API](https://api.artic.edu/docs/). Official museum records, with artwork dates, artists, nationalities, gender, and acquisition history. Good for questions about representation in art collections.

* ✅ [Wikipedia pageviews](https://pageviews.wmcloud.org/): Daily views for any Wikipedia article in any language back to 2015\. A clean, official way to measure public attention to a celebrity, film, team, or event.

* ⚠️ [Google Trends](https://trends.google.com/): Relative search interest over time and by region. **Caution:** values are scaled from 0 to 100, are based on a sample, and **can change slightly every time you download them.** Record the exact download date and settings, and don't treat the values as counts of searches.

# **Health, fitness, and food**

* ✅ [CDC BRFSS](https://www.cdc.gov/brfss/): A large state-level health survey covering exercise, sleep, smoking, obesity, and chronic disease, with California results. It requires survey weights.

* ✅ [CDC PLACES](https://www.cdc.gov/places/): Health estimates for every county, city, census tract, and ZIP code, covering things like physical inactivity, short sleep, and depression. **Note:** these are **model-based estimates**, not direct counts, so describe them that way.

* ✅ [County Health Rankings](https://www.countyhealthrankings.org/): Combines health outcomes and factors such as access to exercise and food for every U.S. county. Good for comparing California's 58 counties.

* ✅ [American Time Use Survey](https://www.bls.gov/tus/): How Americans actually spend their day, including sleep, exercise, screen time, and studying, broken down by age, sex, and employment. Very relatable for students.

* ✅ [CDC Youth Risk Behavior Survey (YRBS)](https://www.cdc.gov/yrbs/): High school students' physical activity, sleep, screen time, and mental health, collected nationally and by state.

* ✅ [California Physical Fitness Test results (CDE)](https://www.cde.ca.gov/ta/tg/pf/): School and district results from FITNESSGRAM. Check which years and measures are available, because the state changed how the test is given and reported after 2019\.

* ✅🔒 [IHME Global Burden of Disease](https://vizhub.healthdata.org/gbd-results/): Estimates of causes of death and disability for every country, 1990 to the present. Free registration required. These are modeled estimates with uncertainty intervals, so report the intervals.

* ✅ [PhysioNet](https://physionet.org/): Real physiological and clinical datasets, including heart rate, ECG, sleep studies, and some wearable-device data. Some datasets are open, and others require credentialing and training.

* ✅ **Your own fitness tracker data.** Apple Health (export from the Health app), Fitbit, Garmin, Strava, and similar services let you export your own steps, heart rate, sleep, and workouts. This is authentic data with clear provenance. Describe the device and its known measurement limits, since wrist-worn devices estimate many values.

* ✅ [USDA FoodData Central](https://fdc.nal.usda.gov/): Official nutrient content for hundreds of thousands of foods, including branded products.

* ⚠️ [Open Food Facts](https://world.openfoodfacts.org/data): Crowd-sourced ingredients, nutrition, and Nutri-Score data for millions of food products in more than 150 countries. Great for international comparisons, but entries are user-contributed and sometimes incomplete or wrong.

* ✅ Restaurant health inspections: several California city and county portals publish them, including [LA County](https://data.lacounty.gov/) and [DataSF](https://datasf.org/opendata/) (search for "inspections").

* ⚠️ [Yelp Open Dataset](https://business.yelp.com/data/resources/open-dataset/): Real reviews and business information for a subset of metro areas, including Santa Barbara. Yelp chose which businesses and reviews to include, so it isn't a complete or random sample. Licensed for academic use.

# **Careers, international students, and higher education**

* ✅ [H-1B and other work-visa salary data (U.S. Department of Labor)](https://www.dol.gov/agencies/eta/foreign-labor/performance): Every employer application for H-1B and other work visas, with job title, location, and offered salary. Very relevant for international students and anyone curious about tech salaries in California.

* ✅ [USCIS H-1B Employer Data Hub](https://www.uscis.gov/tools/reports-and-studies/h-1b-employer-data-hub): H-1B approvals and denials by employer, state, and city.

* ✅ [SEVIS by the Numbers (ICE)](https://www.ice.gov/sevis/whats-new): Annual reports on international students in the U.S., by country of origin, state, and field of study.

* ⚠️ [IIE Open Doors](https://opendoorsdata.org/): The standard source for international student enrollment and U.S. students studying abroad. It mostly publishes summary tables, and the data comes from a survey of institutions, not government records.

* ✅ [NSF NCSES](https://ncses.nsf.gov/): Data on degrees, PhDs, and the science and engineering workforce, including by citizenship.

* ✅ [Stack Overflow Developer Survey](https://survey.stackoverflow.co/): Annual global survey of tens of thousands of programmers, covering salaries, languages, AI tool use, and remote work. Full responses and codebooks are available. Respondents chose to take part, so it isn't a random sample of all developers.

# **Travel, transportation, and the outdoors**

* ✅ [National Park Service visitor statistics](https://irma.nps.gov/Stats/): Monthly visits to every national park, including Yosemite, Joshua Tree, Sequoia, and Channel Islands.

* ✅ Bike share trip data: [Bay Wheels (San Francisco Bay Area)](https://www.lyft.com/bikes/bay-wheels/system-data) and [Metro Bike Share (Los Angeles)](https://bikeshare.metro.net/about/data/). Every trip, with start and end stations and times. Good for spatial and time-of-day analysis.

* ✅ [LAX statistics (Los Angeles World Airports)](https://www.flylax.com/lax-statistics): Monthly passenger and flight counts at LAX. Also see the BTS flight data in the U.S. section above.

* ✅ [NYC Taxi & Limousine Commission trip records](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page): More than a billion taxi and rideshare trips. It's a New York dataset, but a classic for learning to work with big data.

* ✅🔒 [eBird (Cornell Lab of Ornithology)](https://ebird.org/data/download): Bird sightings from citizen scientists worldwide. Download requires a free request form. Sightings cluster where birders go, so account for that.

* ✅ [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/): Every confirmed planet outside our solar system, maintained at Caltech. Also see NASA's [Meteorite Landings data](https://data.nasa.gov/).

# **Politics, society, and fun miscellany**

* ✅ [MIT Election Data \+ Science Lab](https://electionlab.mit.edu/data): Cleaned U.S. election results (presidential, congressional, state, and county), with clear documentation.

* ✅ [Voteview](https://voteview.com/data): Every roll-call vote in Congress, with ideology scores for every member.

* ⚠️ [The Economist's Big Mac Index](https://github.com/TheEconomist/big-mac-data): Burger prices in about 70 countries as a light-hearted measure of exchange rates. The methodology is published on GitHub. Fun for international comparisons.

* ✅ Animal shelter intakes and outcomes: several city portals publish these, including [Long Beach](https://data.longbeach.gov/). They support questions like "which animals get adopted fastest?"

* ✅ [Project Gutenberg](https://www.gutenberg.org/): More than 70,000 public-domain books, good for text-analysis projects. Version details matter, so cite the specific edition (eBook number) you used.


  


### Prompts used:  Prompt 1: Here is a list of source for data sets for doing independent student data science projects.

What I'm asking for from you is to update this list with any additional sources you can find, and to update the descriptions with any advice or comments you think would be helpful to undergraduate students.

I'm particularly interested in finding data that pertains to California, since many of my students are from California, but I have a lot of international students as well, so global data is also interesting.

A particular issue is that the data needs to be authentic data, not "synthetic data" (made up data) that is designed for student projects, but does NOT reflect real world conditions.

I also want to be sure that the students can provide the provenance for their data, so sources that lack this need to be noted with that caveat.  
General & AI-Assisted Research

(After this, I pasted the list of topics used in S26.)

Prompt 2: This is excellent.  Can we add some sources for sports data, entertainment data, health and fitness data, and any other topics that would appeal to undergraduate US domestic and international students?  

