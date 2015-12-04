Analyzing and Modernizing Victoria City Council's Communications: An Interim Report
===================
# Table of Contents
1. [Introduction](#introduction)
2. [Related Work](#related-work)
	1. [CSCW in Meetings](#cscw-in-meetings)
	2. [Local Government Innovation](#local-government-innovation)
	3. [History of CSCW Use in Government](#history-of-cscw-use-in-government)
		1. [Cuparla](#cuparla)
			1. [Creating Cuparla](#creating-cuparla)
			2. [Cuparla Software Design](#cuparla-software-design)
			3. [Methodology used in developing Cuparla](#methodology-used-in-developing-cuparla)
			4. [Evaluation of Cuparla](#evaluation-of-cuparla)
		2. [E-government](#e-government)
			1. [Reasons behind innovating with e-government](#reasons-behind-innovating-with-e-government)
			2. [Methodology to evaluate use of e-government](#methodology-to-evaluate-use-of-e-government)
			3. [Implementation of e-government in Corpus Christi](#implementation-of-e-government-in-corpus-christi)
			4. [Benefits of e-government](#benefits-of-e-government)
		3. [Open Source](#open-source)
			1. [Reasons behind innovating with Open Source](#reasons-behind-innovating-with-open-source)
			2. [Transition to Open Source in Munich](#transition-to-open-source-in-munich)
			3. [Methodology to evaluate usage of Open Source](#methodology-to-evaluate-usage-of-open-source)
3. [Methodology](#methodology)
	1. [Alternatives Considered](#alternatives-considered)
	2. [Our Methodology](#our-methodology)
4. [Results](#results)
	1. [Results from City Council Meetings](#results-from-city-council-meetings)
	2. [Interview Results](#interview-results)
		1. [Communication](#communication)
		2. [Bylaw Development](#bylaw-development)
		3. [Councillor Comfort with Technology](#councillor-comfort-with-technology)
	3. [Issues Identified](#issues-identified)
5. [Conclusions](#conclusions)
6. [Impact](#impact)
7. [Appendices](#appendices)
	1. [Appendix 1: Team Roles](#appendix-1-team-roles)
		1. [Kimberlee Graham-Knight](#kimberlee-graham-knight-group-leader)
		2. [Roshni Jain](#roshni-jain-data-analysis)
		3. [Nigel Dufty](#nigel-dufty-data-collection)
		4. [Tian Geng](#tian-geng-data-analysis)
		5. [Myan Panikkar](#myan-panikkar-editor)
	2. [Appendix 2: Milestones](#appendix-2-milestones)
		1. [Status on Original Milestones](#status-on-original-milestones)
		2. [New Timeline](#new-timeline)
	3. [Appendix 3: Interview Questions](#appendix-3-interview-questions)
	4. [Appendix 4: Tools Used by Council](#appendix-4-tools-used-by-council)
8. [References](#references)

## Introduction

Given the rapid pace at which various technologies have evolved over the past few years, there exists a need to re-evaluate the current usage of technology in the public sector. In particular, there is a need for the public to ensure that their governments are using current technology to its fullest capabilities in order to better service the public. With our research, we aimed to discover what methods the city council of Victoria currently uses for facilitating collaboration and communication. This includes public council meetings as well as their internal communications. We ask three research questions in this paper:

1. What technologies already exist or are being used to help city councillors in their meetings, with respect to document sharing and communication?
2. What issues are they currently facing with their present technology?
3. How can we improve communication between city councillors?

One area in particular that we wanted to focus on was the preparation and management of council meetings via technology. Specifically, we wanted to find out what technologies are used to prepare for the city council's meetings. What software do they use to construct their meeting agendas? How do they use technology to introduce new bylaws, modify them, and then finalize them? What steps does the city take to make this process transparent to the public? Do city councillors use software or other tools during meetings to facilitate the sharing of information? How do city councillors use software to afford the opportunity for remote participation in meetings? These are all questions that we sought to answer in our study.  

One of the main reasons for conducting this study is that most of the existing research about city governments is about how to improve government-citizen relations. There have not been as many studies on how technology plays a role in governmental organization. For the studies that have been conducted, many of the more prominent studies are outdated by at least 10 years, and/or focus on municipalities located in Europe or in the United States. By conducting this study, we offer an opportunity for the municipal government of Victoria to make their current software integration status transparent to its citizens. Transparency on current practices regarding software can be healthy for growth and improvement (as seen in the open source community), since it allows for the government's citizens to critique the current technological solutions (e.g. if cheaper, equally functional alternatives are available). As well, research of this type can provide beneficial information to councillors on what they can do to improve their usage of technology. 

To accomplish this study of Victoria's municipal government, we conducted interviews with its city councillors. This was our primary source of data, as these councillors are the primary focus of this study. To augment these interviews with city councillors, we also conducted interviews with various members of the public that are affiliated with the municipal government of Victoria and one interview with a member of Sooke's city council for comparison data. Alongside these interviews, we observed public council meetings to see what their current practices are for conducting meetings with the public. 

The next section goes over the previous research done in this field and how this previous research is relevant to the research questions we are currently pursuing.

## Related Work

Before looking at previous implementations of computer-supported collaborative work (CSCW) in government settings, we need to understand some of the difficulties of integrating CSCW into meetings. We also need context for why it is important for municipal governments to want to incorporate modern CSCW into their work flow. 

### CSCW in Meetings

According to Schümmer, there are three distinct facets of designing an electronic face-to-face meeting system  [1]:

> 1. the peopleware perspective, the design of social processes that are executed by team members,
2. the generic groupware perspective for designing supportive software tools, and
3. the roomware perspective that considers the configuration of artifacts that constitute the tangible meeting space.

The following figure helps to provide a context for what Schümmer is trying to illustrate. Specifically, it shows where modern, everyday technology fits in to his model of an electronic meeting system [1]. 

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/cscw_in_meetings.png">
</p>

Arguably, the hardest facet of designing an electronic meeting system for a group is understanding their needs. To properly assess the needs of a group that needs to meet on a regular basis, one needs to observe how the group interacts in a meeting and what the group needs from their available technology to augment and improve their work flow. While many tools (both open source and proprietary) today are being rapidly developed and improved on, they are not guaranteed to meet the needs of public officials. 

Understanding Schümmer's scheme as it relates to city council is part of the motivation of our study. To ensure that our government has room to innovate, an assessment of their current technological integration and their current communication practices is necessary. 

### Local Government Innovation

Innovation is an important part of any continued collaborative group work. Walker says innovation is a core task of public institutions and that "innovation has been promoted around the world as a key tool to improve public services" [2]. This is one of the reasons we are targeting the city of Victoria with our study: public services always stand to be improved, and the city is in one of the best positions to affect this change. Ihrke notes that local governments are more likely to innovate than governments at the state or federal level because of "their small size and capacity to make decisions quickly and decisively" [3], and this is another reason as to why we are targeting the city of Victoria. While standards do exist at the provincial and federal level for regulating what technologies can be used in government organizations, municipal governments like the city of Victoria can be more receptive to change and can integrate suggestions for improvement at a much faster pace than provincial or federal bodies. 

We believe the city of Victoria would be interested in this sort of study for two reasons. The first is that by recognizing any potential shortcomings in their current practices they can quickly take steps to remedy these shortcomings; our study offers this through analysis of interviews with city officials. The second reason is that local governments tend to get a lot of pressure to "do more with less" [2] so by offering potential alternatives to the city (should they be applicable), the city can choose to shift the technologies they use and potentially lower their current costs. To help inform this decision, should we make any suggestions towards changing the software or the way they use software we will also include the cost of changing this software, where applicable. 

Before addressing how we assessed the current state of technological use in the municipality of Victoria, we need to consider what has been done before in this field of research. The following section details the history of CSCW integration with governments. 

###History of CSCW Use in Government

Here are some examples of previous attempts to integrate CSCW into government organizations. These examples are in chronological order, and attempt to focus on the processes used to research the organizations involved as well as how they built or identified what software suites would be most applicable for the given organization. In particular, we will be focusing on three case studies that have occurred over the past 20 years:

1. Cuparla (1995)
2. E-government (2001)
3. Open source (2002-2014)

Much of this research focused on _how_ these software suites were designed and implemented, alongside their benefits. However, we want to focus on _why_ these software suites were designed and _why_ they were adopted. 

####Cuparla

In 1995, a number of socio-technical projects were coming on a timely manner to improve the city council administration (in terms of effective communication). In the example of Cuparla, the developers first assessed the need for technology for support. After completing this analysis, they developed this system and then implemented it in specific municipal organizations to serve their particular needs. 

Cuparla was only adopted by a few smaller city councils in Germany, and the literature about it is limited to 5 articles, all by the same author. However, it is a case study in an early adoption of a comprehensive software suite by city council, hence its relevance to our research. 

#####Creating Cuparla

Cuparla was initially developed for the city of Stuttgart, Germany. A detailed analysis of Stuttgart city council work revealed certain characteristics of the city council's work [4]:

- Any software required to support council members needed to have functionality supporting the "any time, any place" style of meeting. This was required as council members did not have fixed office locations to prepare for city hall meetings. 
- The council members collaborated and behaved differently in different contexts. When in their respective political party groups, council members tended to be more informal and open with regards to communication. In official council meetings, they were more controlled and more formal. 
- There was no inherent structure to be followed for communication. Each member of the city council had the right to initiate communication and they had the right to involve members of the administration in any order. 
- At the time, there was minimal computer usage within the council itself. 
 
Given all this information, the developers for Cuparla aimed to satisfy three objectives. Firstly, they sought to bring effectiveness and flexibility in the work of the councils. Secondly, they wanted to provide more access to information for the council members. Finally, they aimed to reduce communication barriers between the council members and administration within the council. The software suite was launched at the end of 1995 in Stuttgart, and by fall 1997, almost every city council member was using the system. 

#####Cuparla Software Design

Cuparla was designed with the aim to support political entities. The following figure is a screenshot of the software suite's main page. As shown by the picture, this software supported many functions, including "information, communication, coordination, and collaboration [5]."

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/cuparla.jpg">
</p>

The design of this software was based on the city council's actual work procedure of using distinct *rooms* for different purposes. Each room had its own set of supported functions. Below is a partial listing of the functions supported by each room:

- **Private Room** - Here, the council member worked at home. This function was intended for an individual's work.  
- **Parliamentary Party** - Using this function, a council member had the opportunity to collaborate with their party colleagues.
- **Committees** - This function let council members collaborate between parties on particular committee issues. 
- **Library** - This function allowed any council member to have access to previously filed information. 

Any documents created in private rooms could be shared by placing them in the room that the user wished to share the document with. While this type of software design seems trivial and archaic by today's software standards, it was a historical landmark for the field of CSCW in government as there are few, if any, documented software suites that were developed for particular municipalities. Cuparla was one of the pioneers in the field of specialized government software. 

#####Methodology used in developing Cuparla

To properly evaluate the Stuttgart city council, a detailed analysis of council work was done using Needs Driven Analysis (NDA). NDA is suitable to concurrently design software and intervene in an organization in a large group environment. This type of analysis identified the need for group support, which then served as the basis for the design of Cuparla. An initial design was implemented within the council, and the developers allowed for a few months of usage before analyzing the usage and effectiveness of the software. 

Two analysis and development cycles were used to develop Cuparla. In the first cycle, Cuparla was tested by 11 city council members. The results obtained from this initial wave were then used to do a second analysis, design, implementation and evaluation phase. This second software cycle was tested on 55 of 56 active city council members. By the end of the second cycle, a field test of Cuparla was performed on the small city of Kornwestheim, in order to determine the effectiveness of the tool in a different environment [4]. 

##### Evaluation of Cuparla

Evaluation of cuparla was done on five sets of criteria and four levels of aggregation [6]. The criteria used to evaluate Cuparla were **cost, time, quality, flexibility,** and **human situation**. The four levels of aggregation used to distinct the user groups involved were the **individual**, the **group**, the **process**, and the **organization**. As seen in the following figure, these criteria were aligned to create a 4x5 matrix for easier evaluation. Any notes made in the evaluation were attributed only to the lowest applicable level. For instance, the costs of a server would be attributed to the **group** as that is the lowest level in direct need of the server, whereas a PC in an office is attributed to the **individual** level. 

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/Evaluation of Curparla.png">
</p>

Using a matrix of this sort seemed to be an effort to reduce the redundancy in data obtained from the evaluation. We did not be using such a method in our study to evaluate software, as our study was more of an exploratory study.

####E-government

E-government, which became popular alongside the development of the Internet in 2000, is the "delivery of government information and services through the Internet 24 hours a day, 7 days per week" [7].

There are three main government relations that pertain to e-government [8]:

1. **Government to Citizen**: citizens paying bills or taxes, voter registration, business permits and license applications.
2. **Government to Business**: purchase for property, equipment, office supplies.
3. **Government to Government**: our category of concern; includes enabling project teams to collaborate using CSCW technologies, provide news/information and online report generation/procurement tools, publishing documents and manuals online to reduce printing costs [9].

#####Reasons behind innovating with e-government

As the boom in Internet technology grew, there was increasing demand for accurate communication within government and with citizens. The development of e-government was fuelled by emerging opportunities in electronic communications, and more ownership of home PC's [10]. In short, it was implemented "to increase the government’s level of quality service by making the paper-driven or counter-based services more convenient and accessible to citizens and businesses [11]."

#####Methodology to evaluate use of e-government

As a case study, Jorgensen and Cable measured the success of e-government in Corpus Christi using a number of tools. They collected data from the personal experiences of one of the co-authors in Corpus Christi, from interviews with carefully selected individuals familiar with the inner workings of the city, and from archival records [10]. In our study, we will likewise collect data from interviews and records of the city.

#####Implementation of e-government in Corpus Christi

The website went live in late October 1999, with a cost of implementation of roughly $13,000 [10]. The site included forms and applications online (both printable to e-mailable) including building permits, job applications, utility bills, and parking and traffic ticket payment and information [11]. The Internet site was replicated as Intranet for city employees, and included a city directory, city policies, training calendars, a bulletin board, and other communications important to employees [10].

#####Benefits of e-government

The advantages of moving many government processes online are numerous, and include increased government accountability, "greater public access to information and a more efficient, cost-effective government," and easier access to many services including online voting and licence renewal [12].

In his paper about the benefits of e-government, Bhatnagar includes a list of some of its social and economic impacts, taken from cases of cities around the world. These benefits include [13]:
- **increased transparency** (dissemination of Government rules and procedures; disclosure of public assets; making decisions and actions of civil servants transparent)
- **reduced administrative corruption** (putting procedures online so that transactions can be easily monitored)
- **improved service delivery** (less time to complete transactions; reduced travel costs for citizens to interact with government; service to larger segment of population)
- **empowerment** (of underserved communities; reduce the brokerage power of intermediaries)
- **streamlined administrative process** (increased ability of managers to monitor task completion rates of civil servants; improved efficiency of civil servants by automating tedious work; integration of databases, reducing inaccuracies caused by the presence of redundant, duplicate databases)
- **reduced administrative burdens for businesses** (faster access to government and less time needed to interact with government)
- **increased revenue** (convenient to pay taxes; improved audit to identify defaulters; plug leakage by reducing corruption)

<need transition here; it cuts off abruptly> 

####Open Source

Open source software began to play a prominent role in government in 2001, when municipalities in Germany began to migrate their users to open source software. We took a particular look at the case study of Munich, as a lot of data and news articles exist to support the reasoning behind their move to open source software. The case of Munich has more research and accessible public information on its transition attached to it than other examples of open source software in government, which is why we chose to focus on it.

In this section, when we refer to open source software, we are specifically referring to software under the **free open-source software (FOSS)**  category. This term is “a generic term for non-proprietary software that is generally free, can be reviewed by large numbers of users, and can be revised and shared free of charge [14]," and serves as a contrast to the proprietary (privately owned) software seen throughout the corporate world. Adopting this type of software can save significant amounts of money (as will be seen with our example of Munich) but the cost of migration, including training of employees, must be taken into account. 

#####Reasons Behind Innovating with Open Source

Whenever a group migrates to a new system, there are risks involved. A top-down approach is usually taken by politicians in order to mitigate these risks [14]. However, migration of systems is sometimes necessary to motivate innovation. Some of the factors that influence this innovation include [14]:

> 1. Pressure from legislators or politicians.
2. Change in leadership from within or outside an organization.
3. Crises or visible public failures. 
4. Internal failings such as an inability to coordinate across departments or meet the demands of a program.
5. New opportunities that occur through development of new technologies or other factors.
 
However, that is not to say that this type of change is always caused by a negative event. Many times, groups that make this sort of migration to open source software are looking for independence from propriety software. The effectiveness of the software can also play a factor, as many times there is an open source alternative to proprietary software that has equal or greater functional capability than its proprietary counterpart(s). Cost can also play a factor, as previously companies would have to pay for licenses to use proprietary products. Today there also exist subscription models for these proprietary solutions, so a group (public or private) may look to open source alternatives to save on cost. 

In the case of Munich, Microsoft was slated to discontinue its support for Windows NT by 2004 due to systemic security flaws [15], which was the operating system that Munich's city had been primarily using. They took this opportunity to seek alternative solutions in an effort to achieve "greater vendor independence" and take advantage of a highly competitive software market [16]. One of their goals was also to utilize the "future-proofness" of open protocols, data formats and interfaces, and the solution they eventually arrived at was to migrate to open source software. 

#####Transition to Open Source in Munich

The following list details all the options that Munich considered after Microsoft announced the discontinuation of Windows NT [16]: 

> 1. MS XP + MS Office XP 
2. MS XP + OpenOffice 
3. GNU/Linux + OpenOffice 

For the option of GNU/Linux, given that this was a major change compared to updating to the current Microsoft OS, they also considered two transitional solutions [16]: 

> 1. GNU/Linux + OpenOffice + PC Emulation (WINE / VMWare) 
2. GNU/Linux + OpenOffice + Terminal Server

In his paper on the transition to open source in Munich, Grassmuck noted that "both transitional solutions presented architectural and operational complexities, not least with respect to security and an increased need for training. They were therefore considered undesirable as such and only to be deployed where no other solution could be found [16].”

Grassmuck also states that the project leaders determined that a successful migration required "consistent adherence to a number of technological and political principles [16]," and used the following principles to guide this migration [16]:

> 1. Applications should be OS-independent.
2. New client-server applications would only be developed or commissioned as web applications according to the J2EE model.
3. Cooperation of all software partners would be necessary as software is customized, and as applications are redeveloped.
4. The project had to have the support of both political leadership and heads of the administration.
5. Proactive education and involvement of employees would be essential.

Munich did successfully migrate to using open source alternatives for their computing needs. The following table outlines the timeline they adhered to for transitioning to open source software. 

|Date|Step in Transition|
|--------|--------------|
|November 2001|Munich decided to investigate open-source options in operating systems and office suites.|
|April 2002|Commissioned a consulting company for options.|
|May 2003|Made the decision to migrate to open-source software and web applications.|
|2004|Migration to open-source began.|

Munich is not the first city to have documented their transition to open source. The first known city to use open-source was Schwäbisch Hall in Baden-Würtemberg, who migrated their servers in 2002 and all their desktops in 2004 [16]. 

#####Methodology to evaluate usage of open source

An independent review of this open source transition was conducted in 2008 by Mark Cassell, in an attempt to explore why cities in Europe had been migrating to open source software. To do so, he relied on semi-structured interviews with members of four cities that had successfully transitioned to open source software: Vienna, Munich, Schwäbisch Hall, and Treuchtlingen [14]. He specifically stated that he used the following methodology to assess the adoption of open source software in these cities.

> The interview instrument consisted of a set of identical questions related to motivation, implementation, and results. Each questionnaire also contained a set of questions specific to the position of the interviewee. To facilitate coding and analysis of the interviews I used N-Vivo, a qualitative analysis software program. I also relied on internal reports, audits, and news releases published by each city to develop the necessary background for the research and to substantiate information collected through interviews. Finally, I surveyed news accounts to corroborate data produced by the cities and the interviews.

These interviews were initially conducted in German and then translated to English. These interviews were conducted over the course of two months and, as Cassell mentions, coded in part by N-Vivo to help in analysis. 

In our project, we did not feel the need to use specific software to assist in coding and analyzing interview data. Given that we were conducting a small number of interviews across two municipalities, most of the interview transcription was done by hand as interviews were completed. 

##Methodology

For our research, we considered a few different types of approaches to discover what the city council of Victoria currently uses for technology, and how to improve the usage of technology by the city. Before we introduce what our research encompassed and the methodology we followed, we first want to discuss the alternatives approaches and why we rejected them. 

### Alternatives Considered 

One of the approaches we considered was to conduct a usability study on the website currently used by the city of Victoria. 
- list more details here
	- what would we have looked at?
	- why did we choose to ignore the site?
		- we chose to ignore the site because we were much more interested on how individual council members were communicating with each other, and then it turned into how they communicate with constituents. Research was generally from the viewpoint of individual councillors, website is more how the council as a whole shares information
- other approaches considered 

- transition into what methodology we used in our research

### Our Methodology

Before conducting our research, we sought information on what previous research in the field of CSCW had been conducted on government organizations. If previous research had provided insights on what technologies or software suites were preferable to governments, this would be valuable information to bring to the city of Victoria. We found three sources of previous work that helped to shape the methodology used for this project. The end results of two of these works, **Cuparla** and **E-government**, were not as relevant to our research (given their age and the rate at which the computing industry has evolved over the past 20 years), but the methods these studies employed helped to refine ours. In the **open source** study, both the methodology used to evaluate the success of adopting open source software and the results are relevant to our study, as open source software is a cost-effective alternative that, depending on the tools currently used, contains similar functionality to its proprietary counterparts. 

For our research, we collected data from two main sources. Our primary method of data collection was through interviews with city councillors, with our secondary method being observance of public city meetings. We chose these two methods of data collection for a few reasons, with the primary reason being that our research questions involve assessing the quality of communication and document sharing that city councillors currently have access to. Talking directly to these city councillors was the most effective way of assessing this information. Our secondary form of data collection allows us to observe the city's methods of sharing documents with the public and their use of technology to moderate and augment their communications between the city and the public. It also serves as a form of risk mitigation, in case we were unable to conduct all of our planned interviews. Alongside these reasons, we chose these methods because they have been shown to be effective in previous studies of a similar form. Poole notes that group observation and asking questions of individual members are the two best ways to obtain information on group dynamics, and he specifically recommends in-depth interviews in order to "obtain symbols that members naturally use to describe their behaviour" [17]. 

We conducted six semi-structured 30-minute interview sessions in total. The council members that we interviewed were decided primarily on availability, as the time available for this research was limited. Three interviews were conducted with city council members of Victoria, with one interview from the IT manager of the city of Victoria and one interview with a citizen that continually involves themselves with city council operations. To provide control data for other local municipalities, we also interviewed a member of the Sooke city council. 

As previously mentioned, these interviews were semi-structured in nature to allow for topics to be expanded as they were discussed. To design our interviews, we used Löfgren's video on qualitative analysis of interview data [18] so that we knew how to phrase questions in order to obtain the information we desired. Our interviews were focused on three main topics: 
 
1. Technology used in creating bills
2. Technology used in day-to-day communications
3. Personal comfort levels with technology

A partial list of interview questions (that do not violate interviewee privacy) can be found in Appendix C. 

As mentioned before, we also attended public city meetings to observe the usage of computers in facilitating meetings. These meetings typically occur every two weeks on Thursday nights at 7:00pm, and are held at City Hall in Victoria. The two meetings attended were held on October 15th and October 29th. The primary goal with attending these meetings was to observe and assess the conduction of the meetings based on the following metrics: what technologies do they use to administer and share documents, how do they allow for crowd contribution, and how is discussion moderated and facilitated. 

## Results

There are two components to our results from this study:

1. City Council Meeting Observation
2. Interview Results
 
Since we observed two meetings and conducted six interviews, our results from the city council meetings have less depth than the interview findings. We'll discuss our findings from the city council meetings, followed by the interview results. 

### Results from City Council Meetings

All councillors currently have a laptop or tablet at the meeting. Some laptops run Windows, but most are MacBooks. The meeting begins with the mayor verbally announcing any late additions or changes to the agenda since it was published online on the Friday before the meeting. We observed a number of late items added to the agenda at both meetings we attended. In order to construct the agenda, members email their items to the clerk and to council in advance of the meeting.

During the meeting, a number of councillors and the mayor were observed taking notes on paper. In order to determine the order of speaking, the councillors put up their hands and the mayor acknowledges them by nodding and writing their names on a piece of paper, the speaker’s list. 

Microsoft Outlook is used for email communications in the meeting, along with PowerPoint for slide presentations, and Word for the motions of the agenda (which can be scrolled through rapidly if the meeting is moving quickly). The motions and slide presentations are projected on three large television screens, one facing the council. Motions are not always read out in full; it is assumed that the councillors have had a chance to read the motions beforehand. 

Speakers to the council are each personally welcomed by the mayor, and get a pre-determined amount of time to speak—usually between 5 and 20 minutes. This is monitored by a clock system that turns the speaker’s mic on or off at the appropriate time, and is manually reset by the clerk after each speaker. We observed one time that the clock was not reset for a speaker.

While the findings from our observation of city council meetings are few, they provide a basis and context for how the city operates and how councillors interact with each other. Our interviews provided much more depth on how city councillors go about doing their work and how modern technology fits in to their work. 

### Interview Results

From our six interviews, we chose to divide our findings into three major categories: **communication**, **bylaw development**, and **councillor comfort with technology**. Part of our focus with our research was to improve councillor-to-councillor communication, so many of our questions were focused on how councillors currently communicate amongst themselves and what channels they use to communicate. Our other questions related to what work they have to complete and what technologies they use to complete said work; most work that councillors do culminates in the creation of bylaws for the municipality. We also explicitly asked our interviewees about their personal comfort with technology, which helps to provide context for what councillors feel comfortable doing and what they perceive their skills to be. After discussing our findings from the interviews, we go over some of the issues that we identified from the interviews and from the meetings along with possible solutions (if they immediately exist). 

#### Communication

One of the results that was highly emphasized through all our interviews is who city councillors primarily interact and communicate with it. When we started our research, one of our main questions was on how we could improve councillor-to-councillor communication; this presumed that in order to get the majority of their work done and their information organized, councillors would have to work and interact with each other on a frequent basis. However, through our interviews we discovered that councillors place a higher emphasis on communicating and interacting with their constituents. The following diagram helps illustrate what we expected versus what we found regarding councillor-to-councillor communication. 

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Final Report/citycomm.png">
</p>

Most of the discussion that happens between councillors is done through official meetings or committees. This is in part due to how the city has organized itself. Members of the city are expected to follow the proper channels for communication: any communication directed towards city workers has to be conducted through an intermediary city manager. Along with this, any communication channel (e.g. an email chain) that contains 5 or more city members constitutes a legal majority that can affect change, so any communication that involves 5 or more city council members must be conducted at an official meeting. This doesn't mean that councillors are forbidden to interact with other councillors - given that they all have offices next to each other, whenever informal discussion needs to happen between councillors it primarily happens in-person. One interviewee did note that there was "very little unstructed time with other councillors," which highlights that the majority of the communication for councillors occurs between councillors and their consituents. 

To collect information from their consituents, councillors use a few technological mediums. The core technology used in their workflow is email, but councillors also make usage of phone calls, Facebook, and Twitter to interact with their constituents. Many of the councillors view their job as a 24/7 job; councillors have to be available at all times to reply to emails, answer phone calls from constituents, and navigate through social media to address issues that come up with constituents. Each councillor has different ways to make this workflow manageable, but the methods employed to manage their individual work flows vary depending on how much they have to respond to in a day. Looking at emails alone, some of the councillors get 200 emails per day, whereas others can get up to 1000 emails a day. One councillor said that "because [emails] can be forwarded, and because they're permanent in writing, they have to be good. Grammar has to be fine, content has to be fine." If a councillor is getting up to 1000 emails a day and they're being held to the standard of good content and good grammar, it can be very easy to fall behind. According to some of our interviews, some councillors have "gotten to the point where they've given up on emails." If it is true that some councillors have given up on email because it is unmanageable (compared to the amount of effort they have to put in to manage it) then something needs to be done to address this. 

The city council of Victoria also interacts as its own entity with the public by usage of social media and the city web site. The city of Victoria has a general page on [Facebook](https://www.facebook.com/CityofVictoriaPage/) <cite later?> that serves as an announcement page for events going on in the city. Some city councillors also make an attempt to maintain their own personal Facebook pages and Twitter accounts. These are mostly used to interact with their constituents, but some councillors also reach out to councillors from *other jurisdictions* via Twitter; interaction between councillors in Victoria is not conducted via social media. However, one interviewee mentioned that the city has "one guy who is primarily for day to day Twitter" for pushing promotional material out and responding to general questions to the city. So there is a movement from the city towards using social media, but not everyone is buying in. One interviewee said that they don't like Twitter "because there is a problem in trying to get relevant information out of folks in a short number of characters." Whether this is a sentiment shared by other council members remains to be seen, but the fact that some councillors actively use Twitter has to be seen as a positive. 

- some councillors were active on social media primarily for being elected, and neglect to update page afterwards
- one councillor used software (NationBuilder) to help analyse trends in social media, but noted that they only felt it was useful for getting elected

One topic that we wanted to bring up in interviews was the notion of privacy. We wanted to know how city councillors ensured private data was kept private and what types of data need to be kept private. A lot of the work and communication that councillors put out (through email, Facebook, other) can be accessed by citizens through a Freedom of Information request (FOI), which means that the majority of written communication conducted by councillors is public information. Some exceptions do exist in regards to privacy; any documents regarding legal issues and any written communication on employee relations or employee performance do not have to be given out via a FOI request. Beyond these two exceptions, councillors have no expectation of privacy in their work and the way they conduct their communication with constituents reflects this. This may also help explain why some councillors are seemingly giving up on responding to emails: at a large enough volume, if they send out a poorly worded email it may come to hurt them in the future (e.g. for job prospects) so it's simply easier to just not respond rather than do a poor job of managing communication. 

For data that does need to remain private (personal files on laptops, for example) there are a few measures put in to place by the city. Each councillor is issued a laptop, an iPad, and a smartphone by the city; while the laptop and smartphone model decision is left to the councillor in question, each of these city-issued devices is encrypted by the IT department. Should these devices be lost, misplaced or stolen from councillors, the data on the devices themselves is encrypted and is much harder to gain access to. Through the interviews, we also learned that communication between city staff members and city council members is stored on servers physically located in Victoria; this is compliant with privacy laws in B.C. that state that personal information cannot be stored outside of B.C. Any sensitive documents that have to be shared between council members are typically shared as physical copies, and are shredded after usage. This approach respects privacy well, but may be open to improvement in the future. 

With regards to meetings, councillors spend a decent amount of time in meetings, both informal and formal. Some councillors conduct informal group meetings with citizens 

- Councillors do informal group meetings with citizens at a small level
- some councillors redirect phone calls from their "official" <office?> number to their personal cell number
- some request phone calls to follow up on particularly large/complicated emails

- Scheduling of meeting is done over an email
- Official meetings are organized by city staff and facilitated by the Mayor


- Councillor can join to city meetings through Skype
	- none of the councillors interviewed were aware that there were bylaws that permitted them to participate remotely in meetings
		- either bylaw found on site is incorrect or councillors simply haven't felt the need to remotely participate in meetings yet
	- for comparison, interviewee from Sooke made mention of some participation via phone for meetings
- Electronic version of agenda is available on Meeting management software during city meetings
- Late Items  are added into addendum of agenda during the meetings
- Comparative study is followed to determine the software which can be used within the City council

#### Bylaw Development

As seen before, data collection for the purposes of changing or creating bylaws is largely an individual effort for city councillors. Each councillor collects data, opinions and complaints from their constituents (primarily via email) and collates these into reports or summaries that they bring to their respective committees or meetings. To facilitate data collection, one interviewee reported that they scan physical documents and then email these attachments to other people for further input. A lot of documents are emailed back and forth between constituents, councillors, and other individuals, with very little collaborative editing or writing occurring. One councillor mentioned that they use Google Docs for collaboratively working with their "closest allies" but that seems to be the exception rather than the rule. This type of version control is what we expected to find when we conducted these interviews: that no official protocol exists for controlling and ensuring the correct version of the document is being used. 

Meetings and committees are where the majority of discussion occurs regarding bylaw development. After issues are discussed and debated in these meetings, city staff that were moderating the meetings will type up reports on what happened during the meeting. From what we gathered from our interviews, city staff do not collaboratively write these reports after the meetings - these reports are typically written on an individual basis and then shared either digitally or via printed copy for further review. It's important to note that the city councillors are not the individuals writing the reports after meetings and committees and that city staff are responsible for writing these documents, as further studies may wish to target this group for study instead of the city councillors. 

The vehicle most widely used to share documents between city council members is sharing via physical distribution.

Some of the data from meetings and reports is made accessible via the city of Victoria's website. Currently, the city offers data in CSV, KML, SHP and XLS formats. However, from our interviews we learned that 

- one interviewee views city council being fairly hypocritical in their plan vs. their execution
	- statement to want to go paperless
	- 1000 page binder for budget discussion made soon after
- city currently uploads data in CSV, KML, SHP, XLS formats
	- Learning of .json code writing to have a data approach instead of file approach
		- **being conducted by a citizen**
		- idea is to take the "millions" of PDFs the city generates and convert them to .json so they can be more easily accessed, edited and modified

<transition into general section on the issues we've identified in city, and how we're classifying them>

#### Councillor Comfort with Technology

### Issues Identified

<classifications fall under some type of categorization, depending on severity of issue and time expected to fix/address>
- On preliminary inspection, there is potentially room for improvement at the council’s meetings. One possibility could be some type of system to automate the speaker’s list, perhaps using an app on a smartphone to indicate speaker order as opposed to paper. Also, perhaps the city council could consider a note-taking app to move away from taking notes about the meeting with pen on paper. There are products on the market to automate the voting process such as IVS City Council that may be considered.
- citizens feel that to get data in a more parseable format they have to put the files into that format
	- should be an effort on city level to put this data into more parseable forms (.json example brought up in one of the interviews)
- weak wifi in city council chambers
	- takes a while to download files (sometimes 2000+ pg PDFs) while in city council meetings
	- some people have to resort to tethering off their iPhones to get wifi in the meeting room
	- shouldn't be an issue in 2015 -- get a stronger setup in the room(s)!
	- loading of files manual or automatic?
- IT is isolated from city hall
	- located in a separate building from city hall entirely
	- software suites are chosen by finance department -- IT only maintains, has no say over what's being chosen in terms of software
- no central repository for files that need to be shared
	- all councillors primarily use computer's file system for file organization
- webcasts and website not well-formatted on mobile

![alt-text](https://github.com/cscw2015/maverick/blob/master/Final Report/city_hall_main_page.png "Main page on mobile")
![alt-text](https://github.com/cscw2015/maverick/blob/master/Final Report/city_video_mobile.png "View for accessing old webcasts")
![alt-text](https://github.com/cscw2015/maverick/blob/master/Final Report/fullscreen_webcast.png "An old webcast, fullscreen")

## Conclusions 

- research questions reiterated here so we can affirm whether or not they were answered:

1. What technologies already exist or are being used to help city councillors in their meetings, with respect to document sharing and communication?
2. What issues are they currently facing with their present technology?
3. How can we improve communication between city councillors?

- answers to each question
- 1. Currently using Microsoft Word on screens in council chambers to see the current document and changed to the document. All have individual laptops and/or tablets that they use to look at documents and references during meetings. 
- 2. Currently facing weak wifi in council chambers, overwhelmed by email. No version control, just email new versions to everyone
- 3. Turns out to be less of an issue than we initially thought. Probably could use some sort of messaging system for communicating with other councillors, as current system seems pretty dysfunctional.
- other questions that have arisen from work
	- what can be explored next? What should be explored next?
		- things to be explored next include in depth look at website, the possibility of implementing some sort of version control software
	- do other nearby municipalities have similar setups and/or issues re:technology?

## Impact

This project immediately offers two things to the city of Victoria:

1. It offers an outside perspective on current communication practices within the government, which may help identify flaws in communication practices; and
2. It offers transparency on communication practices employed by the government, so citizens of Victoria can be more aware of how the city operates on a technical level.

A longer time frame for this study could have allowed for follow-up interviews, observation of private meetings (as opposed to primarily public forums), or even designing and testing a new suite of software that focuses in particular on the needs of the municipality of Victoria. 

Similarly, this study could also be modified to assess similar issues on a provincial or federal scale. Such modified studies would need to have a broader focus (they may involve assessing the public's desires of the government vs. the government's responsibilities towards communications and data privacy) and would require a much larger time frame. 

These types of studies are rarely conducted, in comparison to other fields of work. Typically, government organizations are audited by a specific subset of companies, but these audits tend to focus on ensuring the government is up to the current standard. Our study looks to go beyond the current standards and afford the opportunity for technological innovation, as a benefit for the public. 

##Appendices

### Appendix 1: Team Roles

####Kimberlee Graham-Knight: Group Leader
Kimberlee is taking on the role of group leader. She is responsible for regularly checking in on each group member to ensure that they are fulfilling their roles and that any issues or questions they have can be addressed as soon as possible. This includes delegating tasks as necessary. Kimberlee is also responsible for conducting some of our interviews with city councillors, and has attended some of the city council meetings to help establish a background for our research. Further, she is responsible for some of the literature review along with Roshni.

####Roshni Jain: Data Analysis
Roshni is responsible for overseeing the analysis of all the data we collect from interviews. As interviews are completed, she and Tian will be transcribing the audio recordings provided from these interviews. After all the transcriptions are completed, Roshni will be responsible for leading the analysis on these interview results. She is also responsible for reviewing any relevant literature and collating the background research necessary to ground this project and give it context. To assist with providing context, Roshni has attended some of the city council meetings. 

####Nigel Dufty: Data Collection
Nigel is responsible for a majority of the data collection involved in the project. He is working with Kimberlee and Tian to organize and conduct interviews of Victoria city council members. To ensure that the audio files from the interviews are kept secure, Nigel is acting as an intermediary for transferring audio from the interviews to Roshni and Tian via an encrypted USB stick. Nigel has also attended city council meetings to help provide context for interviews and for our background research. 

####Tian Geng: Data Analysis
Tian is working with Roshni to create transcriptions of interviews as they are completed. He is also working with Kimberlee and Nigel to conduct interviews of city council members of Victoria. Tian is also responsible for conducting literature review alongside Roshni and Kimberlee. 

####Myan Panikkar: Editor
Myan is responsible for all written deliverables in the project. As the primary editor, his job is to ensure that documents needed for the project are coherent, cohesive, and that they are delivered as complete products. This involves some leadership alongside Kimberlee, namely for delegating section content amongst group members as necessary. Myan will also be writing and designing the consultant report that our group intends to deliver to the city council after our interview data has been analyzed. Myan also attended city council meetings to help provide background research. 

## Appendix 2: Milestones

The following table outlines our previous milestones and our progress on these milestones as of November 4th (when we gave an oral update on our project). Many of our milestones were met successfully, but a few issues arose when we compared our progress to our initial timeline draft. 

### Status on Original Milestones

| Date | Task to Complete | Status |
|------|------------------|--------|
|October 15| City Meeting 1 | Finished |
|October 16| Project Proposal Finished | Finished  | 
|October 19| Interview Template Finalized | Finished | 
|October 19| Requests for Interview sent | Pending | 
|October 19| Ethics application complete | Finished | 
|October 29| City Meeting 2 | Finished
|November 4| Oral update on project | Pending |
|November 6| Interviews Completed| Date to be adjusted | 
|November 13| Interim Project Report| Pending |
|December 2| Project Presentation | N/A | 
|December 4| Project Report Finalized | N/A |

One of the more visible issues that can be seen from this table pertains to the interviews. Specifically, we intended to send out requests for interviews on October 19 (when we planned to have our ethics application completed) but we did not complete this until November 4th. While we recognize that our initial deadline was ambitious, leaving our requests for interview until this past week does set us back slightly. Combine this with our increased number of interviews planned and our next deadlines become much stricter. Our new planned date to complete interviews is November 20th. Part of the reason we chose this date pertains to our next issue.

The next issue that this table fails to address is when we plan to have the data from our interviews transcribed. As we plan to do eight interviews in total, transcribing these interviews will take a considerable amount of time. However, we do not have a considerable amount of time available to complete the interviews, transcribe the interviews, interpret their results and propose possible changes to the city's technological setup (if necessary). Currently, we plan to transcribe interviews as we finish. We do need to set a final date for when we want these transcriptions to be complete, so to allow ourselves enough time to analyze the data we chose November 23rd as the final date for interview transcriptions to be completed. 

A third issue that that isn't visible from looking at this table is that we never detailed what would be given to the city council of Victoria as a final deliverable, nor did we state when such a deliverable would be completed and delivered to the city. To address this, we chose to develop a non-academic report to deliver to the city council of Victoria. This report will be less formal in nature and will not contain as many of the academic citations as our final report will, but it will follow a similar structure in order to highlight our findings from the interviews we plan to conduct. 

Given these issues, we made amendments to our timeline from November 4th and beyond. The following table details the changes we previously described in our timeline. 

### New Timeline
| Date | Task to Complete | 
|------|------------------|
|November 4|Requests for Interview sent|
|November 4|Oral update on project|
|November 13|Interim Project Report|
|November 20|Interviews will be Completed|
|November 23|Transcripts will be Completed|
|November 27|Data Analysis will be done|
|December 2|Project Presentation|
|December 4|Final Report|
|December 4|Consultant's Report|

At this point in the project, we have a few tasks left to accomplish. Some of our interviews have been completed already, but we have to finish the remainder of the interviews. Some of our original interview targets have been shifted around due to the previous candidates being unavailable, with some of these new candidates being non-council members. These changes have been reflected in the [Methodology](#methodology) section. 

As each interview is completed, we have to transcribe it. The dates above are the _final_ dates for interviews and their respective transcriptions; we will be dealing with the data as it flows in. Once we have all of the interview data in a usable format, analysis will be conducted on it to determine the best method of approach to technology for the city council. This best method (or set of methods) will then be presented in a report to the city council at the end of the semester. 

## Appendix 3: Interview Questions

The following list contains general questions used throughout our interviews to facilitate discussion. Not all questions are listed, as some are context-specific to interviews and/or break confidentiality. 


## Appendix 4: Tools Used by Council

Through all the interviews we discovered a set of software tools that the city is currently using to manage their day-to-day operations. As these tools do not fit into any other section of the report, we list them here along with their general function. Future studies on the city of Victoria may want to look at these tools (or their replacements, should they be replaced) and assess whether they are being used effectively. 

**Tools**
- Development tracker that has documents about every development that’s happening in the city which was made online this year (2015)
- NationBuilder, a constituency management  for tracking emails. It’s a political organizer. The website basically runs on the NationBuilder platform which has  a database attached to it.
- Atomic Crayon, website provider
- Icompass provides software for information management services for council and committee operations.
- Granicus and Civic web are for council operations. 
- Meeting Management Software designed by iCompass is used  to get the agenda and do some modifications as and when required during the council meetings.
- Meeting  Broadcast Software designed by Granicus is used to broadcast the city meetings.
- Microsoft suite is used for core productivity.
- Tempest is used for building and permitting software.
- JD Edward Software is used for core financial purposes.
- SurveyMonkey is used to collect available meeting times from all councillors
- Website is there for council-public communication
- HaveYourSay is the portal where all the citizen engagement activities are posted
- PlaySpeak was used to track development applications earlier
- Internal App of Civic web is used to manage huge agendas on the councillors ipad during meeting

## References

1. Schümmer, T., Tandler, P., & Hakke, J. M. (2012). The next-generation business meeting: from i-lands to flexible meeting landscapes. *Universal Access in the Information Society, 11*(3), 239-258.
2. Walker, R. M. (2006). Innovation type and diffusion: An empirical analysis of local government. *Public administration, 84*(2), 311-335.
3. Ihrke, D., Proctor, R., & Gapris, J. (2003). Understanding innovation in municipal government: City council member perspectives. *Journal of Urban Affairs, 25*(1), 79-90. 
4. Schwabe, G., & Krcmar, H. (2000). Piloting Socio-Technical Innovation. ECIS 2000 Proceedings, 27.
5. Schwabe, G., & Krcmar, H. (2000). Digital material in a political work context-The case of Cuparla. ECIS 2000 Proceedings, 150.
6. Schwage, G. (2000). From Analysis to Evaluation - The Case of Cuparla. Found online: [http://www.zora.uzh.ch/57144/1/20120125131854_merlin-id_3158.p](http://www.zora.uzh.ch/57144/1/20120125131854_merlin-id_3158.p) 
7. Reddick, C. G., & Frank, H. A. (2007). The perceived impacts of e-government on US cities: A survey of Florida and Texas City managers. Government Information Quarterly, 24(3), 576-594.
8. Tat-Kei Ho, A. (2002). Reinventing local governments and the e-government initiative. *Public administration review, 62*(4), 434-444.
9. Reddick, C. G. (2004). A two-stage model of e-government growth: Theories and empirical evidence for US cities. *Government Information Quarterly, 21*(1), 51-64.
10. Jorgensen, D. J., & Cable, S. (2002). Facing the challenges of e-goverment: A case study of the city of Corpus Christi, Texas. SAM Advanced Management Journal, 67(3), 15.
11. Burn, J., & Robins, G. (2003). Moving towards e-government: a case study of organisational change processes. Logistics Information Management, 16(1), 25-35.
12. Carter, L., & Bélanger, F. (2005). The utilization of e‐government services: citizen trust, innovation and acceptance factors*. Information systems journal, 15(1), 5-25.
13. Bhatnagar, S. (2003). The economic and social impact of e-government. Background Paper for UNDESA publication: E-Government—the Citizens and the State: Debating Governance in The Information Age. World Public Sector Report. http://www. iimahd. ernet. in/~ subhash/pdfs/UNDESAeGovReport. pdf.
14. Cassell, M. (2008). Why governments innovate: Adoption and implementation of open source software by four European cities. International public management Journal, 11(2), 193-213.
15. (2003). Flaw in RPC Endpoint Mapper Could Allow Denial of Service Attacks (331953). Accessed online: [https://technet.microsoft.com/library/security/ms03-010](https://technet.microsoft.com/library/security/ms03-010)
16. Grassmuck, V. “LiMux — Free Software for Munich” (2005) http://waste.informatik.hu-berlin.de/grassmuck/texts/limux.pdf Accessed November 11, 2015.
17. Poole, M. S., Keyton, J., & Frey, L. R. (1999). *Group communications methodology* (pp 92-112). L. R. Frey, D. S. Gouran, & M. S. Poole (Eds.). Thousand Oaks, CA: Sage Publications. 
18. Löfgren, K. (2013). *Qualitative analysis of interview data: A step-by-step guide*. Accessed online: [https://www.youtube.com/watch?v=DRL4PF2u9XA](https://www.youtube.com/watch?v=DRL4PF2u9XA)
