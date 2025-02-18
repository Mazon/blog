+++
title = 'Mistakes in incident management ive done'
date = 2025-02-18T11:06:00+07:00
draft = false
+++

There was a large incident at Unibet around 2015. The platform stopped working and it had something to do with a nosql database it seemed. As i was working as security engineer / manager at the time i was not directly involved with the incident, but i sat in a large open landscape with the people working on it. There was many clients connected to this nosql database and people could not figure out why some connected, then disconnected, some crashed some worked etc. Was really weird behaviour and the platform was in real pain. Sometimes people could login but overall most of the time things was more or less down. I sat and was frustrated that they could not solve it and on the third day i had enough. Yes! the platform was up and down and only partial working of 3 days! I did a quick google search and found a bug ticket on that products github talking about a client version problem that could happen under some circumstances. There was a new version of the client driver availble. 

I mention this to one of the engineers working on the problem and they agreed this was interesting. After deploy of the new client everything started working as expected. At the time i was mostly selfish and proud of myself, while i did not take any credit publicaly for it and very few people actually know i was the one that solved it. In secret i felt proud i solved the longest downtime the company yet to have i believe. 

I think now i did wrong. It is not certain but if i had started helping from my end directly when seeing that the people working on the incident could not solve it within a short period of time, even tho it was outside my role, job function whatever. Maybe, we could have solved the incident sooner. Think this is a good lesson for anyone at a company that regardless of role and your job there might be something you can help with. In some cases the best is to only stand back to not get in the way but keep looking for opportunity to support. Over and out.
