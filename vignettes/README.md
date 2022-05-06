# Knowing where to tap

## Many parts to the problem

Identifying the cause of a problem

Efficiently solving a problem

Avoiding a problem

## Root cause analysis

Faults in any technical system happen. This is a fact of life. Even well
engineered hardware systems are prone to wear and tear and therefore can fail.
Tracking these faults either reactively (when things break) or proactively (before 
things fail) can be approached using a root cause analysis.

Root cause analysis tries to pinpoint where a system breaks by using four
simple rules:

1. identify the problem
2. establish a timeline until the problem (if applicable)
3. correlate circumstances with the problem (event correlation)
4. draw up or sketch when the fault occurs (visualize the process)

Key in root cause analysis is that when you remove the root cause the problem
will not exist anymore. It is important to note that this is different from
removing the causal factors which triggers the root cause. However in some
cases they are related (see boundary conditions below).

### Finding a root - theory

A root cause can easily be found by taking into consideration the rules above
and the five "why" approach. Continue to ask why something does not work until
you reach a root cause (depending on the system this might take more than
five steps).


#### Identifying a problem

Often when things break it produces a set of symptoms, in short things that 
shouldn't happen. However, these symptoms aren't necessarily the root cause
and can be linked in various ways to the root cause however observing that 
things break is the first step towards a solution.

### Defining the problem

Although the next steps (below) will bring you closer to the root cause it is 
always wise to define the true nature of the problem. Throwing your hands up and
stating that it "just doesn't work" is not a helpful step towards a solution.
One has to accurately define what does not work. This will need you to gather
data on the processes involved and the timeline it developed on, but also put
into words what (process) isn't working.

#### Timelines

Timelines are critical in finding many root causes of software and hardware
problems. Timelines give you a before (working) state and and after (failing)
state of a system. Logic dictates that something in the mean time has changed
which alters the outcome of your process.

Defining when something happens is therefore key in finding many software and
hardware issues. Within the context of software development it can not be 
stressed enough how important version control is within this context. Version
control allows you to track the temporal progression of code and revert to a
previous working state. Maintenance logs on physical hardware serve more or less
the same function.

#### Boundary conditions

Not all faults should be resolved. Some faults can be circumvented in a lawful
way, by failing gracefully. However, be sure to investigate the conditions of
failure well. When writing code you create a system which might
have inherent assumptions which are known to you but not necessarily someone else.
This inbalance in information can create situations where a piece of software (or
hardware for that matter) is used outside its original scope. This can cause
faults which are not critical, yet failing gracefully (with clear warnings
or messages of out of scope use) should prevent any confusion on this part.

Black swan events (improbable high impact but not impossible situations) or 
silent risk might also trip you up. This is not necessarily out of scope use
but rather a combination of a set of parameters which results in failure due
to their combined effect. Since the likelihood that all these parameters
converge is low such (logical) errors might sneak into systems but can cause
faults if used long enough in various circumstances. The latter is particularly

### Example 1. The holiday blues

For example, your code breaks after you return from holiday. You've identified
the problem (1), and you have a timeline (2) since you know that things worked
before you left for your holiday. This sets you up to investigate what changed 
between you leaving and returning from your holiday. 

You can now narrow down the source of your problem to this time window and all
actions you (automatically) took between you left and returned. Say, you returned
from your holiday and updated your computer. This would suggest that the state
of your computer has changed and seems to be critical to your piece of software
running correctly.

### Example 2. The unexpected

Out of bound example


### Example 2. Carnival

Type issues

# Cheat sheet

### Finding a root - practices

- breakpoints
- print outputs
- 

### Avoiding problems

- setup unit tests
- tests mechanistic models using a wide range of parameters
- 



