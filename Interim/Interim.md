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
			2. [Methdology used in developing Cuparla](#methodology-used-in-developing-cuparla)
			3. [Cuparla Software Design](#cuparla-software-design)
			4. [Evaluation of Cuparla](#evaluation-of-cuparla)
		2. [E-government](#e-government)
			1. [Reasons behind innovating with e-government](#reasons-behind-innovating-with-e-government)
			2. [Methodology to evaluate use of e-government](#methodology-to-evaluate-use-of-e-government)
			3. [Implementation of e-government in Corpus Christi](#implementation-of-e-government-in-corpus-christi)
			4. [Challenges of e-government](#challenges-of-e-government)
		3. [Open Source](#open-source)
			1. [Reasons behind innovating with Open Source](#reasons-behind-innovating-with-open-source)
			2. [Methodology to evaluate usage of Open Source](#methodology-to-evaluate-usage-of-open-source)
			3. [Implementation of Open Source in Munich](#implementation-of-open-source-in-munich)
			4. [Timeline for Munich's Migration](#timeline-for-munichs-migration)
		4. [Government 2.0](#government-20)
			1. [Research Strategies Followed](#research-strategies-followed)
			2. [Research Findings](#research-findings)
			3. [Impact of Web 2.0 on Government](#impact-of-web-20-on-government)
3. [Methodology](#methodology)
4. [Impact](#impact)
5. [Appendices](#appendices)
	1. [Appendix 1: Team Roles](#appendix-1-team-roles)
		1. [Kimberlee Graham-Knight](#kimberlee-graham-knight-group-leader)
		2. [Roshni Jain](#roshni-jain-data-analysis)
		3. [Nigel Dufty](#nigel-dufty-data-collection)
		4. [Tian Geng](#tian-geng-data-analysis)
		5. [Myan Panikkar](#myan-panikkar-editor)
	2. [Appendix 2: Milestones](#appendix-2-milestones)
		1. [Status on Original Milestones](#status-on-original-milestones)
		2. [New Timeline](#new-timeline)
	3. [Appendix 3: Preliminary Results](#appendix-3-preliminary-results)
6. [References](#references)

## Introduction

- goal is to discover what methods the city council of Victoria currently uses for collaboration and communication
- includes public council meetings as well as their internal communications
- research questions:
	1. What technologies already exist or are being used to help city councillors in their meetings, for document sharing and communications?
	2. What issues are they currently facing with their present technology?
	3. How can we improve communication between city councillors?
- one area we want to focus on is preparation and management of council meetings via technology
	- what technologies are used to prepare for the meetings
	- how is agenda constructed?
	- how are by-laws introduced, modified and finalized via technology?
	- how is the by-law process made transparent to the public
	- what is used *during* meetings to facilitate and share information?
	- what software is used for remote access to meetings?
- methods of gathering:
	- interviews with city councillors from Victoria
	- smaller number of interviews with Vancouver city councillors (as a control group)
	- attending public council meetings to see what current practices are
- much of existing research about city governments is about how to improve government-citizen relations
	- not as much on how technology plays a role in this, or if there is it's outdated
- we want to focus on inter-governmental collaborations and how city councillors coordinates themselves to solve issues
- research of this type can provide beneficial information to councillors on how to improve their operations, and provide transparency to citizens on how government collates information and develops laws for the city

## Related Work

Before looking at previous implementations of computer-supported collaborative work (CSCW) in government settings, we need to understand some of the difficulties of integrating CSCW into meetings and why it is important for municipal governments to want to incorporate CSCW into their workflow. 

### CSCW in Meetings

According to Schümmer, there are three distinct facets of designing an electronic face-to-face meeting system:
1. the peopleware perspective, the design of social processes that are executed by team members,
2. the generic groupware perspective for designing supportive software tools, and
3. the roomware perspective that considers the configuration of artifacts that constitute the tangible meeting space [1].

Arguably, the hardest facet of designing an electronic meeting system for a group is understanding their needs. Given the level of support in the open source community today, innovation in designing supportive software tools is easier to come by than before. <maybe insert examples here later> Along with this, before designing a meeting space for a group to allow for better collaboration you must understand _who_ you are building the room for, _what_ they need in their room to effectively collaborate and _why_ collaboration is necessary in their line of work.

Addressing the first point that Schümmer makes is part of the reason behind our study. To ensure that our government has room to innovate, an assessment of their current technological integration and their current communication practices is necessary. 

### Local Government Innovation

Innovation is an important part of any continued collaborative group work. Walker says innovation is a core task of public institutions and that "innovation has been promoted around the world as a key tool to improve public services" [4]. This is one of the reasons we are targeting the city of Victoria with our study: that public services always stand to be improved, and they are in one of the best positions to affect this change. Ihkre notes that local governments are more likely to innovate than governments at state or federal level because of "their small size and capacity to make decisions quickly and decisively," [2] and this is another reason as to why we are targeting the city of Victoria. While standards do exist at the provincial and federal level for regulating what technologies can be used in government organizations, a municipal government stands to gain more from integrating new technology on a regular basis and is in a good position to do so. 

- Haus claims that "cities hold the potential to construct, articulate and promote common good of their societies by forming policy agendas" [3]. 
- local governments also get a lot of pressure to "do more with less" [4]
- we will incorporate cost estimate of any changes we may propose in final recommendation report to council

- transition into history

###History of CSCW Use in Government

Here are some examples of previous attempts to integrate CSCW into government organizations. These examples are in chronological order, and attempt to focus on the processes used to research the organizations involved as well as how they built or identified what software suites would be most applicable for the given organization. 

####Cuparla

- Number of socio-tech  projects are coming on a timely manner to improve the city council administration in terms of effective communication by following the below level of practices:
	1. the need of technology for support is analysed 
	2. then the system is developed
	3. then the system is implemented in the organization to serve the particular need.

#####Creating Cuparla

- Detailed analysis of Stuttgart city council work revealed certain characteristics
	- Any time any place support to council members was required since they didn't have fixed office locations to prepare for city-hall meetings.
	- Council members collaborate and behave differently in different contexts. Informal and open within their party groups and were more controlled and formal in official council meetings.
	- No proper structure was followed in communication; each member had right to initiate and involve other members of the administration in any order
	- Minimal computer usage within council itself
- Objectives of the Cuparla Project:
	- To bring effectiveness and flexibility in the work of the councils.
	- To have more access to information by council members
	- To reduce communication barriers between council and administration and within the council.

#####Methodology used in developing Cuparla

- Detailed analysis of council work was done by Needs Driven Analysis
- Need for group support was found which served the basis for the Cuparla design.
- Implementation of the design within the council was done as a preliminary level.
- After few months, the analysis of the Cuparla usage was performed in two cycles:
	- In first cycle, the Cuparla was tested by 11 city council members
		- results obtained from them are then used to do second analysis, design, implementation and evaluation phase
	- In the second cycle, this software was tested on 55 or 56 active city council members
- A field test of Cuparla was performed on the small city of Kornwestheim to determine the effectiveness of the tool [5]
	
#####Cuparla Software Design

- designed with aim to support political entities
- supports functions such as information, communication, coordination, collaboration
- Based on the city council actual work procedure, the design consist of rooms, shown in figure below: 
	- private room - where the council member works at home 
	- party room - where council member collaborates with their party colleagues
	- room for committee meetings
	- room for work groups
	- private post office
	- library for filed information
- Documents created in private room can be shared by placing in the room they wish to share in [6]

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/cuparla.jpg">
</p>

##### Evaluation of Cuparla

- Cuparla was evaluated on five sets of criteria and four levels of aggregation[7]: 
	- Cost 
	- Time
	- Quality
	- Flexibility
	- Human Situation, further evaluated on: Individual, Group, Process Organization
- criteria and levels of aggregation aligned to create a 4x5 matrix, shown below

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/Evaluation of Curparla.png">
</p>

- any notes made in eval were attributed only to lowest applicable level
	- e.g. costs of server are attributed to **group**, PC in office is attributed to individual **user**
	- seems to be an effort to reduce redundancy in data from evaluation

####E-government

- "delivery of government information and services through the Internet 24 hours a day, 7 days per week" [8]
- does not consider non-Internet technologies
- three governmental relationships to consider[9]:
	1. **Government to Citizen**: citizens paying bills or taxes, voter registration, business permits and license applications
	2. **Government to Business**: purchase for property, equipment, office supplies
	3. **Government to Government**: our category of concern; includes enabling project teams to collaborate using CSCW technologies, provide news/information and online report generation/procurement tools, publishing documents and manuals online to reduce printing costs[10]

#####Reasons behind innovating with e-government

- increasing demands for timely and accurate communications
- emerging opportunities in electronic communications
- more ownership of home PC’s
- goal of citizen and customer communication [11]

#####Methodology to evaluate use of e-government

- in Corpus Christi, Texas, used case study approach
- data included experiences of co-author, interviews with select individuals and archival records

#####Implementation of e-government in Corpus Christi

- site went live in late October 1999
- cost of implementing site in 1999 was approx. $13,000.
- Internet site replicated as Intranet for city employees, includes city directory, city policies, training calendars, a bulletin board, other communications important to employees
- forms and applications online, from printable to e-mailable, building permits, job applications, utility bills, parking and traffic ticket payment and info
- staff trained by Communication and Quality Management dept. in Adobe Acrobat 4.0, Adobe ImageReady and Macromedia DreamWeaver

######Challenges of e-government

- people creating fake sites and getting the city to include them (eg. Fire Dept) 
- putting building permits online
- 100,000 hits/month on website first year, 10,000/day after
- people not using online services after major investment
- requests to put job applications, engineering plans online
- different than e-business in 3 main respects: Access, Structure, Accountability
- Access: business can choose its customers; city cannot
	- lack of access to e-government furthers economic inequality
	- people with disabilities need dedicated web programming to access site
	- public forums elicit hate speech, so tough to include them on city websites
- Structure: decision-making more dispersed in public sector than business
- Accountability: constraint
	- once project is funded, can be micro-managed to ensure correct performance [11]

####Open Source

- FOSS = “free, open-source software” 
- “a generic term for non-proprietary software that is generally free, can be reviewed by large numbers of users, and can be revised and shared free of charge” [12]
- can save significant amounts of money, but the cost of migration, including training of employees, must be taken into account

#####Reasons Behind Innovating with Open Source
- migrating to a new system involves risks, so it's often a top-down approach by politicians. [12]
- "factors that influence innovation:
	1. pressure from legislators or politicians; 
	2. change in leadership from within or outside an organization; 
	3. crises or visible public failures; 
	4. internal failings such as an inability to coordinate across departments or meet the demands of a program;
	5. new opportunities that occur through development of new technologies or other factors.” [12]
- independence
- effectiveness 
- cost savings 
- In the case of Munich, Microsoft discontinued its support for Windows NT [13]
- greater vendor independence (more competition in the software market) [13]
- "future-proofness" of open protocols, data formats and interfaces [13]

#####Methodology to evaluate usage of open source
- semi-structured interviews [12]
- “The interview instrument consisted of a set of identical questions related to motivation, implementation, and results. Each questionnaire also contained a set of questions specific to the position of the interviewee. To facilitate coding and analysis of the interviews I used N-Vivo, a qualitative analysis software program. I also relied on internal reports, audits, and news releases published by each city to develop the necessary background for the research and to substantiate information collected through interviews. Finally, I surveyed news accounts to corroborate data produced by the cities and the interviews” [12]

#####Implementation of Open Source in Munich
- “The alternatives were: 
	1. MS XP + MS Office XP 
	2. MS XP + OpenOffice 
	3. GNU/Linux + OpenOffice 
	And two transitional solutions: 
		3a. GNU/Linux + OpenOffice + PC Emulation (WINE / VMWare) 
		3b. GNU/Linux + OpenOffice + Terminal Server 
Both transitional solutions presented architectural and operational complexities, not least with respect to security and an increased need for training. They were therefore considered undesirable as such and only to be deployed where no other solution could be found” [13]
- “the project leaders determined that a successful migration required consistent adherence to a number of technological and political principles: 
	1. applications should be OS-independent; 
	2. new client-server applications would only be developed or commissioned as web applications according to the J2EE model; 
	3. cooperation of all software partners would be necessary as software is customized, and as applications are redeveloped; 
	4. the project had to have the support of both political leadership and heads of the administration; 
	5. proactive education and involvement of employees would be essential” [13]

######Timeline for Munich's Migration
- November 2001: Munich decided to investigate open-source options in operating systems and office suites
- April 2002: Commissioned a consulting company for options
- May 2003: Made the decision to migrate to open-source software and web applications.
- 2004: Migration to open-source began.
- Note: The first city to use open-source was Schwäbisch Hall in Baden-Würtemberg, who migrated their servers in 2002 and all their desktops in 2004 [13]

####Government 2.0

- Government 2.0 , reflecting the concept of web 2.0 [14] is the extension of the Web 1.0 technologies (which are already been in use by most of the city councils under e-government). 
- Web 2.0 emphasis to e-democracy wherein multimodal, non-hierarchal, collaborative and deliberative networks can be built.
- It emphasizes a more interactive process with the potential use of media for promoting citizen participation. [15]

#####Research strategies followed
 
- The following questions were asked:
	- Are web 2.0 applications relevant for the government context?
	- If they are, in what way is web 2.0 likely to have an impact on government?
	- How significant could this impact be?
	- How are web 2.0 applications implemented in the government context?
- To answer the above questions, the below methods are followed:
	- A web survey of existing innovative web 2.0 initiatives in government-related activities was conducted 
	- A desk-based review of existing web 2.0 applications in the private sector, in order to understand applications that could also have potential for government
	- A set of case studies of existing experiences, based on desk research and interviews with the project managers.

#####Research Findings
- The methods followed helped them to find following results
	- It gave an overview where the web 2.0 technologies can be used
	- How each of the domains could get impacted  through the adoption of web 2.0 applications.

#####Impact of Web 2.0 on Government

<p align="center">
<img src="https://github.com/cscw2015/maverick/blob/master/Interim/Web2.0.png">
</p>

- Here, users are both civil servants and citizens
	- The centre circle represents group of users who are active in designing and delivering the service. The web 2.0 is used by analysts to create wiki-based intelligence reports in Intellipedia, or citizens creating a new petition online.
	- The second circle represents the group of users who play a fundamental role in ensuring the quality and relevance of content submitted by other users. For example: the rating of evidence submitted to Peer-to-Patent
	- The third circle represents the users who used the web 2.0 applications and get benefitted from the other user's services. For instance, review on any e-petition by other users helped the users to come up with some decision.
	- The fourth circle represents to those who used the online services to get the quality data without any voluntary engagement. In the private sector, a classic example is the "most read articles" page in online newspapers.[16]

##Methodology

We will be collecting data from two main sources. Our primary method of data collection will be through interviews with city councillors, with our secondary method being observance of public city meetings. We chose these two methods of data collectionn for a few reasons, with the primary reason being that our research questions involve assessing the quality of communication and document sharing that city councillors currently have access to. Talking directly to these city councillors is the most effective way of assessing this information. Our secondary form of data collection allows us to observe the city's methods of sharing documents with the public and their use of technology to moderate and augment their communications between the city and the public. It also serves as a form of risk mitigation, should we be unable to conduct all of our planned interviews. Alongside these reasons, we chose these methods because they have been shown to be effective in previous studies of a similar form. Poole notes that group observation and asking questions of individual members are the two best ways to obtain information on group dynamics, and he specifically recommends in-depth interviews in order to "obtain symbols that members naturally use to describe their behaviour" [17]. 

Our goal is to conduct eight 30 minute interview sessions. The council members that we will be interviewing will be decided primarily on availability, as the time available for this research is limited. We want to interview six members of the Victoria city council (including the mayor), a member of Sooke city council, and public figures that involve themselves with the city council on a regular basis. These interviews will be semi-structured, so that we can elaborate on topics that come up through discussion in the interviews. 

As mentioned before, we also attended public city meetings to observe the usage of computers in facilitating meetings. These meetings typically occur every two weeks on Thursday nights at 7:00pm, and are held at City Hall in Victoria. The two meetings attended were held on October 15th and October 29th. The primary goal with attending these meetings was to observe and assess the conduction of the meetings based on the following metrics: what technologies do they use to administer and share documents, how do they allow for crowd contribution, and how is discussion moderated and facilitated. 

## Impact

- project can immediately offer two things:
1. Outside perspective on current communication practices within the government, which may help identify flaws in communication practices
2. Transparency on communication practices employed by the government, so controversies like the current BC government FOI requests can be avoided
- scale and time frame of project don't allow for in-depth analysis
	- similar studies could be conducted on other municipal governments, provincial governments or even federal
	- larger time frame would allow for observation of different meetings and follow-up interviews

##Appendices

### Appendix 1: Team Roles

####Kimberlee Graham-Knight: Group Leader
Kimberlee is taking on the role of group leader. She is responsible for regularly checking in on each group member to ensure that they are fulfilling their roles and that any issues or questions they have can be addressed as soon as possible. This includes delegating tasks as necessary. Kimberlee is also responsible for conducting some of our interviews with city councillors, and has attended some of the city council meetings to help establish a background for our research. 

####Roshni Jain: Data Analysis
Roshni is responsible for overseeing the analysis of all the data we collect from interviews. As interviews are completed, she and Tian will be transcribing the audio recordings provided from these interviews. After all the transcriptions are completed, Roshni will be responsible for leading the analysis on these interview results. She is also responsible for reviewing any relevant literature and collating the background research necessary to ground this project and give it context. To assist with providing context, Roshni has attended some of the city council meetings. 

####Nigel Dufty: Data Collection
Nigel is responsible for a majority of the data collection involved in the project. He is working with Kimberlee and Tian to organize and conduct interviews of Victoria city council members. To ensure that the audio files from the interviews are kept secure, Nigel is acting as an intermediary for transferring audio from the interviews to Roshni and Tian via an encrypted USB stick. Nigel has also attended city council meetings to help provide context for interviews and for our background research. 

####Tian Geng: Data Analysis
Tian is working with Roshni to create transcriptions of interviews as they are completed. He is also working with Kimberlee and Nigel to conduct interviews of city council members of Victoria. Tian is also responsible for conducting literature review alongside Roshni. 

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

As each interview is completed, we have to transcribe them. The dates above are the _final_ dates for interviews and their respective transcriptions; we will be dealing with the data as it flows in. Once we have all of the interview data in a usable format, analysis will be conducted on it to determine the best method of approach for the city council. This best method (or set of methods) will then be presented in a report to the city council at the end of the semester. 

## Appendix 3: Preliminary Results

- some notes from meetings
	- all councillors are already using laptops/tablets at the meetings
	- start meetings by announcing changes to agenda from when it was published
	- many items on the agenda are "late items"
	- voting is done by simple hand raise
	- councillors indicate they would like to speak by raising hand
	- mayor writes down a list on paper of which councillor(s) are speaking next
	- people presenting give slides to council beforehand
- small analysis of meetings

## References

1. Schümmer, T., Tandler, P., & Hakke, J. M. (2012). The next-generation business meeting: from i-lands to flexible meeting landscapes. *Universal Access in the Information Society, 11*(3), 239-258.
2. Ihrke, D., Proctor, R., & Gapris, J. (2003). Understanding innovation in municipal government: City council member perspectives. *Journal of Urban Affairs, 25*(1), 79-90. 
3. Haus, M., & Sweeting, D. (2006). Local democracy and political leadership: Drawing a map. *Political studies, 54*(2), 267-288.
4. Walker, R. M. (2006). Innovation type and diffusion: An empirical analysis of local government. *Public administration, 84*(2), 311-335.
5. Schwabe, G., & Krcmar, H. (2000). Piloting Socio-Technical Innovation. ECIS 2000 Proceedings, 27.
6. Schwabe, G., & Krcmar, H. (2000). Digital material in a political work context-The case of Cuparla. ECIS 2000 Proceedings, 150.
7. Schwage, G. (2000). From Analysis to Evaluation - The Case of Cuparla. Found online: [http://www.zora.uzh.ch/57144/1/20120125131854_merlin-id_3158.p](http://www.zora.uzh.ch/57144/1/20120125131854_merlin-id_3158.p) 
8. Reddick, C. G., & Frank, H. A. (2007). The perceived impacts of e-government on US cities: A survey of Florida and Texas City managers. Government Information Quarterly, 24(3), 576-594.
9. Tat-Kei Ho, A. (2002). Reinventing local governments and the e-government initiative. *Public administration review, 62*(4), 434-444.
10. Reddick, C. G. (2004). A two-stage model of e-government growth: Theories and empirical evidence for US cities. *Government Information Quarterly, 21*(1), 51-64.
11. Jorgensen, D. J., & Cable, S. (2002). Facing the challenges of e-goverment: A case study of the city of Corpus Christi, Texas. SAM Advanced Management Journal, 67(3), 15.
12. Cassell, M. (2008). Why governments innovate: Adoption and implementation of open source software by four European cities. International public management Journal, 11(2), 193-213.
13. Grassmuck, V. “LiMux — Free Software for Munich” (2005) http://waste.informatik.hu-berlin.de/grassmuck/texts/limux.pdf Accessed November 11, 2015.
14. Reddick, C. G. (Ed.). (2010). Politics, Democracy and E-Government: Participation and Service Delivery: Participation and Service Delivery. IGI Global.
15. Kloby, K. (Ed.). (2012). Citizen 2.0: Public and Governmental Interaction through Web 2.0 Technologies: Public and Governmental Interaction Through Web 2.0 Technologies. IGI Global.
16. Osimo, D. (2008). Web 2.0 in government: Why and how. Institute for Prospectice Technological Studies (IPTS), JRC, European Commission, EUR, 23358.
17. Poole, M. S., Keyton, J., & Frey, L. R. (1999). *Group communications methodology* (pp 92-112). L. R. Frey, D. S. Gouran, & M. S. Poole (Eds.). Thousand Oaks, CA: Sage Publications. 
