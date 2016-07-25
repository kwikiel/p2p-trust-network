# p2p-trust-network

This is so far just some loose ideas

## Rationale

Often it's useful to be able to trust an online identity, i.e. for peer-to-peer lending sites, peer-to-peer home exchange sites, work assignments, etc.

Most often the various platforms (like Couchsurfing, Uber, BeWelcome, Loanbase, Localbitcoins etc) will have some built-in support for ratings; user account A can leaving positive feedback for B after A and B has had an interaction on that platform.  The ratings never leave the platform.  There are usually no ways to see the difference between a conman creating yet another fake account and a newcomer to the platform.  It is impossible for an outsider that have been scammed on one platform to leave a negative feedback warning users on another platform about the scammer.

What we need is a global network-of-trust system.  It should be truely peer-to-peer, it should be based on open standards and open source.  Just the risk of getting negative feedback on such a network could be enough deterrent to avoid certain types of scam.

## Features needed

A real person should be able to record personal details.

A real person should be able to record various online identities and link them up to the personal details.

A real person should be able to record different kind of trust in the system, like "I've met Peter and verified his ID documents", "I know the real person Peter has the username peter123 on Google Buzz", "Peter cannot be trusted", "I borrowed my car to Peter and he never came back with it", "I endorse Peter for his knowledge of greek ancient history", etc.

One should be able to query an online identity and if there is any kind of chain between you and this account it should be visible.

It should be easy to import/sync data from existing systems.  I.e, importing data from PGP "web-of-trust", importing data from sites like LinkedIn and Facebook, etc.

## Privacy and problems

Such a network will contain a lot of valuable metadata that can be abused in all sorts of ways - that's something to be concerned over.  One should consider smart ways to use encryption.

Such a network is also quite open to unjust revenge-attacks from angry ex-partners, etc.

## Implementation details

A global database - perhaps something blockchain-based?

## Existing works

* OpenPGP key signings is already some form of "web-of-trust"-network - but it has quite some weaknesses, it is only useful for connecting email addresses with real names.  A keysigning supposedly should be read as "I have checked the ID documents of Eve", though it's normal to skip the ID verification process.
* PeerTrust - http://www.cc.gatech.edu/projects/disl/PeerTrust/ - seems to be a white paper from 2004.  The "Related Work"-section contains only dead links
* Keybase - keybase.io
* Namecoin
* Orisi
* Onename
* TrustDavies http://earlbarr.com/publications/trustdavis.pdf
* 

Goodies from traity https://traity.com/faq

1. The first stage is the phase of identity. We have to know that you are who you say you are. I believe that, although this seems simple, it's one of the most impeding challenges of the reputation economy. It is purely a matter of transparency. We ask users to login with different social networks and we'll check that those networks seem legit (in terms of friends, content, when they were created, friends are legit themselves, etc.) and will check that the name is consistent across them, or that you have many of the same friends in the different networks. We'll also go offline, to ask you to upload your passport or ID, so that we can "verify it".We delete the picture, we just maintain the fact that "you verified yourself with the right name".
2. The next phase has to do with you. Your bio, your personality, your achievements. The more you tell us about yourself, the better for your transparency and the better to show others. This does not "prove" reputation in any way, because any person could write anything they want about themselves, but this is part of that subjective reputation where we might trust other people who are similar to us, and this is not about what is right or wrong, it's just about how/who you are.
3. The next phase has to do with studying your social networks. I mentioned this earlier, but there are more algorithms we are running. Who are your best friends, where do you spend most of your time, is it consistent with where your best friends spend time? If you say on LinkedIn that you worked for McKinsey, do you have friends in your network who also worked for McKinsey? If they did not, it might seem strange. This does not cover all aspects of reputation, but now if you want to fake a profile, you have to fake 500 profiles of 500 friends, and probably also their friends, so we are making it more difficult for people to fake their social identities.
4. The next phase has to do with recommendations. We ask your friends what they would recommend you for. They might think you are friendly, or disciplined, or any other trait. This is part of your reputation. These are actions within Traity. We are decentralising it so that you can give "badges" to other people for whatever you believe they have reputation. From being creative to being great leaders or being funny.
5. The more visual aspect is that we are integrating with different reputation webs like collaborative consumption companies. Sharing houses, sharing cars, etc. All of them have its own reputation system, which is very inefficient because users need to start from zero in every market. And if they have passport verification, you have to upload your passport to 100 sites. Not very efficient. This is what we call the ReputationAPI. When you give us access, we take reviews information from collaboration economy companies. Algorithms here don't play a big part. Aggregation is more important. If you think about it, eBay gives you the % rating and the number of transactions. The % is important (you want to see 99.9%) but the number of transactions as well. Less transactions is worse, more transactions is safer. Even if you see 98% in 50 transactions, you will want to read "the bad one," so that's why I say that algorithms are not so important here. It's all about transparency and letting people have access to the full history so that they can read the bad one, or whatever they want to make up in their minds.
