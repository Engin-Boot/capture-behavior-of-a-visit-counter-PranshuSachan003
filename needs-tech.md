# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given (Sensor for entry-card issuer is not working properly)
  When  (patient enters)
  Then  (Use SQL Server Management Studio to recover the visit-counter)

Scenario: Reconcile counts if the sensor is offline for a while

  Given (Sensor for entry-card issuer is not working properly)
  When  (patient enters)
  Then  (go to previous saved count on database AND increment by one)
