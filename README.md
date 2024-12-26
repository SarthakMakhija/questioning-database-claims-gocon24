# Questioning database claims: Design patterns of storage engines
Material for the gocon-india 24 talk

[Questioning database claims_ Design patterns of storage engines (Presented).pdf](https://github.com/user-attachments/files/17988243/Questioning.database.claims_.Design.patterns.of.storage.engines.Presented.pdf)

The recording of the talk is available 
[here](https://www.youtube.com/watch?v=_55OM23zhUo).

The article describing the journey of my talk - from brainstorming the topic and building the presentation to running mock sessions and delivering the final talk, is available [here](https://tech-lessons.in/en/blog/behind_the_mic_my_journey_to_delivering_a_conference_talk/).

I made a mistake with MongoDB.
Phil Eaton pointed it out that the default write concern "majority" actually implies "j: true" which means data is synchronized (i.e. fsync-ed) before returning a success to a client.
