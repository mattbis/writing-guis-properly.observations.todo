# writing-guis-properly.observations

## local to a topic space and scenario - please ignore - not meant as a generalised guide....

.. it seems since nobody understands this I will have to note some things down

### pre notes

1) UI Thread & Main Process

2) Windowing and GUI Limitations

3) Understanding GDI and PostMessage

4) Understanding OpenGL is not going to solve your problems

5) Cross-platform When and When Not ( OSX First compilation is fraught with problems on other platforms )

6) the importance of `no-gui` or `minimal-gui` see: mitigations.

7) its not actually that complicated you dont need a framework for everything.. there are many examples, THEY ALL SUFFER THE SAME PROBLEM

#### constraints - os internals - security and saturation

define Saturation - when there are so many gui updates and messages - the operating system will prioritise messages. ( effectively your instances stop working when trying to click a change ( a bundle of messages ) and when receiving updates )

define Migitation - see my previous gists, there is no remediation since it increases the stack size and causes delays per update refresh  everything down. ( its only possible beyond 64gig and i9 - sofaik )

Factors that effect **scale**, **complexity** 

1) dynamic link libraries
2) so
3) osx

### CONCEPTS

1) - Point1 is simple **MOST PEOPLE ARE POOR** they do not have the latest and greatest - in fact they are likely 2-8 years behind hardware wise...
   - Point2 is always offer a non-gui option from a `manifest`

#### RUNTIME MODES

1) What are modes? How many should we have ? See ( user research )
2) Before releasing your product and assets ( make sure you really understand your market, your consumers, the tech stack and you hire REALLY GOOD TESTERS )

