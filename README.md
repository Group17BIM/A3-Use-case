# A3-Use-case

3A: Analyse use case

1.	Goal: Deliver to the user/client important information about the beams that are in investigated building.
	
2.	Model Use (Bim Uses): Our model use can be named as “ Plain Visualization” for structure analysis that is highly needed use case in construction industry. For that uses, type of Analyse is specified as Forecast with Design phases.
We would like to focus on its technical aspects such as geometry and properties so structural engineers and contractors are people that this use case in address for. It require disciplinary validate structural analysis and material properties analysis. It is forecast type of analysis where communication between processes is needed. This structure will avoid lost data in file exchange when we use FEM software.

3B: Propose a (design for a) tool / workflow

3.	Process: 
	
 BPMN model for current Structural use case.
 
BPMN model for your proposed tool.

4.	Description of the process of your tool / workflow:
Usually first step would be to get source data from reference files/assumptions. We start with number of beams on each building floor (BIM file is transformed into IFC). Next step would be finding their coordinates in space. From that data we will take necessary parts that we want to submit in our calculation process for instance: dimensions. Then we will be able to express loads that are carrying through the structure. When we get results that will suits to our expectations, workflow circle have done its job. Otherwise some changes should be made.

3C: Information exchange

5.	Information Exchange: 
   
Here is preview of Use_case_INFX_Team_05.xlsx file.

6.	IFC: For our process we need detailed information about construction materials e.g. load bearing, stabilizing layer. Some of IFC data: IFC beam, iFC name, IFC type, IFC wall, IFC geometry, IFC space, IFC material. In general Level Of Development should be 400 but lower rating could also be useful. More precise values for parts are: 400 for Level Of Information, 300 for Level Of Reliability, 325 for Level Of Geometry. Detailed value for each entity is reached by analyzing Dikon files and they are shown in early mentioned xlsx file. Results have to be compared with requirements sheets like BR 18 where is possibility to stuck to correct limits. For intended situations all entities properties should pass this challenge but if there are some mismatches, corrections could be done using provided tools.
We are assuming providing information with other stakeholders about final structural model and the prototype of this model too. From them we receive feedback that gives us ability to make improvements in IFC model which is ours input data to the “material of interest”.
  
3D: Value What is the potential improvement offered by this tool?
This is the common question when developing tools and processes as an intrapreneur in a company. Here we should consider the business and societal value of this tool – does it save time to the company, does it make employees happier / more productive? Could it reduce material use in society?

7.	Describe the business value (How does it create value for your business / employer): It can have an important meaning to industry (represented by appropriate crew) that would like to speed up their procedures of structural analysis from first steps of actual project. On that early stage of development any changes may have crucial consequences in the future. If we came across any kind of mistake (for example failure to comply with the requirements of the BR 18) it would be much lower in costs to solve out than later. There will be also human resources savings because some of them won’t have to work on mistakes that have been terminated at the beginning. This time can be very important to others involved in building project – for example architects.
	
8.	Describe the societal value (How does it make the world better):
World will be better because company that want to use this tool will save time. Calculation and research will be made for them by semi-automated program and in that time they could do other useful things that could improve world even more. Same goes with individual user that now is no more stressed with deadline of finding “structural results” in endless documents pile. Because, all he have to do is to input IFC file and watch results in html window. This phenome would make him happy and happy customer is very important in nowadays world. Probably avoiding mistakes from incorrect calculations will save some materials on unnecessary constructions, so it is next point how it could have positive influence on environment.

3E: Delivery
In this part we are focus on the input data that you need for our final tool / workflow.

9.	Your tool/workflow: Description of how our tool / workflow would solve the use case is clear.
We have used text editor that is compatible with python adding ifcopenshell package with blenderbim add-on that is required. And with that, getting important for use case data (from provided ifc file) we obtain database that could be used for next steps according to our tool path. Some basic analysis can be performed with already held info. For example calculations of loads that each building part can carry out. Functions gives us possibility of further investigation on more detailed information. Those activities are briefly presented in point 4 text. This whole tool is important part of solving our use case and even can exist on its own (like only function in use case).











10.	Delivery:
Step I: Get commissioned document from customer.
Step II: Make IFC from this file (if it is not yet).
Step III: Find beams in this building.
Step IV: Get values of parameters that we had described in our workflow.
Step V: Check results with norms like BR 18 for instance.
Step VI: Show results to the client in easy to read form of html file (that is presented below).

 

Speaking about delivery from user point of view, he may need some kind of guidance. It may be hard for him to feel confident in program because some staff could be done in different parts of software environment. That’s why we came up with our idea to create a tool that will read input file of a building and then at the end will show to customer clean and easy to read html file with visualization of important parameters. He can click on each floor to reach values of results.
