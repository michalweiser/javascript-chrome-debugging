Debug JavaScript in Chrome
===========================

This document contains usefull informations about debugging in Chrome Developer Tools. Listed commands are not copying original documenatation references, to find all commands and informations follow links in Resources section. Informations are grouped to logical sections, each of them represents specific part of developers workflow.

Keyboard shortcuts
------------------
| Command     | Mac | PC |
|-------------|:---:|:--:| 
| Open Devtools | alt + cmd + i | ctrl + shift + i |
| Open DevTools and focus console | alt + cmd + j | ctrl + shift + j |
| Quick access | cmd + p | ctrl + p |

Console tools
-------------

In case you decide to use any console command always remember to remove them before your code goes to production! Best practice to use console object is to use it through global window object since in many app environments window is considered as globally defined object -> window.console.log('my log'); Always remember that window.console is not defined in all browsers. In case browser doesn't support console, code will crash immediately. Best practice to solve this situation is to overload console object (example: https://github.com/sunnykgupta/jsLogger): 

* log, info, debug - all aliases lead to simple logging function witch uses printf conventions
* trace - allows print function call stackon current code position and state
* count - enables to count specific labels (good for multiple iterations through complex structures)
* table - shows nicely alligned output of objects with the same struture
* dir vs. dirxml - shows JS object or XML representation of showed object
* warn, error - specific calls of log() function -> indicated by specific warning or error symbol at the front of the log message (triggers special devtools counters for warnings and errors)
* assert - may be used as simple test tool

Command line tools
------------------
* $_
* $1 - $4
* keys, values
* selectors
* inspect
* getEventListeners
* monitor
* monitorEvents
* debug
* copy


Debugging tricks
----------------

* quick access
* debugger;
* preserve log
* F8 for :hover
* break on
* change element status
* keyboard shortuts

Performance optimization
------------------------
* profile
* time
* timeline
* timeStamp

Extensions to look at
---------------------

* http://domflags.com/
    
    
Resources:
----------

* http://vimeo.com/53073654
* https://developer.chrome.com/devtools/index
* https://www.youtube.com/watch?v=f7AU2Ozu8eo
* https://www.youtube.com/watch?v=nOEw9iiopwI
* http://discover-devtools.codeschool.com/
