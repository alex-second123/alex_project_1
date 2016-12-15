# alex_project_1

This is an example of a simple web API implemented using
[Flask](http://flask.pocoo.org/) and
[Flask-RESTful](http://flask-restful.readthedocs.org/en/latest/).


1. This application is to act as a simplified version of UNC's media resources center video and audio equipment checkout service. 
	 in the equipment tab, there are three active links to individual pieces of equipment (Canon M400, Greenscreen, Zoom H1 Digital) each      with a form to check them out from the media resources center 

2. it's functionality (or lack of) includes allowing a student (via an active UNC PID) to check out various articles of equipment from the media resources center,
	allowing a student to delete their previous request 
	allowing a student to update their previous request 

3. desired functionality would include:
   -updating, posting, and deleting reservations from the javascript calendar that right now is not doing anyhting 
   -having the "Log In" functionality to allow a UNC employee to update, delete, or add equipment to the available equipment resource via     their unique  credentials
   -handling for when a piece of equipment has multiple reservations, give priority to that which was placed first 

4. additional documentation 

"PID": 9 digit unique student identifier used in the form data and JSON
"date_start": date the student wishes their reservation to start
"date_end": date the student wishes their reservation to end
"Equipment": unique piece of equipment the student wishes to check out 

5. resources 
Canon M400 = resource for the Canon M400 camera with forms to edit and create a request
Zoom H1 Digital Recorder = resource for the Zoom H1 Digital Recorder with forms to edit and create a request
Greenscreen = resource for greenscreen equipment with forms to edit and create a request
Home_request = form for update (not used in the app flow)
all_equip = resource for all of the available equipment at checkout with forms to add or delete equipment 
Calendar = JS calendar that ideally would post the start and end date of a student's reservation for other students to see and 
			schedule accordingly


6. new classes

(attempted to keep the namespace of the original code the same which ended up being very logically challenging)

EquipmentList #class to allow the auth user to edit and add equipment to the resource
Cal #class that would take in requests and post their start and end dates on the imported JS calendar 


7. end 

Intellectual property to UNC media resource center 
images linked to thier original sources, credit to proprietors of those images 
original code credited to Dr. Ryan Shaw via https://github.com/sils-webinfo/helpdesk/
other cited code via JavaScriptKit.com (although not functionally used) 
occasional basic CSS styling guides via http://www.w3schools.com/
