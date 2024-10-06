+++
title = 'Perils of key management'
date = 2024-10-05T11:26:05+07:00
draft = false
+++

When design and reviewing the security of a crypto exchange one of the things that came up was how to secure the users funds in the best way. So started to think about a cold wallet  design. Where just a fraction of the users fund would be online during the day to cover for any withdrawals but most of the funds would be transfered at the end of the day to a cold wallet address that could only be accessed offline by use of multiple key custodians. There are different level of support for multi signature for the biggest crypto currencies that allow  a wallet to be protected by multiple people each having their own private key. The currencies i was dealing with was etherium and bitcoin primarly. There is a lot to say about the technical aspects of this but in this article i mostly focus on the management of keys and lessons learned that can be useful for anyone doing this kind of work. 

I had the chance to talk to Vitalik Buterin briefly, the creator of etherium about this topic also and while he more focused on the mathematical details of these systems, it still gave some good insights overall. One, he mentioned that "mathematical" having smaller amounts and divide things into smaller chunks could decrease risk. This can be extrapolated as having smaller wallets also, but also smaller transaction sizes etc. But is a good and most likely quite obvious insight in that you cannot loose what you don't have. The other insight i got from this conversation was that he mention they used Multisig on the etherium foundation wallet and they almost lost access! This stayed with me and will write a little about what can and most likely happens in most cases. 

There was another instance of something that happened later with another wallet outside of this crypto exchange i was involved with. It also had Multisig and was divided between 5 people. Requiring 3/5 to access the funds. 3 of the people was in one company and 2 of the people was in another company. There, also a incident happened that almost stopped large transactions from happening. 

In the case with etherium foundation, while i don't know all details and he only mentioned very short they did have multisig, unsure how many people was needed but it was apperent they almost lost access but finally found the last key needed to unlock and access all thefunds. They later improved on their procedures but it was a close call. Would etherium even excist today if they did not manage?

In the case with the other wallet, the 3 people from one company refused to cooperate and there was a legal dispute until a deal was reached in the end, allowing the access to funds but during a couple of days. The two founders that started the wallet was locked out. 

I believe with these incidents, the common pattern of only having 2/3 is def not recommended. There are too many unknowns. Such as lost keys, forgotten passwords, disgruntled employees etc. 3/5 is better but is not enough just to have it put in place. The importance of key cermonies where you test the keys are not to be understated. You would need to put in quite a lot of time to really make sure you have the correct key management procedures, the more often the better. Also clear responsibility for anyone of the key custodians to report if they lost, forgot their keys etc. Proper training how to store keys, backup of keys and so on.

Also so important to select the people that going to be key custodians. Do you have 5 people that are dilligent enough in your organization? It is not always easy to find. You don't want to replace the people too often.

Also, i noticed that when someone leave as a key custodian or a new one will come. It is not always easy to just replace them and you will need the correct procedure for this. In etherium with smart contracts, it was easier and replacement of keys could be made but for bitcoin a new wallet was most likely to be created.



