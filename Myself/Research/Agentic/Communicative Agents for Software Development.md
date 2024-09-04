#Agents #LLM
#### Abstract/Intro:
Using LLMs across Software Development Process

Core is ChatDev a virtual Chat for software Development
Water-Fall Method in this Development experiment 
Four Distinct Stages: Designing, Coding, Testing, and Documentation

Each team has Software "Agents" 

7 minutes make something for less than a dollar 
Github:https://github.com/OpenBMB/ChatDev

LLMs have a huge potential in automating Software due to code and documentation being text something LLMs excel at structuring

Hallucination is a big risk the larger the project:
Lack of granular tasks the more vague the less effective
No Cross Examination

Fix:
Proposed chat chain that divides each phase into atomic subtasks. Each node represents subtask, and have two roles multi-turn discussions
#### Result
The experiment analyzed Software produced in response to 70 user requirements
Results:
`The experiment analyzed all the software produced by ChatDev in response to 70 user requirements. On average, ChatDev generated 17.04 files per software, alleviated potential code vulnerabilities caused by code hallucinations 13.23 times, had a software production time of 409.84 seconds, and incurred a manufacturing cost of $0.2967. Discussions between a reviewer and a programmer led to the identification and modification of nearly twenty types of code vulnerabilities, while discussions between a tester and a programmer resulted in the identification and resolution of more than ten types of potential bugs. In summary, our main contributions are as follows:

#### ChatDev:
##### 2.1 Chat Chain:
ChatDev uses Waterfall
Four Phases:
Design: Innovate Ideas through brainstorming and technical design requirements are made
Coding: Development and review of source code
Testing: Integrate all components and utilize feedback from interpreter for debugging
Document: Generate environment specifications and user manuals

All of these actions are then excuted using chat chain with each agent having a role 
Architecture:![[Architecture.png]]
Three Keys to ChatDev:![[Three Keys.png]]
Role Assignment:
Prompt Engineer roles for each agent only form of prompting is to initiate role-playing scenarios

Two Prompts with Two LLMs One Mission:

Each interaction has two roles Instructor and Assistant
CEO plans while CPO execute tasks and providing responses
Use Inception Prompting to achieve role specialization

These Prompts mission:
instructor and assistant prompts encompass vital details concerning the designated task and roles, communication protocols, termination criteria, and constraints aimed at preventing undesirable behaviors

Memory Stream: 
Memory Stream allows for Agent's previous dialogues to be recorded and saved
Mt is record at time t  I1 is instructor instruction while A1 is Assistant response

Conversational messages up to time t:
![[Screenshot 2024-05-02 at 5.30.07 PM.png]]

v = LLM-based decision extractor which can be implemented via communication protocol detection or self-reflection

![[Screenshot 2024-05-02 at 5.37.54 PM.png]]

Update Process: Fed back into Message history and Instruction history
![[Screenshot 2024-05-02 at 5.35.07 PM.png]]
Communication Protocol developed: 
At the end of chat for example requirements when consensus is reached a speicifc format is is spit out <Modality>:DesktopAPP
System self checks to see if in compliance with protocol

Self Reflection:
Sometimes reach consensus however do not trigger predefined communication protocols as termination conditions. In this case we must use self-reflection. A psuedo-self is initated and a new chat is made these psuedo informs assitant of historical records and requests a summary. Encourages reflection to stop halluciation

