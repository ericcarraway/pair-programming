Thursday, Nov 19, 2015

# Lunch and Learn: Pair Programming
```
* Where we've been
    * BDD / TDD - writing tests first based on JIRA / User Stories
    * Modularity and code organization
    * Intro to Vim
    * Martin Fowler / Neil Ford "Explaining Agile" video
* Today
    * Our Pair Programming experiences from the last four days
* Where we're going
    * Lunch and Learn suggested topic board (Etherpad)
    * Doesn't have to be a single presenter using slides
    * Other potential formats?
        * Moderated discussion
```

## Why do we pair program?
* Avoid knowledge silos
* Large (or overlapping) tasks / user stories
* It's more than just typo spotting!
  
#### Obvious reasons for pair programming  
#### Less obvious reasons for pair programming  
* Abstract tasks
* Changing requirements
* Shorter deadline (one week mini-sprint vs. our typical two weeks)
* Quantity of work in the backlog
* Prioritization changes

## Getting started / pre-requisites
```
* Just jump in and deal with issues as they come up
    * We didn't find a rhythm until Day 3
* Dev environment
    * Use a comfortable editor and box configuration for both devs
        * Not a good time to experiment with a new editor
        * Not good if only one dev knows Vim
        * QWERTY / DVORAK
        * Avoid interference and productivity barriers
    * Multiple monitors vs. a single monitor
        * Having spaces for editor/browser/terminal/Slack
    * Standing vs. sitting desk
    * Whiteboard available
    * Notebook/paper and pen available
```
### How to Git with multiple partners for fun and profit  
Understanding `git` workflow - how to collaborate on a branch / PR  
Thanks to @tomtom for his help on Slack  
_Summary_  
`TeamMemberA` and `TeamMemberB` collaborate on `TeamMemberA`s box.  
They reach a stopping point and push to `TeamMemberA`'s GitHub `origin`.  
`TeamMemberA` makes a W.I.P. pull request for other team members to review and comment on.  
If `TeamMemberB` then wants to work on `TeamMemberA:story-1234-asdf`,  
he should add `TeamMemberA`'s fork as a remote via:  
```
git remote add TeamMemberA https://github.com/TeamMemberA/our-team-project.git

git fetch --all

git checkout TeamMemberA/story-1234-asdf

...make code changes...

git add && git commit

git push
```
This will update `TeamMemberA/story-1234-asdf`,
which in turn will update the pull request that is open for that branch.
This also means `TeamMemberA` needs to fetch changes into his local `story-1234-asdf` branch after `TeamMemberB` pushes.
### Maintain your typical workflow
The good habits you have for programming alone, make sure you still do these while pairing!
* Plan
* Break things into steps
* Make TODO lists
* Set goals
* Decide stopping points in advance
* Ask questions
For example,
    - What will the URIs look like for AJAX requests?
* Think in terms of a "stack"
```
* UI / View
* Controller
* Service / Resource
* Stub.by - Mock data
    * Requests - YAML
    * Responses - JSON
```
* Think in terms of a narrative
```
* A user does this...
* and then this happens...
* and then this happens...
* and finally...
```
* Use breaks
* Work in pomodoros
* Pace yourselves
```
Contrasting opinions on pacing
    * Momentum
    * The value of "early wins"
    * Blocker-breaking stamina in the bank
```

## The driver role and the navigator role
* If less experienced in an area, you drive (e.g. directives)

## Personality and the human aspect
* Align schedules on a macro and micro level
```
MACRO
    With flexible office hours,
    a 7-4 dev may not work well with
    a 9-6 dev
MICRO
    Take coffee and restroom breaks at the same time
```
* As programmers, we often need a balance of social/collaborative situations and solitary situations
* If you need alone time, make sure you take it
_You may miss your heads-down with headphones in-the-zone feels._

## Bring in an objective 3rd-party
* Knowledge silos => silo pairs
* Use a 3rd-party rubber ducky (+1 @sharkySharks)
* Avoid tunnel vision, which is still possible with two people

## Disadvantages
```
* Ties up two people
    * When a third person is waiting on one of those two people...
```

## Added benefit: learn each other's workflow tidbits of knowledge
Examples:
* Use breakpoints in Chrome DevTools, use less `console.log`
* John Papa Style Guide on Angular _"Best Practices"_*
* Chrome tab navigation (Command + 1)
## Antipatterns
* BTW, Eric hates this word
