Tell us what your idea is
=========================

Where is my phone?
Where are my keys?
When will my wife be back?

These are questions that I ask myself every day several times.
Wouldn't it be great if an electronic personal assistant could answer those?
We made extensive tests and there are lots of signals that can be used to determine the answers to those questions:
Bluetooth LE becomes more and more ubiquitous and nearly everywhere you can get several wifi signals.
The problem is that those signals are very unsteady and change when people move around.
We will use machine learning to determine locations from those signals.
Even harder but feasible are geo-information and probabilities for people's movements.
We will use this information to answer the questions from above.

Where is my phone? On the couch!


Tell us how you plan on bringing it to life
===========================================

Sample code: see this repository

Google has extensive knowledge on how to determine the location of a phone while using minimal battery power - Android's geofencing is an excellent example for that.
Getting the opportunity to talk to the people who implemented geofences would be awesome.
Until then we will keep sampling our environments and get as much information as possible.
So far we record the signal strengths of mobile network, wifi networks, bluetooth and bluetooth LE signals.
We also record the measurements of the acceleration sensor to detect device movements.
The plan is to use the signals to determine the location once the phone stops to move.
Register the location on a cloud server and go to sleep until the phone moves again.

The problem is the location detection step.
While in certain circumstances it is very easy, e.g. "I see a strong signal of the bluetooth of the car, so I am in the car", other situations are not so easy to detect, e.g. if you are close do open doors between rooms.
We experiment with different ML algorithms to see what yields the best results.
As of now decision trees look promising.

The cloud part is functional on Google Cloud as is an Alexa integration (we don't own a Google Assistant and had experience with Alexa from earlier projects).

As the simple cases already work, we are sure to be able to present something on May 1st 2020.


Tell us about you
=================

I am a software developer since I was 11 - so for 36 years now, which gives me a broad experience from tiny embedded systems to massive parallel cloud server systems.
I currently work for Deutsche Telekom - the first 3 years in the cloud unit and the last 4 years in the smart home unit.
Therefore I have a broad experience with cloud databases, cloud computing as well as networking and I also know how to mangle individual bits and how radio waves work.
I do Android development since the 2nd Android developer challenge (back in 2010, right?).
I've won two "Random Hacks of Kindness" and came in second on a third one.
The "we" above is because I how some very experienced colleagues who helped me with several problems and challenged my ideas.

Some apps I've written:
https://play.google.com/store/apps/developer?id=Kurt+Huwig

My daily work:
https://play.google.com/store/apps/details?id=de.telekom.smarthomeb2c

Some cloud project I did in my spare time - which is now defunct as it turned out to be not interesting enough.
https://www.openwarner.de/


