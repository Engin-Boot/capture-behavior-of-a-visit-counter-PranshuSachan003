# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given (Sensor for entry-card issuer works properly)
  When  (person enters)
  Then  (Sensor identifies the patient AND increments the visit-counter by one)

Scenario: Compute parking slots to reserve for visiting specialists

  Given  (Sensor for hospital staff attendance system works properly)
  When   (Before specialists visits the hospital)
  Then   (Reserve the parking slot for specialists)
