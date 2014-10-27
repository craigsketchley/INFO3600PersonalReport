# Craig Sketchley - Individual Report

## Statement & Extent of Work Done

### XP Work

#### JIRA Expert

I completed the following tasks in my role as JIRA Expert:

* Acquired an academic JIRA licence from Atlassian - [email](JIRAkeyEmail.pdf).
* Installed and configured JIRA with Rohan - [instance](codiographers.cloudapp.net:8080), [team meeting log](../../TeamMeetings/18-8-2014.md). JIRA used an Azure cloud server kindly setup and managed by Rohan. The JIRA setup included:
    + Hooking up a database backend.
    + Setting up the Agile plugin for JIRA.
    + Configuring team member accounts.
* Added a [custom fields to JIRA](JIRACustomFields.png):
    + to enable the client to ‘approve’ a story - added checkbox.
    + to allow multiple team members to be added to a story since JIRA natively only allows one person to be assigned to a task - added a multiple user text box to list users working on a story.
* Setup a [custom workflow](JIRAStoryWorkFlow.png) for the story lifecycle allowing our client to sign-off on stories that are 'In Review'.
    + Sprint Backlog -> In Progress -> In Review -> Done.
* Maintained the JIRA instance throughout the semester - [JIRA broke](JIRAMaintainence.png).
* Integrated our Bitbucket repository into JIRA to enable [linking to user stories within our commit messages](JIRALinkedCommits.png).
* Offered [support to team members](JIRASupport.png) regarding JIRA usage:
* Facilitated completion of sprints and [updating the storyboard](JIRASprintLog.png) after end of [sprint meetings](../../TeamMeetings/13-10-2014.md). This then enables Arash to [sign-off](JIRAArashCloseLog.png) on stories.
* Encouraged [best use of JIRA](JIRABestPractices.png) throughout the semester.

#### Wiki & Bitbucket Manager

As Wiki & Bitbucket Manager, the majority of work completed was during the projects first few weeks. This involved:

* Initiating, organising, planning and maintaining the project Wiki - [Big commit to organise the wiki](https://bitbucket.org/mtro1538/vc-heart/wiki/commits/36d71495c5fb30256bda0cd1020907a227412f93) (this was used as an exemplar team wiki during a lecture).
* Encouraged team members to branch from the `default` branch to implement a story/feature then submit a pull request to merge the changes into `default`.
* Researched and linked on the Wiki [homepage](../../Home.md) to a good [Markdown syntax resource](https://bitbucket.org/tutorials/markdowndemo), for use when contributing to the Wiki.

Ongoing work throughout the semester included:

* Ensuring Wiki & Bitbucket contributions are kept to a high standard [LINKS!?].
* Respond to queries regarding [Bitbucket use](BitBucketSupport.png) or Wiki contribution.

#### Shadow Mercurial Expert

In my role as shadow Mercurial Expert I completed the follow work:

* Resolved an issue with a corrupt changelog within our Wiki repository - issue #11, [Atlassian support request email](WikiBitbucketSupportEmail.pdf).
* Supported fellow team members in person throughout the semester if they had any mercurial queries.

#### Miscellaneous

Further to the previously mentioned roles, there were also a number of tasks not specifically related to an assigned role but helped facilitate the group processes of the team. These include:

* Researched, initiated, setup ([Mikes reply to his HipChat invite](HipChatSetup.pdf)) and maintained HipChat; an instant messenger used by our team for ad-hoc communication and updates. It was used extensively by the team, this can be seen by looking at the [exported HipChat JSON logs](../Common/HipChatLogs.json). HipChat is also an Atlassian tool and it therefore integrated well with our Bitbucket repository; ensuring all team members were up to date on any commit activities. The HipChat logs show 833 messages between team members, not including commit messages and 'Quotes of the Day'.
* Contributed to all academic obligations throughout the semester.
* Rohan and I produced & delivered the [Sprint 1 Presentation](../../Course/Sprint1Presentation.pptx).
* Reviewed a collaboration tool, [FogBugz](FogBugz.md).

### Coding Work

Please find all the commits I made throughout the semester [here](https://bitbucket.org/mtro1538/vc-heart/commits/all?search=user(Craig)). Almost all of the commits were as a part of a pair-programming group; specifically with Rohan, with the occasional pair-programming session with Mike or Ricky. [Crucible](http://codiographers.cloudapp.net:8060/changelog/vc-heart) offered some statistics for team member commits shown here:

![Commits](https://bitbucket.org/mtro1538/vc-heart/wiki/TasksCompleted/Craig/CrucibleCommits.png "Crucible commits for Craig Sketchley")

The graph demonstrates a distributed amount of commits over the course of the semester. These commits include pair-programming sessions with other users and therefore do not include commits made by any team member I pair-programmed with. Rohan and myself were [allocated the OpenCL implementation epic](../../TeamMeetings/18-8-2014.md) during the week 4 team meeting and all of the coding work was contributing towards that.

#### Learning

Neither Rohan nor I had any experience with CUDA, OpenCL or CHASTE; so a lot of the work involved during the initial weeks was learning these frameworks and libraries. We completed online tutorials, watch recorded lectures and read books (please see my [weekly log](../../TeamDetails/Wikis/Craig.md) for more details). Since other team members were going to be using CUDA I contributed some [notes](CUDANotes.md) to our wiki whilst completing an introductory tutorial.

Learning was on-going throughout the semester ([weekly logs](../../TeamDetails/Wikis/Craig.md) evidence this), especially with CHASTE which consisted of 100000+ lines of code. Our client who was technical and familiar with all the technologies required in this project was kind enough to offer pair-programming sessions at the client site, where he could be on hand to offer advice and support. List of all client site pair-programming sessions are listed [here](../../PairProgramming/Client.md), I have also included some emails organising these sessions ([week 5](Week5PPclient.pdf), [week 9](Week9PPclient.pdf), [week 10](Week10PPclient.pdf)). The work logs for each [story on JIRA](http://codiographers.cloudapp.net:8080/browse/VCHEART-7) also indicate ongoing learning each week. 

#### OpenCL

Initially we identified a single User Story for our epic of converting the given CUDA model to use OpenCL. After initially spending time educating ourselves on the required technologies (see week 4 in my [weekly logs](../../TeamDetails/Wikis/Craig.md)), we tried to dive straight in making changes to the CUDA implementation to enable OpenCL. We considered the conversion to OpenCL would be straightforward but the differences between CUDA and OpenCL, combined with the complexity of CHASTE made getting started very difficult. We attended the client site for a pair programming session supported by our technical client. From this we were able to break our single User Story into several smaller stories/tasks that would enable us to progress incrementally. Spread across the 4 sprints for our project were 5 stories/tasks identified for the [OpenCL epic](http://codiographers.cloudapp.net:8080/browse/VCHEART-7). The following table lists the stories within the OpenCL Epic and their status by the end of the project. For each story please refer to the linked work logs on JIRA.

| Code  | Story Title                           | Status    | Comments |
| ----- | ------------------------------------- | --------- | -------- |
| [VCHEART-10](http://codiographers.cloudapp.net:8080/browse/VCHEART-10) | Simple testable OpenCL example        | Delivered |          |
| [VCHEART-26](http://codiographers.cloudapp.net:8080/browse/VCHEART-26) | Implement OpenCL model                | Delivered |          |
| [VCHEART-39](http://codiographers.cloudapp.net:8080/browse/VCHEART-39) | Remove CUDA dependency from model        | Delivered |          |
| [VCHEART-45](http://codiographers.cloudapp.net:8080/browse/VCHEART-45) | Generate OpenCL GPU manager functions    | Delivered |          |
| [VCHEART-46](http://codiographers.cloudapp.net:8080/browse/VCHEART-46) | Run OpenCL on VC server               | Not implemented | Insufficient time |

Work was completed in the branch ‘OpenCL’, all related commits can be found [here](https://bitbucket.org/mtro1538/vc-heart/commits/branch/OpenCL).

The final product of this Epic we worked on can be found [here](https://bitbucket.org/mtro1538/vc-heart/src/4321eaca74dc8f8667da443f8305c736fcd24960/models/__opencl__/?at=default)

#### [Sprint 1](http://codiographers.cloudapp.net:8080/secure/RapidBoard.jspa?rapidView=1&view=reporting&chart=sprintRetrospective&sprint=1)

##### [Simple Testable OpenCL Example](http://codiographers.cloudapp.net:8080/browse/VCHEART-10)

Although not technically a User Story, our first story/task was to implement a simple, testable OpenCL program; this would act as a starting point on which to integrate into the current CUDA model and offer us a good introduction into writing OpenCL code. This story/task was of value to the client, as it would demonstrate that running OpenCL code on a Virtual Machines was possible. Pair-programming logs for this story can be found within the subtask of the story, [VCHEART-32](http://codiographers.cloudapp.net:8080/browse/VCHEART-32). An example commit from this story can be found [here](https://bitbucket.org/mtro1538/vc-heart/commits/5c03dad108176bdd1730005297c79b5cdedc690d?at=OpenCL). It should be noted that since this task had no direct tangible value to the client, the simple example does not exist in the final client deliverables.

#### [Sprint 2](http://codiographers.cloudapp.net:8080/secure/RapidBoard.jspa?rapidView=1&view=reporting&chart=sprintRetrospective&sprint=2)

##### [Remove CUDA Dependency from Model](http://codiographers.cloudapp.net:8080/browse/VCHEART-39)

In order to begin implementing OpenCL equivalent functionality, all CUDA dependency within the current model needed decoupling. This required a greater understanding of the CUDA cardiac model and the interaction between classes. Further Pair-Programming sessions at the client site were required to fully decouple the dependencies. Here is an [example commit](https://bitbucket.org/mtro1538/vc-heart/commits/0bb2d8f8a2cf413f282c488109b5ffa8a1f13f57) for this story.

#### [Sprint 3](http://codiographers.cloudapp.net:8080/secure/RapidBoard.jspa?rapidView=1&view=reporting&chart=sprintRetrospective&sprint=3)

##### [Generate OpenCL GPU Manager Functions](http://codiographers.cloudapp.net:8080/browse/VCHEART-45)

Initially, the original CUDA model utilised a set of GPU manager functions that wrapped all the CUDA API calls. In an attempt to minimise the differences between the original CUDA version and the completed OpenCL version, a similar pattern of having GPU manager functions wrap the OpenCL API calls was designed. An example commit can be found [here](https://bitbucket.org/mtro1538/vc-heart/commits/e2916e97f1ab35aada939dedcad9c9fc68221cac).

#### [Sprint 4](http://codiographers.cloudapp.net:8080/secure/RapidBoard.jspa?rapidView=1&view=reporting&chart=sprintRetrospective&sprint=4)

##### [Implement OpenCL Model](http://codiographers.cloudapp.net:8080/browse/VCHEART-26)

Once the GPU was accessible through the OpenCL GPU manager functions, all that was left to do was convert the kernels into OpenCL kernels and enable all the OpenCL GPU calls within `CardiacMultiCellManager.hpp`. This required quite a significant amount of work and I easily logged over 40 hours during this story. An example commit can be found [here](https://bitbucket.org/mtro1538/vc-heart/commits/7eeedcd29e8e1f9e073bf130ab9cfe34efdb65a9), [here](https://bitbucket.org/mtro1538/vc-heart/commits/4ce06f85204916a88e056acf145843e8bfde2316) and [here](https://bitbucket.org/mtro1538/vc-heart/commits/880197a459f2fd0580ca2b87477060de69e74078).

##### [OpenCL Model Runs on VC Server](http://codiographers.cloudapp.net:8080/browse/VCHEART-46)

In order to fully take advantage of OpenCL it should be tested on other systems, in particular, the large server at the Victor Chang. This story was not quite finished and required a small bit of tweaking which will be resolved after the completion of this project. The integration work can be found [here](https://bitbucket.org/mtro1538/vc-heart/commits/457d9b1ba37438781d55296caed61229f9b75a49) and the issues we had with this are listed [here](https://bitbucket.org/mtro1538/vc-heart/issue/73/opencl-mystery-seg-fault) and [here](https://bitbucket.org/mtro1538/vc-heart/issue/72/mesh-compilation-errors).


## Quality of Work

In addition to my work in the XP roles explained above, we tried to follow the most appropriate of the [12 best practices of XP](http://www.jera.com/techinfo/xpfaq.html). I have included evidence of these best practices in their contribution to the quality of work in the table below:

XP Best Practice | Description & Evidence
------------- | ---------------------
__Simple Design__ | Our approach has always been to develop in small increments, only making small but essential modifications in the codebase. Our approach was to modify the existing codebase a little as possible so when the OpenCL implementation is complete it could be converted into a template as easily as possible. Notice only small differences between the original model [`BatchCompute` method](https://bitbucket.org/mtro1538/vc-heart/commits/e96f0836a6d7dcb14b0f953e329ade0b0b83a8c5#Lopencl/cuda/GPUOhara_Rudy_2011_vccri.hppT79), and my final [`BatchCompute` method](https://bitbucket.org/mtro1538/vc-heart/src/4321eaca74dc8f8667da443f8305c736fcd24960/models/__opencl__/templates/OpenCLOhara_Rudy_2011_vccri.hpp?at=default#cl-80).
__Continuous Testing__ | The stories we were working on did not lend itself directly to writing many tests. Whilst we did not explicitly write a large amount of tests we did constantly check our implementation and how it integrated with CHASTE. See week 7 & 10 of my [weekly log](../../TeamDetails/Wikis/Craig.md) for the issues with testing. Some TDD can be found within this [commit](https://bitbucket.org/mtro1538/vc-heart/commits/31761af4ed0566211090f3c41ebbdc00760f09e0).
__Refactoring__ | Our assigned required constant refactoring. Our client always encouraged us to make small incremental changes to maintain something that worked, even if they were a bit hacky; once we had implemented the desired functionality we would refactor to improve the code standard. An example of a refactor can be found [here](https://bitbucket.org/mtro1538/vc-heart/commits/31761af4ed0566211090f3c41ebbdc00760f09e0) where I had to abstract out a single OpenCL simple example in smaller functions to make it more testable.
__Pair-programming__ | Throughout the entire semester we've always tried to use pair-programming. Check the [weekly logs](../../TeamDetails/Wikis/Craig.md) and [story work logs for our epic](http://codiographers.cloudapp.net:8080/browse/VCHEART-7). We've been [pair-programming at the client site](../../PairProgramming/Client.md).
__On-site Customer__ | Our client was very generous with his time throughout the semester and as a technical client, was very involved and supportive. We had a number of pair-programming sessions with him. [Pair-programming at the client site](../../PairProgramming/Client.md)
__Coding Standards__ | Our reliance on Pair-programming throughout the project contributed to high quality coding standards. We used [Crucible](http://codiographers.cloudapp.net:8060/changelog/vc-heart), a code review platform. See the [weekly logs](../../TeamDetails/Wikis/Craig.md) and [story work logs for our epic](http://codiographers.cloudapp.net:8080/browse/VCHEART-7) for records of pair-programming.

## Reflection

Overall I feel very pleased with what we as a team have been able to accomplish this semester. At the beginning of the semester, each team member listed their high level goals for the semester on their individual wiki page. These were then collated and combined into one team oriented high-level goal (found on [wiki homepage](../../Home.md)):

> "To create value for the client, learn something new, achieve an HD ... and save lives"

Our client has expressed his satisfaction at our accomplishments both in the [client deployment presentation](../Common/vccri-presentation.pptx), the final [client meeting](../../ClientMeetings/20-10-2014.md) and through issue #70. This was further confirmed as our [client suggested](../../ClientMeetings/20-10-2014.md) that we could publish our accomplishments in a biomedical journal or conference paper.

The OpenCL story has exceeded the clients expectations as he was not expecting us to finish as evidenced by the [client meeting minutes in week 11](../../TeamMeetings/13-10-2014.md) and verified by an [email correspondence](OpenCLClientSatisfaction.pdf).

I believe I was an effective JIRA expert; from setting up our own Jira instance and customising it for our uses, to maintaining the instance and providing support (as evidenced above). The [activity stream](http://codiographers.cloudapp.net:8080/secure/Dashboard.jspa#Activity-Stream/10003) on our Jira instance shows high usage amongst all team members, illustrating effective 'Mutual Performance Monitoring'. One area of weakness was our story completion procedure; all stories tended to be moved into 'In Review' only after a sprint had passed the finish date, the client would then move the stories to 'Done'. Moving the stories was usually done either during or after a weekly meeting. This led to a rather alarming [burndown chart](http://codiographers.cloudapp.net:8080/secure/RapidBoard.jspa?rapidView=1&view=reporting&chart=sprintRetrospective&sprint=3) in certain cases. I should have encouraged team members to 'own' their stories and progressed stories themselves whenever the story was complete, not just at the end of a sprint. In some cases, the end of the sprint did line up completion of the story and therefore this cannot be helped. From the start we found it very difficult to generate stories for this project and break them down into manageable pieces; it tended to have rather large pieces of functionality which required a full sprint to complete.

As Wiki & Bitbucket manager I believe I was able to orient the team by constructing an exemplar Wiki within the [first few weeks](https://bitbucket.org/mtro1538/vc-heart/wiki/commits/36d71495c5fb30256bda0cd1020907a227412f93). This enabled the team to log work effectively, contribute resources easily and provided a portal for 'Team Leadership' through meeting schedules, agendas and minutes.

As the shadow Mercurial expert, I was able to adopt the 'Backup Behaviour' and solve a problem we had early on with our Mercurial Wiki repository (see issue #11 and the [Atlassian support request email](WikiBitbucketSupportEmail.pdf)). As the project progressed, the team grew more comfortable with Mercurial and therefore required my expertise less.

When I compare what I planned to achieve each week with what I was actually able to accomplish, I can see that my planning was mostly accurate. This was especially true as the semester, and therefore the project, progressed. In the initial few weeks, I was extremely over ambitious as I had limited technical knowledge to truly understand the scope of the OpenCL Epic and the CHASTE codebase. This can be seen in an [email thread](Week5PPclient.pdf) between myself and the client as I was beginning the first story (see the first 2 emails in the thread). It makes sense that as I developed a greater understanding of the technical requirements, that my task estimation would improve (week 11 in the [weekly log](../../TeamDetails/Wikis/Craig.md) is an excellent example of this).

One area where my planning and programming fell short was testing. I had planned to increase my testing each week but found it difficult because of the nature of the codebase (see weeks 7 & 10 of my [weekly log](../../TeamDetails/Wikis/Craig.md)). Even though there were hundreds of tests already integrated within CHASTE, we could have found more ways to test our external code.


