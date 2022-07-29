# CS498_NarrativeViz

By Balakumar Balasubramaniam, CS 498

Click here to see the visualization. 

### Message
There are three key messages in this visualization: 

1. Central banks around the world are a lot more active in raising and lowering rates than most people perceive

2. Most central banks follow the US lead, especially in times of crises

3. But EM banks tend to raise rates faster during the recovery phase

I used publicly available rates data to create this visualization. The data was pre-processed in python before using in this project. 

### Narrative structure
I used a Martini glass narrative structure. The first visualization (default) shows 5 of the DM and 5 of the EM rates changes over a couple of decades. This is the author driven step. 

The reader can then click on the tabs to illustrate the other points about DM vs EM central bank behaviors. 

Take together, this narrative forms a martini glass structure. 

### Visual structure
Highlights and transitions are used as appropriate to improve the messaging and visual structure. For example, the text annotations transition over a few seconds to draw the user's attention. The lines are turned on and off to remove visual clutter. Large plots with adequate axis range provide clarity. Further, the axes ranges are not changed between the tabs. While this may seem counter-intuitive, user testing showed that this is a better approach than dynamicall changing axes. 

### Scenes
There are three scenes in this visualization. The first scene shows all central-bank rates data, and illustrates that central banks are very active, historically. The second scene shows that DM banks often follow the US Fed's lead. The third scene shows that EM banks raise rates faster during recovery. In all scenes, the appropriate lines are turned on or off depending on the context.

### Annotations
Annotations are triggered when the user steps through the tabs at the top. The text messages (and their colors) change as the user moves through the visualization. 

### Parameters
The parameters in the visualization are the three tabs at the top. 

Other parameters are declared in the code as variables in the code and include width, height, margin sizes, and line colors. 

### Triggers
The triggers are activited when the stepper buttons at the top are pressed. When switching to the "Developed markets" or "Emerging markets" tabs, some of the existing lines are turned "off" to clean up the messaging. When the use clicks on the first tab again, all the lines are turned "on".

#### Acknowledgments
I used the stepper.js class from NYTimes (with significant modifications) and used the d3 examples page for plotting lines. 
