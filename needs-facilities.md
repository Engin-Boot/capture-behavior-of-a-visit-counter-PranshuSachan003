# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given ( Sensor for foot-fall counter at the door works properly)
  When  (person visits the hospital)
  Then  (increment visit-counter by one and update database each day)

Scenario: Alert when seating capacity is full

  Given (Sensor for entry-card issuer works properly)
  When  (person enters)
  Then  (Sensor identifies the patient and alert if seating capacity is full)
