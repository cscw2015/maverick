Analyzing and Modernizing Victoria City Council's Communications: Final Report
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
6. [Impact](#impact-and-future-work)
7. [Appendices](#appendices)
	1. [Appendix 1: Team Roles](#appendix-1-team-roles)
		1. [Kimberlee Graham-Knight](#kimberlee-graham-knight-group-leader)
		2. [Roshni Jain](#roshni-jain-data-analysis)
		3. [Nigel Dufty](#nigel-dufty-data-collection)
		4. [Tian Geng](#tian-geng-data-analysis)
		5. [Myan Panikkar](#myan-panikkar-editor)
	2. [Appendix 2: Milestones](#appendix-2-milestones)
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

Before looking at previous implementations of computer-supported collaborative work (CSCW) in government settings, we need to understand some of the difficulties of integrating CSCW into meetings. We also need context for why it is important for municipal governments to want to incorporate modern CSCW into their workflow. 

### CSCW in Meetings

According to Schümmer, there are three distinct facets of designing an electronic face-to-face meeting system  [1]:

> 1. the peopleware perspective, the design of social processes that are executed by team members,
2. the generic groupware perspective for designing supportive software tools, and
3. the roomware perspective that considers the configuration of artifacts that constitute the tangible meeting space.

The following figure helps to provide a context for what Schümmer is trying to illustrate. Specifically, it shows where modern, everyday technology fits into his model of an electronic meeting system [1]. 

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/cscw_in_meetings.png">
</p>

Arguably, the hardest facet of designing an electronic meeting system for a group is understanding their needs. To properly assess the needs of a group that needs to meet on a regular basis, one needs to observe how the group interacts in a meeting and what the group needs from their available technology to augment and improve their workflow. While many tools (both open source and proprietary) today are being rapidly developed and improved on, they are not guaranteed to meet the needs of public officials. 

Understanding Schümmer's scheme as it relates to city council is part of the motivation of our study. To ensure that our government has room to innovate, an assessment of their current technological integration and their current communication practices is necessary. 

### Local Government Innovation

Innovation is an important part of any continued collaborative group work. Walker says innovation is a core task of public institutions and that "innovation has been promoted around the world as a key tool to improve public services" [2]. This is one of the reasons we are targeting the city of Victoria with our study: public services always stand to be improved, and the city is in one of the best positions to affect this change. Ihrke notes that local governments are more likely to innovate than governments at the state or federal level because of "their small size and capacity to make decisions quickly and decisively" [3], and this is another reason as to why we are targeting the city of Victoria. While standards do exist at the provincial and federal level for regulating what technologies can be used in government organizations, municipal governments like the city of Victoria can be more receptive to change and can integrate suggestions for improvement at a much faster pace than provincial or federal bodies. 

We believe the city of Victoria would be interested in this sort of study for two reasons. The first is that by recognizing any potential shortcomings in their current practices they can quickly take steps to remedy these shortcomings; our study offers this through analysis of interviews with city officials. The second reason is that local governments tend to get a lot of pressure to "do more with less" [2] so by offering potential alternatives to the city (should they be applicable), the city can choose to shift the technologies they use and potentially lower their current costs. To help inform this decision, should we make any suggestions towards changing the software or the way they use software we will also include the cost of changing this software, where applicable. 

Before addressing how we assess the current state of technological use in the municipality of Victoria, we need to consider what has been done before in this field of research. The following section details the history of CSCW integration with governments. 

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

- Any software required to support council members needed to have functionality supporting the "anytime, anyplace" style of meeting. This was required as council members did not have fixed office locations to prepare for city hall meetings. 
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

Evaluation of Cuparla was done on five sets of criteria and four levels of aggregation [6]. The criteria used to evaluate Cuparla were **cost, time, quality, flexibility,** and **human situation**. The four levels of aggregation used to distinguish the user groups involved were the **individual**, the **group**, the **process**, and the **organization**. As seen in the following figure, these criteria were aligned to create a 4x5 matrix for easier evaluation. Any notes made in the evaluation were attributed only to the lowest applicable level. For instance, the costs of a server would be attributed to the **group** as that is the lowest level in direct need of the server, whereas a PC in an office is attributed to the **individual** level. 

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/Evaluation of Curparla.png">
</p>

Using a matrix of this sort seemed to be an effort to reduce the redundancy in data obtained from the evaluation. We did not use such a method in our study to evaluate software, as our study was more of an exploratory study.

####E-government

E-government, which became popular alongside the development of the Internet in 2000, is the "delivery of government information and services through the Internet 24 hours a day, 7 days per week" [7].

There are three main government relations that pertain to e-government [8]:

1. **Government to Citizen**: citizens paying bills or taxes, voter registration, business permits and license applications.
2. **Government to Business**: purchase for property, equipment, office supplies.
3. **Government to Government**: our category of concern; includes enabling project teams to collaborate using CSCW technologies, providing news/information and online report generation/procurement tools, publishing documents and manuals online to reduce printing costs [9].

#####Reasons behind innovating with e-government

As the boom in Internet technology grew, there was increasing demand for accurate communication within government and with citizens. The development of e-government was fuelled by emerging opportunities in electronic communications, and more ownership of home PC's [10]. In short, it was implemented "to increase the government’s level of quality service by making the paper-driven or counter-based services more convenient and accessible to citizens and businesses [11]."

#####Methodology to evaluate use of e-government

As a case study, Jorgensen and Cable measured the success of e-government in Corpus Christi using a number of tools. They collected data from the personal experiences of one of the co-authors in Corpus Christi, from interviews with carefully selected individuals familiar with the inner workings of the city, and from archival records [10]. In our study, we have likewise collected data from interviews and records of the city.

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

E-government later spawned the Government 2.0 movement, in which governments increasingly interacted with citizens and communicated amongst themselves using Web 2.0 technologies such as social media. Another development that was contemporary with Government 2.0 was the adoption of Open Source software solutions to meet the needs of cities. 

####Open Source

Open source software began to play a prominent role in government in 2001, when municipalities in Germany began to migrate their users to open source software. We take a particular look at the case study of Munich, as a lot of data and news articles exist to support the reasoning behind their move to open source software. The case of Munich has more research and accessible public information on its transition attached to it than other examples of open source software in government, which is why we choose to focus on it.

In this section, when we refer to open source software, we are specifically referring to software under the **free open-source software (FOSS)**  category. This term is “a generic term for non-proprietary software that is generally free, can be reviewed by large numbers of users, and can be revised and shared free of charge [14]," and serves as a contrast to the proprietary (privately owned) software seen throughout the corporate world. Adopting this type of software can save significant amounts of money (as will be seen with our example of Munich) but the cost of migration, including training of employees, must be taken into account. According to Yochai Benkler, the new economy is based on increasing use of FOSS [15], and the development of FOSS such as Wikipedia is contemporary with the development of cities adopting open source solutions.

#####Reasons Behind Innovating with Open Source

Whenever a group migrates to a new system, there are risks involved. A top-down approach is usually taken by politicians in order to mitigate these risks [14]. However, migration of systems is sometimes necessary to motivate innovation. Some of the factors that influence this innovation include [14]:

> 1. Pressure from legislators or politicians.
2. Change in leadership from within or outside an organization.
3. Crises or visible public failures. 
4. Internal failings such as an inability to coordinate across departments or meet the demands of a program.
5. New opportunities that occur through development of new technologies or other factors.
 
However, that is not to say that this type of change is always caused by a negative event. Many times, groups that make this sort of migration to open source software are looking for independence from proprietary software. The effectiveness of the software can also play a factor, as many times there is an open source alternative to proprietary software that has equal or greater functional capability than its proprietary counterpart(s). Cost can also play a factor, as previously companies would have to pay for licenses to use proprietary products. Today there also exist subscription models for these proprietary solutions, so a group (public or private) may look to open source alternatives to save on cost. 

In the case of Munich, Microsoft was slated to discontinue its support for Windows NT by 2004 due to systemic security flaws [16], which was the operating system that Munich's city had been primarily using. They took this opportunity to seek alternative solutions in an effort to achieve "greater vendor independence" and take advantage of a highly competitive software market [17]. One of their goals was also to utilize the "future-proofness" of open protocols, data formats and interfaces, and the solution they eventually arrived at was to migrate to open source software. 

#####Transition to Open Source in Munich

The following list details all the options that Munich considered after Microsoft announced the discontinuation of Windows NT [17]: 

> 1. MS XP + MS Office XP 
2. MS XP + OpenOffice 
3. GNU/Linux + OpenOffice 

For the option of GNU/Linux, given that this was a major change compared to updating to the current Microsoft OS, they also considered two transitional solutions [17]: 

> 1. GNU/Linux + OpenOffice + PC Emulation (WINE / VMWare) 
2. GNU/Linux + OpenOffice + Terminal Server

In his paper on the transition to FOSS in Munich, Grassmuck noted that "both transitional solutions presented architectural and operational complexities, not least with respect to security and an increased need for training. They were therefore considered undesirable as such and only to be deployed where no other solution could be found [17].”

Grassmuck also states that the project leaders determined that a successful migration required "consistent adherence to a number of technological and political principles [17]," and used the following principles to guide this migration [17]:

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

Munich is not the first city to have documented their transition to FOSS. The first known city to use open source was Schwäbisch Hall in Baden-Würtemberg, who migrated their servers in 2002 and all their desktops in 2004 [17]. 

#####Methodology to evaluate usage of open source

An independent review of this open source transition was conducted in 2008 by Mark Cassell, in an attempt to explore why cities in Europe had been migrating to FOSS. To do so, he relied on semi-structured interviews with members of four cities that had successfully transitioned to open source software: Vienna, Munich, Schwäbisch Hall, and Treuchtlingen [14]. He specifically stated that he used the following methodology to assess the adoption of FOSS in these cities.

> The interview instrument consisted of a set of identical questions related to motivation, implementation, and results. Each questionnaire also contained a set of questions specific to the position of the interviewee. To facilitate coding and analysis of the interviews I used N-Vivo, a qualitative analysis software program. I also relied on internal reports, audits, and news releases published by each city to develop the necessary background for the research and to substantiate information collected through interviews. Finally, I surveyed news accounts to corroborate data produced by the cities and the interviews.

These interviews were initially conducted in German and then translated to English. These interviews were conducted over the course of two months and, as Cassell mentions, coded in part by N-Vivo to help in analysis. 

In our project, we did not feel the need to use specific software to assist in coding and analyzing interview data. Given that we were conducting a small number of interviews across two municipalities, most of the interview transcription was done by hand as interviews were completed. 

##Methodology

For our research, we considered a few different types of approaches to discover what the city council of Victoria currently uses for technology, and how to improve the usage of technology by the city. Before we introduce what our research encompassed and the methodology we followed, we first want to discuss the alternatives approaches and why we rejected them. 

### Alternatives Considered 

One of the approaches we considered was to conduct a usability study on the website currently used by the city of Victoria. We were not sure what content of the website we would have looked at, or what rubric for evaluation we would have used, until we talked to people first in order to get a sense of what was most important on the website and for the functioning of the city. Now that we have spoken to councillors and to people in the community, it has become clear that the data available on the website in terms of bylaw development and passing is most important, and that this is readily available on the website according to sources we spoke with. We chose to ignore the site in our research because we were much more interested on how individual council members were communicating with each other, and then it turned into how they communicate with constituents. Research was generally from the viewpoint of individual councillors, while the website is more how the council as a whole shares information.

Another approach we considered was to send out a mass survey of councillors in Victoria. We could have developed a good set of questions and sent them out by email to the 8 councillors and waited for them to respond. However, this would have allowed for limited time to respond, which might have limited the results we received. Also, because there are only 8 councillors total in Victoria, plus the mayor, it seemed manageable to interview some of them. Judging by the results we received, it was unlikely we would have received as much data from questionnaires. In the end, we decided interviews were the best way to extract data from the councillors.

### Our Methodology

Before conducting our interviews and attending council meetings, we sought information on what previous research in the field of CSCW had been conducted on government organizations. If previous research had provided insights on what technologies or software suites were preferable to governments, this would have been valuable information to bring to the city of Victoria. We found three sources of previous work that helped to shape the methodology used for this project. The end results of two of these works, **Cuparla** and **E-government**, were not as relevant to our research (given their age and the rate at which the computing industry has evolved over the past 20 years), but the methods these studies employed helped to refine ours. In the **open source** study, both the methodology used to evaluate the success of adopting open source software and the results are relevant to our study, as open source software is a cost-effective alternative that, depending on the tools currently used, contains similar functionality to its proprietary counterparts. 

We collected data from two main sources. Our primary method of data collection was through interviews with city councillors, with our secondary method being observance of public city meetings. We chose these two methods of data collection for a few reasons. First, our research questions involve assessing the quality of communication and document sharing that city councillors currently have access to. Talking directly to these city councillors was the most effective way of assessing this information. Our secondary form of data collection allows us to observe the city's methods of sharing documents with the public and their use of technology to moderate and augment their communications between the city and the public. It also serves as a form of risk mitigation, in case of inability to conduct all of our planned interviews. Alongside these reasons, we chose these methods because they have been shown to be effective in previous studies of a similar form. Poole notes that group observation and asking questions of individual members are the two best ways to obtain information on group dynamics, and he specifically recommends in-depth interviews in order to "obtain symbols that members naturally use to describe their behaviour" [18]. 

We conducted six individual, in-depth, semi-structured, 30-minute interview sessions in total. The council members we interviewed were decided primarily on availability, as the time available for this research was limited. Three interviews were conducted with city council members of Victoria, with one interview from the IT manager of the city of Victoria and one interview with a citizen that continually involves themselves with city council operations. To provide control data for other local municipalities, we also interviewed a member of the Sooke city council. 

As previously mentioned, these interviews were semi-structured in nature to allow for topics to be expanded as they were discussed. To design our interviews, we used Löfgren's video on qualitative analysis of interview data [19] so that we knew how to phrase questions in order to obtain the information we desired. Our interviews were focused on three main topics: 
 
1. Technology used in creating bylaws
2. Technology used in day-to-day communications
3. Personal comfort levels with technology

A partial list of interview questions (that do not violate interviewee privacy) can be found in Appendix C. 

As mentioned before, we also attended public city meetings to observe the usage of computers in facilitating meetings. These meetings typically occur every two weeks on Thursday nights at 7:00pm, and are held at City Hall in Victoria. The two meetings attended were held on October 15th and October 29th. The primary goal with attending these meetings was to observe and assess the conduction of the meetings based on the following metrics: what technologies do they use to administer and share documents, how do they allow for crowd contribution, and how is discussion moderated and facilitated? 

Some of the limitations of our methodology are that it is extremely time-consuming to interview city councillors, then transcribe and analyze the data. Because of the amount of effort required, other possible options, such as analyzing the website, were not able to be pursued. Also, Poole notes that interviewees may not always be entirely truthful [18] because they may feel certain pressures, and these pressures must be doubly important for people in the public eye such as city councillors. As we discovered, the councillors consider nearly all of their communication to be public, and because the interviews are recorded and transcribed, it is possible many of the councillors considered them to be essentially public, and may have been guarded with some of their answers. Further, our study was conducted over a short period of time, so there was no accounting for how the attitudes and behaviours of the councillors towards technology change over time. Finally, we made the assumption in our questions that the main group to be studied was the councillors working together. So, our line of questioning reflected this bias. However, over the course of our research, we discovered that councillors spend much more time and energy interacting with their constituents, and in hindsight we might have changed our questioning to account for this.

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

While the findings from our observation of city council meetings are few, they provide a basis and context for how the city operates and how councillors interact with each other. Our interviews provided much more depth on how city councillors go about doing their work and how modern technology fits into their work. 

### Interview Results

From our six interviews, we chose to divide our findings into three major categories: **communication**, **bylaw development**, and **councillor comfort with technology**. Part of our focus with our research was to improve councillor-to-councillor communication, so many of our questions were focused on how councillors currently communicate amongst themselves and what channels they use to communicate. Our other questions related to what work they have to complete and what technologies they use to complete said work; most work councillors do culminates in the creation of bylaws for the municipality. We also explicitly asked our interviewees about their personal comfort with technology, which helps to provide context for what councillors feel comfortable doing and what they perceive their skills to be. After discussing our findings from the interviews, we go over some of the issues that we identified from the interviews and from the meetings along with possible solutions (if they immediately exist). 

#### Communication

One of the results that was highly emphasized through all our interviews is who city councillors primarily interact and communicate with. When we started our research, one of our main questions was on how we could improve councillor-to-councillor communication; this presumed that in order to get the majority of their work done and their information organized, councillors would have to work and interact with each other on a frequent basis. However, through our interviews we discovered that councillors place a higher emphasis on communicating and interacting with their constituents. The following diagram helps illustrate what we expected versus what we found regarding councillor-to-councillor communication. 

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Final Report/citycomm.png">
</p>

Most of the discussion that happens between councillors is done through official meetings or committees. This is in part due to how the city has organized itself. Members of the city are expected to follow the proper channels for communication: any communication directed towards city workers has to be conducted through an intermediary city manager. Along with this, any communication channel (e.g. an email chain) that contains 5 or more city members constitutes a legal majority that can affect change, so any communication that involves 5 or more city council members must be conducted at an official meeting. This doesn't mean that councillors are forbidden to interact with other councillors - given that they all have offices next to each other, whenever informal discussion needs to happen between councillors it primarily happens in-person. One interviewee did note that there was "very little unstructured time with other councillors," which highlights that the majority of the communication for councillors occurs between councillors and their constituents. 

To collect information from their constituents, councillors use a few technological mediums. The core technology used in their workflow is email, but councillors also make usage of phone calls, Facebook, and Twitter to interact with their constituents. Many of the councillors view their work as a 24/7 job; councillors have to be available at all times to reply to emails, answer phone calls from constituents, and navigate through social media to address issues that come up with constituents. Each councillor has different ways to make this workflow manageable, but the methods employed to manage their individual work flows vary depending on how much they have to respond to in a day. Looking at emails alone, some of the councillors get 200 emails per day, whereas others can get up to 1000 emails a day. For the councillors that receive a smaller number of daily emails, some request that constituents give them a phone call to follow up on particularly complicated or longer emails, and this is for a couple of reasons. The first is that phone calls are more personal and allow for more direct communication between constituents and councillors, and the second is that councilors are expected to write emails of higher quality. One councillor said "because [emails] can be forwarded, and because they're permanent in writing, they have to be good. Grammar has to be fine, content has to be fine." If a councillor is getting up to 1000 emails a day and they're being held to the standard of good content and good grammar, it can be very easy to fall behind (note that none of the councillors have administrative staff). According to some of our interviews, some councillors have "gotten to the point where they've given up on emails." If it is true that some councillors have given up on email because it is unmanageable (compared to the amount of effort they have to put in to manage it) then something needs to be done to address this.

Councillors spend a decent portion of time in meetings, both formal and informal. For informal meetings, councillors work with other individuals (other council members, city staff or citizens) in informal committees to work on various issues. Some of these committees end up being formalized, and any formal city council committee or meeting is required to be run by city staff and has to follow specific standards for how the meeting is conducted. Official meetings are organized by city staff through email and are typically facilitated by the mayor; to determine meeting times, one councillor mentioned the use of SurveyMonkey to collect viable meeting times for individuals involved in the meeting. Remote participation in meetings is possible via Skype or phone call, but remote participation is limited legally. Remote callers are only permitted to listen in on the meetings, as discussion and voting has to be legally conducted in person. We found that this finding in Victoria was consistent with other municipalities, as Sooke has similar policies regarding remote participation in meetings, although Sooke uses speaker phone instead of Skype. However, some councillors in Victoria were unaware of the possibility of remote participation and claimed to have never heard of it. 

The city council of Victoria also interacts as its own entity with the public by usage of social media and the city web site. The city of Victoria has a general page on Facenbook that serves as an announcement page for events going on in the city. Some city councillors also make an attempt to maintain their own personal Facebook pages and Twitter accounts. These are mostly used to interact with their constituents, but some councillors also reach out to councillors from *other jurisdictions* via Twitter; interaction between councillors in Victoria is not conducted via social media. However, one interviewee mentioned that the city has "one guy who is primarily for day to day Twitter" for pushing promotional material out and responding to general questions to the city. So there is a movement from the city towards using social media, but not everyone is buying in. One interviewee said that they don't like Twitter "because there is a problem in trying to get relevant information out of folks in a short number of characters." Whether this is a sentiment shared by other council members remains to be seen, but the fact that some councillors actively use Twitter has to be seen as a positive step towards more transparency. 

One topic that we wanted to bring up in interviews was the notion of privacy. We wanted to know how city councillors ensured private data was kept private and what types of data need to be kept private. A lot of the work and communication that councillors put out (through email, Facebook, other) can be accessed by citizens through a Freedom of Information request (FOI), which means that the majority of written communication conducted by councillors is public information. Some exceptions do exist in regards to privacy; any documents regarding legal issues and any written communication on employee relations or employee performance do not have to be given out via a FOI request. Beyond these two exceptions, councillors have no expectation of privacy in their work and the way they conduct their communication with constituents reflects this. This may also help explain why some councillors are seemingly giving up on responding to emails: at a large enough volume, if they send out a poorly worded email it may come to hurt them in the future (e.g. for job prospects) so it's simply easier to just not respond rather than do a poor job of managing communication. 

For data that does need to remain private (personal files on laptops, for example) there are a few measures put into place by the city. Each councillor is issued a laptop, an iPad, and a smartphone by the city; while the laptop and smartphone model decision is left to the councillor in question, each of these city-issued devices is encrypted by the IT department. Should these devices be lost, misplaced or stolen from councillors, the data on the devices themselves is encrypted and is much harder to gain access to. Through the interviews, we also learned that communication between city staff members and city council members is stored on servers physically located in Victoria; this is compliant with privacy laws in B.C. that state that personal information cannot be stored outside of B.C. Any sensitive documents that have to be shared between council members are typically shared as physical copies, and are shredded after usage. This approach respects privacy well, but may be open to improvement in the future. 

While communication is an important portion of the city councillor's jobs, so too is developing and ratifying the bylaws that govern the city. Through our interviews we gained some insight on how the city attempts to facilitate collaboration between councillors as well as some of the methods employed to ensure documents are up-to-date and contain all relevant data

#### Bylaw Development

As seen before, data collection for the purposes of changing or creating bylaws is largely an individual effort for city councillors. Each councillor collects data, opinions and complaints from their constituents (primarily via email) and collates these into reports or summaries that they bring to their respective committees or meetings. To facilitate data collection, one interviewee reported that they scan physical documents and then email these attachments to other people for further input. A lot of documents are emailed back and forth between constituents, councillors, and other individuals, with very little collaborative editing or writing occurring. One councillor mentioned that they use Google Docs for collaboratively working with their "closest allies" but that seems to be the exception rather than the rule. This type of version control is what we expected to find when we conducted these interviews: that no official protocol exists for controlling and ensuring the correct version of the document is being used. 

Meetings and committees are where the majority of discussion occurs regarding bylaw development. After issues are discussed and debated in these meetings, city staff moderating the meetings type up reports on what happened during the meeting. From what we gathered from our interviews, city staff do not collaboratively write these reports after the meetings - these reports are typically written on an individual basis and then shared either digitally or via printed copy for further review. It's important to note that the city councillors are not the individuals writing the reports after meetings and committees and that city staff are responsible for writing these documents, as further studies may wish to target this group for study instead of the city councillors. 

The vehicle most widely used to share documents between city council members is sharing via physical distribution. One interviewee noted that while the city was making an effort to go paperless, when the time to finalize the budget comes around they "come out with this 1000-page binder about their budget which is just a printing of line accounts and business units" and that this paper-based document was the focus of discussion for a series of meetings. While some people do prefer documents to be in a paper-based format, the last part in the quote on the document being a printed version of "line accounts and business units" highlights part of the way in which the city views data. Assessing the structure of documents produced by the city may be an alternate focus of research in future studies, as identifying how the city organizes its documents may help in making data more accessible to the councillor's constituents.

We learned from our interviews that one citizen is already trying to make data more accessible on their own. This citizen is taking development documents produced by the city (the exact format was unspecified in our interview) and is "learning how to code them with .json so you can actually turn [the development documents] into functional bits of data." This speaks volumes about the effort that the city is currently putting in to make data accessible, in that a small subset of the population of Victoria is unhappy enough to start putting this effort of file translation in. The city of Victoria may need to reconsider how they are distributing documents and data digitally in order to keep up with the pace of the digital world; currently, the city offers CSV, KML, SHP and XLS files through their Open Data section of their website. An in-house effort to provide data in more parsable formats (i.e. json) may be something worth considering on the city's end. 

#### Councillor Comfort with Technology

In our interviews, we also wished to assess how councillors view the technologies they currently use. We asked each councillor specifically how comfortable they felt with their smartphone and their computer, and to rate their own technology literacy. The results we got from this section were varied and quite intriguing. 

One interviewee rated themselves as an 8 or 9 out of 10, but then immediately went on to say that "if you ask me to build a website or you know create a firewall I have no idea. Or to encrypt something... I have the IT people to do that." For this particular interviewee, they seem to have off-loaded the need for technological literacy beyond their day-to-day operations and instead rely on their IT department to ensure that the security standards they require are being met. This interviewee also noted that they were most comfortable using the phone and answering emails, and feel that they can be more precise in using a mouse to navigate menus over a touch screen. This seems to highlight that for *their* particular needs (day-to-day communication) they feel particularly comfortable in what they know versus the technologies that are more modern (i.e. personal touchscreen-based devices, like an iPad). 

Another councillor that we interviewed stated that they "will always be a novice" in regards to technologies, which is a much different mindset than the previous interviewee. This councillor felt that they would prefer to try something first and fall back on the nearby experts if what they attempted failed. When asked about what technologies they felt comfortable using, they mentioned that they had used Skype to listen in on meetings while in Paris and that they were fine with telephone calls and telephone conferences. However, they mentioned that getting devices to sync up properly (their smartphone, their tablet and their computer) was frustrating at times, because they knew that something wasn't working properly but they didn't have the knowledge of what particular component was screwing up. In this particular case, they had to call a member of IT to help them get everything properly synced again. 

A different councillor that we interviewed felt that they were a "7 in using smartphones and computers" but didn't provide much information beyond that. This councillor did mention that they only used Facebook and Twitter during their election campaign but that they don't like using those mediums outside of their election campaigns. 

One of the councillors identified that their smartphone "can definitely do things that are powerful than I know how to use but I guess I don't know how." They recognized that while there were apps available to their smartphone that could "probably make [their] life easier" but that they didn't immediately need them and felt no need to install or try them. With their phone, they felt comfortable in performing all the functions they needed to do, but felt that they could be more adept in using computers. They specifically brought up the desire to be better at graphic design and that it was "a specific skill set that my computer can handle but I can't." While graphic design is not necessarily a skill limited to computer-based graphic design, the sentiment that they can't handle certain tasks that their computer can is an important one to take note of.

Through our sample size of 4 councillors interviewed, we found that half of them felt that they were technologically literate and that the other half felt that they were only scraping the surface of the field of computing. One of the problems we found when we were going over the results this question was that we never provided apt comparisons for what different numbers on a 1-10 scale would mean - in fact, the interviewees introduced that rating scale independently, when prompted with the question, "How would you rate your comfort level with technology?" Some councillors rated themselves very highly on their technology literacy, but without a provided frame of reference this number means very little. However, what we can gather from it is that based off what each councillor understood regarding the technologies available today, the councillors that were more aware of what technology was capable of felt that they were not as literate. In contrast, the councillors that limited their view of technology to just phones or just computers felt that they were very technologically literate *with regard to these technologies.* This sample size of 4 councillors is nowhere near enough to be able to generalize a conclusion on councillors and perceived technology literacy, but it is an interesting finding nonetheless. 

### Issues Identified

Through the interviews we managed to gain some insight on problems that both councillors and city staff face in their day-to-day operations. Here we go over some of the immediate issues that were presented in the interviews, and some other key points that we felt were problematic (or could be problematic). Some points from observing city council meetings are also brought up in this section, as there are some issues with how the city currently facilitates their meetings.  

On preliminary inspection, there is potentially room for improvement at the council’s meetings. As previously mentioned, currently the city uses a paper-based solution to keep track of the speaker's list (which councillors are talking and in what order), but this could be improved. One possibility could be some type of system to automate the speaker’s list, perhaps using an app on a smartphone to indicate speaker order as opposed to paper. The city council does employ an app called AgendaNotes that allows for note-taking on the agenda, according to the IT specialist we spoke with, but none of the councillors we interviewed mentioned using this software at meetings. Perhaps more education about the benefits of the software as opposed to paper would aid in adoption of this technology.

One of the first issues that we discovered through our interviews was that the wifi in city council chambers is particularly weak. One councillor noted that it took him a while to download documents during meetings (sometimes 2000+ pages) and that many people had to tether off their iPhones or other smartphones in order to get internet access during city meetings. This type of issue shouldn't be encountered in 2015, and should be addressed sooner rather than later.

However, this point made by the councillor inadvertently raised another key issue that needs to be addressed by the city. Currently the city employs no methods to facilitate file sharing beyond emailing documents back and forth. While the problem of having weak internet to download 2000+ page PDFs during meetings is apparent, one possible fix (that would take more time to implement) would be to set up a file sharing server or a network drive for use in sharing documents. This way, when a councillor enters the building and loads up their device they don't have to go and search for the file to download, wait for the download to complete and then be able to view it, because it's already available to them and is ready to go. Services such as Dropbox exist for this type of purpose, but Dropbox in particular may not be an applicable solution to the city of Victoria due to B.C.'s data privacy laws. Whatever the final solution may be, this should be employed alongside strengthening wifi access in city hall. 

We brought up this issue in the Bylaw section but felt it was worth mentioning again: citizens are starting to feel that the data made available by the city is lacking and that improvements need to be made. The fact that citizens are taking the documents made available by the city and translating them to .json format should be sounding alarms to workers in the city, because this means that the format in which they are offering data isn't being accepted by the public. <need more here, probably need better phrasing too>

One point that came up through our interviews, although not explicitly, is that the IT department is separated from many facets of the city's operations. The city's IT crew is located in a separate building from the city, and essentially maintains the status quo that the city sets regarding technology. All choices regarding technology used by the city are not decided by the IT department; through our interviews, we learned that the software suites that are used by the city are decided by the finance department for the city. While cost is an important factor in deciding what software to use, it is not by any means the only factor that should be taken into consideration. Given that technology is the strong point of the IT department, this group should have a larger say in what software suites are used by the city and what technologies are employed by government employees. 

One of the final issues that we noted was brought up in passing through one of our interviews. The city of Victoria offers a livestream for viewing their city meetings, and they conduct this through a service called Granicus. While we have not been able to ascertain the quality of the livestreamed video (as it was not the focus of our study) by taking a look at the service used we see room for improvement. Below is a screenshot of the view a user would see when they attempt to access an older video via computer. 

![alt-text](https://github.com/cscw2015/maverick/blob/master/Final%20Report/granicus_agenda_video.png "View for accessing old webcasts")

As seen from this screenshot, there is a large chunk of uneven white space and the video appears to be an afterthought, as it's pushed to a corner of the screen rather than being the main focus of the page. Again, the structure of the website and its usability was not a core part of our research, but keeping their website up to date is an important task for the city. 

## Conclusions 

In order to assess whether our study gathered the information we desired, we need to reaffirm what our research questions were. The three questions we asked in this study were: 

1. What technologies already exist or are being used to help city councillors in their meetings, with respect to document sharing and communication?
2. What issues are they currently facing with their present technology?
3. How can we improve communication between city councillors?

For technologies that are being used to help city councillors in document sharing and communication, we need to look at the meeting environment and the day-to-day work that each councillor conducts. For meetings, Microsoft Word is displayed on a projector screen to view the agenda or current document. We know that groups that present to the city during the meetings we observed use PowerPoint presentations to share information, but with regards to other document types (e.g. PDFs of reports) we are unsure of how these are being distributed. In day-to-day work, document sharing is facilitated primarily via email, with some councillors using applications like Google Documents only with people that they trust. With respect to communication, councillors primarily use email as a technological medium to interact with each other. Due to the way the city operates, these interactions are fairly limited (as any points that are discussed in detail need to be brought to a meeting environment) so instead councillors interact with their constituents. They do this via email and phone primarily, with a few using Twitter or Facebook to communicate with constituents. 

The only explicit issue that was brought up during interviews was the weak wifi in city council chambers. However, after going through the interview results we have determined that some councillors feel overwhelmed by the volume of email that they have to deal with on a daily basis, and that for some individuals it may be overwhelming enough to dissuade them from trying to respond to emails at all. There may be a mismanagement or misallocation of emails between the councillors (some reported getting only 200 emails a day while others are getting up to 1000 a day), but the key issue here is that councillors have no real way of filtering the emails without opening up each one to see if they can respond to it adequately. One other major issue that we have discovered is that the city offers no solution to its councillors in terms of version control, which is a topic that we explicitly searched for through interviews and through observation. 

For improving communication between city councillors, this is a misconception that we had when we began our research. As outlined before, we believed that in order to conduct their jobs, councillors needed to collaborate with one another outside of the meeting environment. This is not the case, as the majority of communication that occurs is between councillors and constituents. While the possibility of improving councillor-to-councillor communication still exists (and should eventually be explored) councillors place much more weight on interacting with their constituents. Future research should take a look at this and explore the possibility of improving councillor-to-citizen communication over attempting to improve councillor-to-councillor communication. 

## Impact and Future Work

This project immediately offers two things to the city of Victoria:

1. It offers an outside perspective on current communication practices within the government, which may help identify flaws in communication practices; and
2. It offers transparency on communication practices employed by the government, so citizens of Victoria can be more aware of how the city operates on a technical level.

A longer time frame for this study could have allowed for follow-up interviews, observation of private meetings (as opposed to primarily public forums), or even designing and testing a new suite of software that focuses in particular on the needs of the municipality of Victoria. Similarly, this study could also be modified to assess similar issues on a provincial or federal scale. Such modified studies would need to have a broader focus (they may involve assessing the public's desires of the government vs. the government's responsibilities towards communications and data privacy) and would require a much larger time frame. 

These types of studies are rarely conducted, in comparison to other fields of work. Typically, government organizations are audited by a specific subset of companies, but these audits tend to focus on ensuring the government is up to the current standard. Our study looks to go beyond the current standards and afford the opportunity for technological innovation, as a benefit for the public.

Other questions have arisen from this work that require more research. For example, there could be research into how the public perceives technology use in city council, versus how councillors perceive it, versus what is actually used. This would be a valuable offering in the field of CSCW. Further, recommendations could be made to city council about what specific technologies to adopt, such as for version control and for updating their website, and these would require more research into matching the various software available to the various needs of city council. This study provides the foundation for much more research to be conducted in the field of CSCW and government.

##Appendices

### Appendix 1: Team Roles

####Kimberlee Graham-Knight: Group Leader
Kimberlee helped to facilitate the function of the group. She interviewed four people in total, including the official from Sooke, and provided some of the background research for the related work section. She helped to write all three reports and edited and proofread them. She attended both city council meetings, and transcribed one of the interviews.

####Roshni Jain: Data Analysis
Roshni transcribed three interviews and was involved in the analyis of all the data we collect from interviews.She attended one council meeting  to collect data. She also provided some of the background reseach for the related work section and helped in writing all the three reports. She participated in the final presentation too. 

####Nigel Dufty: Data Collection
Nigel kept the encrypted USB stick with the interviews on it and would collect and distribute the interviews to members of the group as necessary. He sent out three requests for interview and interviewed two individuals. Nigel attended a city council meeting and watched another online to collect data. Nigel was also involved with editing and suggesting changes to all of the reports. He also participated in all of the presentations to the class.

####Tian Geng: Data Analysis
Tian is working with Roshni to create transcriptions of interviews as they are completed. He is also working with Kimberlee and Nigel to conduct interviews of city council members of Victoria. Tian is also responsible for conducting literature review alongside Roshni and Kimberlee. 

####Myan Panikkar: Editor
Myan was responsible for all written deliverables in the project. As the primary editor, his job was to ensure that documents needed for the project are coherent, cohesive, and that they are delivered as complete products. This involved some leadership alongside Kimberlee, namely for delegating section content amongst group members as necessary. He also attended city council meetings to help provide background research and helped in designing and giving presentations. 

## Appendix 2: Milestones

The following table outlines our milestones that we used to ensure completing of tasks throughout our research. 

| Date | Task to Complete |
|------|------------------|
|October 15| City Meeting 1 |
|October 16| Project Proposal Finished |
|October 19| Interview Template Finalized |
|October 19| Requests for Interview sent|
|October 19| Ethics application complete |
|October 29| City Meeting 2 |
|November 4|Requests for Interview sent|
|November 4| Oral update on project |
|November 13|Interim Project Report|
|November 20|Completion of Interviews|
|November 23|Interview transcription completed|
|November 27|Finalization of data analysis|
|December 2|Project Presentation|
|December 5|Final Report|
|December 5|Consultant's Report|

The two city meetings attended were two hour sessions on Thursday nights. As these sessions are available for the public to attend and give input on, we used these to get context behind what the council currently does and how it communicates its decisions to the public. 

Interviews took longer than expected to complete, partially because our requests for interview were sent out later than expected. This may have affected the number of interviews we were able to obtain, as we were only able to get 6 interviews in total. 

As each interview was completed, we had to transcribe it. The dates above are the _final_ dates for interviews and their respective transcriptions; we processed the data as it flowed in. With all of the interview data in a usable format, analysis was conducted on it to determine any flaws or issues regarding technology usage within the municipality of Victoria. 

## Appendix 3: Interview Questions

The following list contains general questions used throughout our interviews to facilitate discussion. Not all questions are listed, as some are context-specific to interviews and/or break confidentiality.

- What kind of data do you need to share on a day to day basis to do your job? For example, who do you need to communicate with to do your job?
- How much of your job is data that you have to keep private?
- How do people request access to your emails?
- So about creating bills. How do you go about creating those? Do you collaboratively work documents together and if so, how do you do that? What technologies do you use usually? Email?
- So when you collect different data to collect a bill you get a bunch of different information from people right? How do you organize, collate, and sort that data?
- How do you make sure everyone has the same version of documents when you're collaborating with other city councillors?
- How many city council related emails would you say you get in a day?
- When you are speaking with people who are other councillors, what types of technology do you use? Do you post them in person? What about texting?
- When you're dealing with other councillors, how do you communicate with them?
- Who organizes the meetings then? How do they organize the meetings?
- How comfortable do you feel with your smartphone and your computer? Do you feel like you're using it to the best of your ability? Do you feel like you could be using it more?
- How would you rate your technology literacy? How good would you say you are with technology?
- Do you feel like you're limited in any way with your current tech setup? Are you able to do everything you feel like you need to do? Is there something you would change or that you wished you could do a little better?
- Have you ever seen any miscommunication at the council level?
- How does a member of the public find out about bill creation and follow legislation at the council level?
- How would you get the public input?
- What types of information do you browse for, in terms of your job, on the Internet?
- How do you ensure that things don't get discussed [between councillors] and that they go to a meeting, who ensures that?
- How do you organize and run meetings, council meetings?
- What kinds of technology do you use in the meeting rooms?
- Are councillors allowed to remotely participate in meetings?
- What do you feel most comfortable doing with your technology that you do on a frequent basis?
- Is there a way for people to share their documents generally in meeting if they need to?
- Do you handle sensitive information by using different technologies and avoid using email?

## Appendix 4: Tools Used by Council

Through all the interviews we discovered a set of software tools that the city is currently using to manage their day-to-day operations. As these tools do not fit into any other section of the report, we list them here along with their general function. Future studies on the city of Victoria may want to look at these tools (or their replacements, should they be replaced) and assess whether they are being used effectively. 

- Development tracker that has documents about every development that’s happening in the city which was made online this year (2015)
- NationBuilder, a constituency management  for tracking emails. It’s a political organizer. The website basically runs on the NationBuilder platform which has  a database attached to it.
- Atomic Crayon, website provider
- iCompass provides software for information management services for council and committee operations.
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
- Team Budget by Questica for keeping track of finances in a group
- AgendaNotes is used for councillors to make computerized notes about the agenda

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
15.  Benkler, Yochai. (2005). "The New Open-Source Economics." Online video: http://www.ted.com/talks/yochai_benkler_on_the_new_open_source_economics?language=en#t-552871
16.  (2003). Flaw in RPC Endpoint Mapper Could Allow Denial of Service Attacks (331953). Accessed online: [https://technet.microsoft.com/library/security/ms03-010](https://technet.microsoft.com/library/security/ms03-010)
17. Grassmuck, V. “LiMux — Free Software for Munich” (2005) http://waste.informatik.hu-berlin.de/grassmuck/texts/limux.pdf Accessed November 11, 2015.
18. Poole, M. S., Keyton, J., & Frey, L. R. (1999). *Group communications methodology* (pp 92-112). L. R. Frey, D. S. Gouran, & M. S. Poole (Eds.). Thousand Oaks, CA: Sage Publications. 
19. Löfgren, K. (2013). *Qualitative analysis of interview data: A step-by-step guide*. Accessed online: [https://www.youtube.com/watch?v=DRL4PF2u9XA](https://www.youtube.com/watch?v=DRL4PF2u9XA)
