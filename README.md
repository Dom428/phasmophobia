General Gameplay

    Tutorial is 0.5 difficulty
    Amateur is 1 difficulty
    Intermediate is 1.5 difficulty
    Professional is 2 difficulty

Sanity

    Game internally uses insanity, which is then displayed as sanity in the truck as (100 - insanity) + Random.Range(-2, 3)

    Small map
        Normal drop rate: 0.12
        Setup drop rate: 0.09

    Medium map
        Normal drop rate: 0.08
        Setup drop rate: 0.05

    Large map
        Normal drop rate: 0.05
        Setup drop rate: 0.03

    Solo games (that are not a tutorial)
        Drop rates from above / 2

    Insanity
        Capped at 50 during setup phase
        Uncapped to 100 during regular play
        Increases every frame by ((deltaTime * setup/normal drop rate) * difficulty rate (below))
        Insanity does not increase when you are in light or are outside the house
        Light status updates every 2 seconds
        Insanity level is synced to other players every 5 seconds
        Being within 3m of a Jinn instantly increases your insanity by 25%
        Entering a recognised phrase into a Ouija Board has a 1-in-3 chance of increasing your insanity by 40%
        Sanity pills decrease your insanity by 40%
        Poltergeists increase your insanity by double the number of props they are allowed to move

    If the ghost is visible, or is in hunting phase, and is within 10m of the player, the player's insanity raises by deltaTime (time since last frame) * sanity drain strength
        Ghosts have a default sanity drain factor of 0.2
        Phantoms have a sanity draining strength of 0.4

Sanity effects

    The game will attempt to spawn ghosts at a window when the player is inside the house at a random interval between 10s and 30s if the player's insanity is above    50, otherwise at a random interval between 10s and 20s.
    This ghost will start far away from the window and dash towards the window until it is 0.2m away, then disappear
    Evidence
Dirty Water

    Ghosts will use a tap and spawn dirty water as soon as they enter a bathroom
    Ghosts leave a Ghost Interaction EMF (Level 2) on the sink

Freezing Temperatures

    Ghosts that have freezing temperatures as an attribute will make the room they are in go down to -10C (14F), while all other ghosts make the room drop to 5C (41F). However, your thermometer has a +-2C randomness, so as soon as you see your thermometer go below 3C or 37.4F, or if you see cold puffs when you are in a room, you can tick off Freezing Temperatures.

Ghost Orbs

    Ghost orbs only spawn in the ghost's favourite room, and can be seen in the doorway to that room from a hallway. This favourite room is designated on ghost spawn
    Ghost orbs can be seen before entering the house if a fixed camera is pointing at the door/hallway to their favourite room.

Ghost Writing

    Ghosts have a 5-in-12 chance of doing random interactions such as opening doors, throwing props, and writing in ghost books.
    The ghost book does not appear to need to be in the ghost's room. Yet to be confirmed.

Spirit Box

    Ghosts can only respond once every 10 seconds
    "Nothing detected" means the game recognised your phrase, but it triggered a fail check. However, fail checks and answers do not seem to be mutually exclusive.
    Ghosts that do not use spirit box will never respond
    Ghost responses only work if you are using Local Push to Talk (if you have push to talk enabled) or have a VR headset on. If you use Voice Activation, the ghost will always hear you.
    Ghosts will not respond if you are more than 3m away from them, or are on a different floor
    Ghosts that only respond to one person are shy
    Ghosts will not respond if the fusebox is on and a light switch in your current room is on
    Ghosts are more likely to respond to the Spirit Box if you have said their name in isolation (i.e. anger them with a phrase) recently
    Ghosts can respond with either location answers, difficulty answers, or age answers
        Different location sounds are played depending on whether you are at least 4m away from the ghost
            Difficulty questions:
                What do you want?
                Why are you here?
                Do you want to hurt us?
                Are you angry?
                Do you want us here?
                Shall we leave?
                Should we leave?
                Do you want us to leave?
                What should we do?
                Can we help?
                Are you friendly?
                What are you?
            Location questions:
                Where are you?
                Are you close?
                Can you show yourself?
                Give us a sign
                Let us know you are here
                Show yourself
                Can you talk?
                Speak to us
                Are you here?
                Are you with us?
                Anybody with us?
                Is anyone here?
                Anyone in the room?
                Anyone here?
                Is there a spirit here?
                Is there a Ghost here?
                What is your location?
            Gender questions:
                Are you a girl?
                Are you a boy?
                Are you male
                Are you female
                Who are you
                What are you
                Who is this
                Who are we talking to
                Who am I talking to
                Hello
                What is your name
                Can you give me your name
                What is your gender
                What gender
                Are you male or female
                Are you a man
                Are you a woman
            Age questions:
                How old are you,
                How young are you,
                What is your age,
                When were you born,
                Are you a child,
                Are you old,
                Are you young
Ghost behaviour
Car

    The car alarm can be turned on when the ghost is within 2m of the car. When the alarm is on, the car's headlights will also be on, and it will play some sounds.
    To turn it off, you need the car keys and hit Use on the car. As soon as the car alarm turns on, a Ghost Interaction EMF (Level 2) spot will be created at the car's position.

Doors

    As soon as a ghost with fingerprints touches a door, it will spawn the fingerprint evidence, but only on one side of the door. Fingerprint evidence does not spawn Ghost Interaction EMF
    Doors always lock during hunting phase, and will remain locked for a random amount of time between 10 and 20 seconds
    Doors all start with a locked timer between 5-20 seconds
    Ghosts make door knocking sounds when they are within 3m of the door, and create a Ghost Interaction EMF (Level 2) at the door's audio source location.
    Ghosts can close and lock doors randomly, which do NOT trigger Ghost Interaction EMFs.

Favourite Rooms

Ghosts stay in their favourite room for 30 seconds, then return to their idle phase
Footsteps

    Wraiths do not make black light footsteps after stepping on a salt pile
    Wraiths have an additional Wraith multiplier set to 50 after stepping in salt, making it less likely to start a hunting phase
    Ghost footsteps play at 5% volume during non-hunting and non-appearing phases
    When the ghost has appeared, footsteps are immediately played at full volume when in line of sight, then at 30% volume while you can still see the ghost
    During hunting phase, random hunting noises are played at full volume, then at 30% while you can still see the ghost

Fusebox

    Small houses can have a max of 10 lights on
    Medium houses can have a max of 9 lights on
    Large houses can have a max of 8 lights on
    The ghost spawns a Ghost Interaction EMF (Level 2) when they use the fusebox
    Ghosts have a 1-in-5 chance of turning the fusebox back on

Generic VOIP recognition

    Ghosts can react with your voice all throughout the game, even when you are not holding down a VOIP key

    You must be in the ghost room to trigger a response

    You must be in a room for more than 2 seconds for phrases to be recognised

    Shy ghosts will not respond to you if there are multiple people in the room

    Ghosts can react to their name at any time, even when you are not holding down a VOIP key, with a 20 second delay in between reactions

    Saying the ghost's name makes the ghost more likely to respond to the Spirit Box

    Saying just the ghost's first name is sufficient

    A generic ghost reaction will add a random value between 10 and 25 to their activity multiplier

    Generic reactions have a 1-in-200 chance of the ghost turning the fusebox off

    Generic reactions have a 1-in-8 chance of interacting with a random prop

    Generic reactions have a 1-in-8 chance of interacting with a random door

    Generic reaction phrases
        "Fuck",
        "Bitch",
        "Shit",
        "Cunt",
        "Ass",
        "Bastard",
        "Motherfucker",
        "Motherfucker", (yes, this is repeated. Probably indicattes a higher chance of them reacting to this)
        "Arsehole",
        "Crap",
        "Pussy",
        "Dickhead",
        "Bloody Mary"
        Plus 57 more that are language-specific. The English versions are provided below. For all langauges, refer to localisation.csv found in this repository, and search for Phrase_. All these are taken directly from the .csv, lack of punctuation, spelling errors, and all.
        Ghost behaviour
Car

    The car alarm can be turned on when the ghost is within 2m of the car. When the alarm is on, the car's headlights will also be on, and it will play some sounds.
    To turn it off, you need the car keys and hit Use on the car. As soon as the car alarm turns on, a Ghost Interaction EMF (Level 2) spot will be created at the car's position.

Doors

    As soon as a ghost with fingerprints touches a door, it will spawn the fingerprint evidence, but only on one side of the door. Fingerprint evidence does not spawn Ghost Interaction EMF
    Doors always lock during hunting phase, and will remain locked for a random amount of time between 10 and 20 seconds
    Doors all start with a locked timer between 5-20 seconds
    Ghosts make door knocking sounds when they are within 3m of the door, and create a Ghost Interaction EMF (Level 2) at the door's audio source location.
    Ghosts can close and lock doors randomly, which do NOT trigger Ghost Interaction EMFs.

Favourite Rooms

Ghosts stay in their favourite room for 30 seconds, then return to their idle phase
Footsteps

    Wraiths do not make black light footsteps after stepping on a salt pile
    Wraiths have an additional Wraith multiplier set to 50 after stepping in salt, making it less likely to start a hunting phase
    Ghost footsteps play at 5% volume during non-hunting and non-appearing phases
    When the ghost has appeared, footsteps are immediately played at full volume when in line of sight, then at 30% volume while you can still see the ghost
    During hunting phase, random hunting noises are played at full volume, then at 30% while you can still see the ghost

Fusebox

    Small houses can have a max of 10 lights on
    Medium houses can have a max of 9 lights on
    Large houses can have a max of 8 lights on
    The ghost spawns a Ghost Interaction EMF (Level 2) when they use the fusebox
    Ghosts have a 1-in-5 chance of turning the fusebox back on

Generic VOIP recognition

    Ghosts can react with your voice all throughout the game, even when you are not holding down a VOIP key

    You must be in the ghost room to trigger a response

    You must be in a room for more than 2 seconds for phrases to be recognised

    Shy ghosts will not respond to you if there are multiple people in the room

    Ghosts can react to their name at any time, even when you are not holding down a VOIP key, with a 20 second delay in between reactions

    Saying the ghost's name makes the ghost more likely to respond to the Spirit Box

    Saying just the ghost's first name is sufficient

    A generic ghost reaction will add a random value between 10 and 25 to their activity multiplier

    Generic reactions have a 1-in-200 chance of the ghost turning the fusebox off

    Generic reactions have a 1-in-8 chance of interacting with a random prop

    Generic reactions have a 1-in-8 chance of interacting with a random door

    Generic reaction phrases
        "Fuck",
        "Bitch",
        "Shit",
        "Cunt",
        "Ass",
        "Bastard",
        "Motherfucker",
        "Motherfucker", (yes, this is repeated. Probably indicattes a higher chance of them reacting to this)
        "Arsehole",
        "Crap",
        "Pussy",
        "Dickhead",
        "Bloody Mary"
        Plus 57 more that are language-specific. The English versions are provided below. For all langauges, refer to localisation.csv found in this repository, and search for Phrase_. All these are taken directly from the .csv, lack of punctuation, spelling errors, and all.
        Can you speak
            Show us
            Let us know you are here
            Do something
            Is there anyone with me
            Scream
            Are you alone
            Can we speak
            would like to speak to you
            Is there anyone here
            May I ask you
            Can you speak to us
            Would you like to talk
            Are you the only one here
            Are you waiting
            Is there anything that I can do
            Do you know who we are
            Are you happy
            Are you here all the time
            Are you male or female
            Are there children here
            Do you want us to leave
            Make a noise
            Can I ask you
            Can you make a sound
            Show us your presence
            Knock something
            Make a sound
            Open the door
            Throw something
            Talk to me
            Talk to us
            We mean you no harm
            Open a door
            We are friends
            Is this you're home
            Can you speak to us
            I'm scared
            I am scared
            scared
            scary
            spooky
            Horror
            Scare
            Open this door
            Frighten
            panic
            Fright
            Hide
            Run
            Show your presence
            Show us
            Show me
            Turn on the light
            Turn off the light
            Are there any ghosts
            Give us a sign
