## book appointment + new patient
* greet
 - utter_name
 - utter_patient_type
* enter_data{"patienttype": "yes"}
 - action_store_patient_type
 - utter_ask_name
* enter_data{"name": "Max Meier"}
 - action_store_name
 - slot{"person_name": "Max Meier"}
 - utter_ask_email
* enter_data{"email": "maxmeier@firma.de"}
 - action_store_email
 - slot{"email": "maxmeier@firma.de"}
 - utter_date_time
* enter_data{"date": "monday at 2 pm"}
 - action_store_date
 - slot{"date": "2018-08-22T19:30:00+00:00"}
 - action_book_appointment