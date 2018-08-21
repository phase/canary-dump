# Votifier

| Info Ripped |  |
|--|--|
| Version                  | 1.9 |
| Authors                  | VisualIllusions, darkdiplomat |
| Category                 | Administration, Information |
| CanaryMod Target Version | 1.1.2 |
| License                  | GPL v3 |
| Source Code              | https://github.com/Visual-Illusions/votifier |


Original Description:

---

 Votifier 1.9

What is Votifier?

Votifier is a plugin whose purpose is to get notified (aka votified) when a vote is made on a Minecraft server list for the server. Votifier creates a lightweight server that waits for connections by a Minecraft server list and uses a simple protocol to get information about that vote. Votifier is and always will be open-source.
Is it secure?

Votifier employs 2048-bit RSA encryption to ensure that nobody can spoof a vote packet. When Votifier is run for the first time, it generates a unique key pair only for your server to use. When you register Votifier with a supporting server list, that server list will ask for your public RSA key so it can encrypt vote packets before sending them to you. Votifier is so secure, not even its own developers can hack it.
What does Votifier do when it receives a vote notification?

Votifier has a vote listener system where listeners are notified when Votifier receives a vote notification. Sort of like the Bukkit plugin system itself. Each of these listeners can carry out their own task (i.e. rewarding the player via iConomy, etc.) in response to the vote.

To install a vote listener, simply put it in Votifier's listeners folder.
Note that you must run Votifier first before this folder is made.

For having a log of votes, the 
[FlatfileVoteListener](https://web.archive.org/web/20150325075749/https://github.com/downloads/vexsoftware/votifier/FlatfileVoteListener.class)
can be used. This listener logs votes to a text file located at config/Votifier/votes.log
Where can I find vote listeners?

Vote listeners can be found at the vote listeners forum. PENDING CANARY
How do I write a vote listener?

Information about how to write a vote listener can be found on the vote listeners page on the VexSoftware wiki.
How can my server list support Votifier?

Information about Votifier's protocol can be found on protocol documentation page on the VexSoftware wiki.
