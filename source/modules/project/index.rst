Project
=========

Each scenario always follows the same basic format:

Scenario: Some description of the scenario

  Given some context

  When some event

  Then outcome

Each part of the scenario - the context, the event, and the outcome - can be extended by adding the And or But keyword:

Scenario: Some description of the scenario

  Given some context

  And more context

  When some event

  And second event occurs

  Then outcome

  And another outcome

  But another outcome

