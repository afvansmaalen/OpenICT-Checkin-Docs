API
===================================
.. _api:

There are 2 API versions available, until further notice only v1 is being used. It will automatically remap every API call to the default API version in case the version has been omitted. 

.. _v1:
V1
--------

/api/v1/getVersion: 
	Returns a JSON with the used version.

/api/v1/getUserAll
	Returns a JSON with all users.
	
/api/v1/getUserAdmins:
	Returns a JSON with all users who have their role set as 1.

/api/v1/getUserStudents:
	Returns a JSON with all users who have their role set as 0.
	
/api/v1/getUser/{id}:
	Returns a JSON with the user associated with id.
	
/api/v1/setUser:
	Functiionality not written.

/api/v1/getUserForms/{user_id}:
	Returns a JSON with all answers of user user_id.
	
/api/v1/geUserFormLatest/{user_id}:
	Returns a JSON with the answers of the latest form filled in.

/api/v1/geUserDailyLatest/{user_id}:
	Returns a JSON with the answers of user user_id of the daily check-in form (form_id 1).
	
/api/v1/getFormAll:
	Returns a JSON with all forms

/api/v1/getForm/{id}:
	Returns a JSON with the form form_id and its associated questions.
	
/api/v1/getDaily:
	Returns a JSON with the daily check-in form (form_id 1).
	
/api/v1/setForm:
	Functiionality not written.

/api/v1/getAnswerAll:
	Returns a JSON with all answres written.
	
/api/v1/getFormAnswers/{id}:
	Returns a JSON with the answers in the row id.
	
/api/v1/saveFormAnswers:
	Saves the answers in the database.
	Expects:
		user_id -> The id of the user who answered the form.
		form_id -> The id of the form that is filled in.
		array_answers -> An array of the answers in string format. 
			Example:
				{
					"5",
					
					"My day went well",
					
					"colleagues were nice"
				}

/api/v1/getQuestionAll:
	Returns a JSON with all questions.

/api/v1/getQuestion/{id}:
	Returns a JSON with Question id.
	
/api/v1/editQuestion/{id}:
	Functiionality not written.

/api/v1/putDaily:
	Creates a basic answer sheet
.. _v2:
V2
--------
/api/v2/getVersion: 
	Returns a JSON with the used version.
	
