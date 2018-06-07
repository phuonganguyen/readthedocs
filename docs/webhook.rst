Webhook Event
=============

Common properties
-----------------

* Desription

	=========  ======  ==================================================================
	Property   Type    Desription
	=========  ======  ==================================================================
	type       String  Identifier for the type of event.
	timestamp  Number  Time of the event in milliseconds.
	source     Object  Source user object with information about the source of the event.
	=========  ======  ==================================================================
	
* Source User

	=========  ======  ==================================================================
	Property   Type    Desription
	=========  ======  ==================================================================
	type       String  user
	user_id    String  Letstalk ID of the source user
	=========  ======  ==================================================================
	
Message Event
-------------

* Desription

	=========  ======  ==================================================================
	Property   Type    Desription
	=========  ======  ==================================================================
	type       String  message
	payload    String  message payload. This will be an encrypted JSON String.
	=========  ======  ==================================================================
	
* Example::

	{
		"type": "message",
		"timestamp": ​1527151205790​,
		​"source": {
			"type": "user",
			"user_id": "jimmy.chen"
		},
		"payload": String
	}
	
Add Contact Event
-----------------

* Desription

	=========  ======  ==================================================================
	Property   Type    Desription
	=========  ======  ==================================================================
	type       String  add_contact
	=========  ======  ==================================================================
	
* Example::

	{
		"type": "add_contact",
		"timestamp": ​1527151205790​,
		​"source": {
			"type": "user",
			"user_id": "jimmy.chen"
		}
	}
	
Add Contact Event
-----------------

* Desription

	=========  ======  ==================================================================
	Property   Type    Desription
	=========  ======  ==================================================================
	type       String  delete_contact
	=========  ======  ==================================================================
	
* Example::

	{
		"type": "unsubscribe",
		"timestamp": ​1527151205790​,
		​"source": {
			"type": "user",
			"user_id": "jimmy.chen"
		}
	}
	
Ask Key Event
-------------

* Desription

	=========  ======  ==================================================================
	Property   Type    Desription
	=========  ======  ==================================================================
	type       String  ask_key
	=========  ======  ==================================================================
	
* Example::

	{
		"type": "ask_key",
		"timestamp": ​1527151205790​,
		​"source": {
			"type": "user",
			"user_id": "jimmy.chen"
		}
	}