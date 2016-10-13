# README #

### Author: Harpreet Dhillon , harpreet@uoregon.edu ###

---

### Purpose ###
* This application is for Project 3 of CIS 322 at University of Oregon.
* The purpose of this project was to modify an existing system that submitted a POST request through a form. The modifications were to use AJAX interactions on each keystroke instead.

### Application Specifics ###
* The application runs on the flask_vocab.py script and displays either:
  * The index page template
  * or the respective error template: 400, 403, 500
* As keystrokes are read, a JSON object will be sent to the server via a POST request. The returned data will then either be displayed or make some modification to the anagram page.

### Running the Application ###
* Test deployment to other environments including Raspberry Pi.  Deployment 
  should work "out of the box" with this command sequence:
  * `git clone <yourGitRepository> <targetDirectory>`
  * `cd <targetDirectory>`
  * `make configure`
  * `make run`
  * (control-C to stop program)
* The default port is 5000, so the webserver should be reachable at http://localhost:5000 , and also through its IP address.
 
### Testing the Application ###
* Nose tests for vocab.py, letterbag.py, and jumble.py can be run with:
  * `nosetests`
