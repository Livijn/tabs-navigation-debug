# tabs-navigation-debug 
Build project (npm i && ionic serve) and open browser

### Bug 1: Wrong endpoint after swipe to go back
* Make sure you refresh from Tab 1
* Click Tab 2
* Click Tab 1
* Click To Child
* Click Tab 2
* Click Tab 1
* Swipe to go back
* You are now on tab 2

### Bug 2: Cannot swipe back
* Make sure you refresh from Tab 1
* Click To Child
* Click Tab 2
* Click Tab 1
* You cannot swipe back
