# Verifiably Secure Elections

> Democracy is the worst form of government, except for all the others.

~ Winston Churchill

## Abstract
*We herein propose an electorial system which aims to address the key security issues
with elections, but does so in a way that can be independently verified with minimal
technical or domain knowledge.*

## 1. Philosophical Foundation
It should be obvious that elections ought to be free, fair, secure, and verifiable.
Not only because the free and fair election is central to a democratic government's
assertion that revolution is immoral, but also because electoriates have proven to be
*reliably* better decision makers than technocrats.

Unfortunately there is a persistant anti-democratic myth within "educated" circles
that government should be run by the "adults in the room". This myth may give rise to
the idea that a little bit of election fraud is sometimes at least partially
justifiable "for the greater good".

While it's not important to the technical solution, we consider that it is worth
debunking this myth, lest it otherwise fester in the mind of the reader as we present
our proposal.

As long as the democratic process has existed, technocrats have argued that the
democratic process results in rule by the mediochre, and claimed that superior results
will emerge from rule by the smartest / wisest.

Much of this thinking is owed to Plato, who artfully and persuasively argued for rule
by a "Philosopher King", but in
[The Open Society And Its Enemies](https://archive.org/details/in.ernet.dli.2015.59272),
Karl Popper did a very good job debunking this idea, in particular pointing out that
there were no less than 9 of Plato's own puples and associates who became tyrants.

In [Seeing Like A State](https://archive.org/details/seeinglikestateh00scot_0)
James C. Scott documented specific "well intended projects" of technocratic central
planning which devolved into horrific atrocities.

Nassim Taleb further identified this anomoly of underperforming experts in his
[Skin In The Game](https://en.wikipedia.org/wiki/Skin_in_the_Game_(book)), and went on
to theorize about the underlying mechanism.

Finally, in the short video [Rules for Rulers](https://www.youtube.com/watch?v=rStL7niR7gs)
CGP Gray made an incredibly well argued and accessible analysis of the game theoretical
forces which prevent autocratic governments from becoming anything other than the
tyranical hellscape we all know as "dictatorship".

## 2. Significance of Verifiability
Among the elections conducted around the world, some appear to be very well conducted,
others are little more than play-acting. Unfortunately, even carefully administored
elections can rarely differentiate themselves from shams. The objective of this document
is to define a process by which an election board can administor an election whose
security properties are independently verifiable.

Verifiably secure elections not only benefit the institution of government by putting
to rest reasonable challenges to it's legitimacy, but also help to establish a yard stick
by which other governments may be compared by businesses and investors.

It is foreseen that verifiably secure elections, once established in a few localities,
may spread as stakeholders demand the additional transparency.

## 3. Objectives
It is the objective of this project that the security properties of the election should be,
to the greatest extent practical, "obvious to a regular joe".

The design should go out of it's way to make things verifiable, even if they are unlikely
to be targets of vote fraud.

Where security properties can't be made obvious, they should be independently verifiable
by any field expert.

## 4. Scope
In order to establish the security of an election, or indeed of anything, we need to first
identify what it is that we want to prevent.

1. **Fake votes**: How do we know that nobody "stuffed the ballot box"?
2. **Switched Votes**: How do we know that our votes were counted as we cast them, and not
changed by a counting machine?
3. **Bribery & Intimidation**: How do we ensure that nobody is being paid, or pressured,
to vote in a certain way?

The standard answer to the challenge of **Switched Votes** is voter a receipt - but giving
people a ticket which indicates how they voted creates a huge issue with
**Bribery & intimidation** because local mafias may demand, or pay, for the ticket.

As of now, we are not addressing impediments to voting - such as not enough voting stations
or police blocking people who are going to vote. These threats are very real, but very
difficult to address in an independently verifiable way. If we identify a solution to these
challenges, we may update the document at a later date.

What will never be in scope is "voter stupidity" or "misinformation" or the like. These
matters are controlled for via constitutionally limited government and separation of powers.
Any action taken under the pretense of being smarter than the electoriate is itself an
affront on the democratic process and, as demonstrated in [1](/#1__Philosophical_Foundation),
has no justification beyond a discredited technocratic myth.

## 5. Blockchain and Publishing
Much ink has been spilled about the vague idea of "voting on the blockchain" but with without
any specific detailed proposals. We consider that a public blockchain such as Bitcoin is
useful for the purpose of time-stamping the publication of data, but beyond this simple
timestamping use case, we find blockchain to be unfit for the purpose.

Blockchain timestamping is often referred to as "blockchain notary". It does nothing to prove
a message's authenticity but it does create a record of the message having been crafted
*at a certain time*.

## 6. The Voter Registration List
The name and city of residence of each person on the voter registration list is published,
though not the address, date of birth, or any other personal information. This allows
political parties to present legal challenges to the voter roles based on people who dead or
have moved elsewhere.

## 7. The Ballots
* Ballots are printed on forgery resistant paper, like money.
* They also have serial numbers, like money.
* These serial numbers are sequencial and a box of ballots sent to a particular polling
station shall have a single range of sequence numbers.
* The manufacturer of the ballots shall create no more ballots than 1.5 times the number of
registered voters.
* The manufacturer publishes the sequence ranges of all ballots in each box that is sent out
to a polling place.

## 8. Cohorts
At each polling place, the people who pass through are grouped into cohorts of between
200 and 1000 people. This allows *most* of the information about the election to be made
public while maintaining plausible deniability regarding how people actually voted.

The names of the people in each cohort are published, and the final tally of the vote is
published, but the mapping of person to vote is un-linkable.

## 9. Voting Process
If it wasn't obvious already, voting must be done in person with an identity document.
Voting by mail or electronically, currently, has too many unknowns to be practical in the
context of trying to create verifiable security.

1. When a voter goes to the voting center, there are three poll workers checking ID to enter.
2. They step up to one of the poll workers and present identification, the poll worker
checks their finger for election ink and checks on a phone app that they are registered to
vote and have not yet voted.
3. Once they are confirmed, the poll worker puts election ink on their index finger and lets
them pass the desk into the building. The building has a single-wide door which is guarded
by a security guard whose job it is to ensure that nobody enters without a poll worker
having validated them first.
4. Once inside the building, the voter enters a lobby where there are two people at a desk
who are handing out ballots. Both of the poll workers are taking ballots from the same box.
The reason for this layout is so that there is no chance of a line forming between the ID
checkers and the ballot providers, which would potentially de-anonymize voters.
5. The poll worker handing out ballots checks that the voter has ink on their index finger
but not middle finger, then scans each ballot with a phone app. Scanning the ballot
"activates" it. Ballots which have never been activated are not considered legal.
6. After scanning the ballot, the poll worker stamps it with an official ink stamp so that
it is identified as active, and hands it to the voter.
7. At this point, the voter takes the ballot to a voting booth and casts their vote.
8. Walking out of the voting booth, the person puts their ballot into the counting machine
and as they leave, a poll worker dips their middle finger in election ink.
9. The counting machine takes a scan of each ballot, the images of which will be published.

Ballots are kept, on paper, for 7 years in case of any legal challenge to the vote.

## 10. Verifying Your Vote
A person who wants to verify their vote, at risk of losing some of their anonymity, may
take out their phone during the voting process and take a photo of the ballot's ID number.

The ballot has no tear-off section because this creates an intollerable risk of
**Bribery & Intimidation** attacks. However, the ability to photograph one's own ballot
while voting already exists today, so the addition of a serial number which can be
independently verified later is deemed not to add any intollerable risk.

## 11. Databases
A public database stores:
* The information about each ballot in a cohort
  * The name of the poll worker who activated the ballot
  * The machine-interpreted tally of the vote
  * The scanned photo of the ballot
* The names of each voter who voted in a cohort and the name of the poll worker who
checked their ID

## 12. Applications
The workers at the polling place use phone apps which work on any modern mainstream
telephone. They are expected to bring their own device and install the app on that device.
The state prepares a list of validated phone models from the most popular personal devices.
The apps use the secure computation value on the Android or iPhone OS.

In deciding between state issued electronic devices and BYOD, we determined that BYOD had
a superior risk profile because while one clever and devious poll worker might hack their
phone to try to attack the process, election device companies are a much greater attack
vector.

The phone app to be installed on the devices is open source and compilation is validated
by multiple independent parties using Reproducible Builds.

The same app works for both the people checking ID and the people activating and handing
out ballots. In both cases, the phone stores the data locally until the cohort has
completed and only then is it uploaded to the public database, with all entries sorted
alphabetically/numerically such that there is no way to link a person to a ballot based
on time.

## 13. Voting Machine
The voting machine must be produced by a voting machine, or scanner/printer company. It
must run open source software which is compilation is validated by multiple independent
parties using Reproducible Builds.

The voting machine must have a single removable memory chip only, which contains the
validated software, it will not be accepted if it contains any other persistant storage
chip.

The voting machine must be incapable of marking or modifying the ballot in any way, it
is forbidden to contain any form of ink.

After voting is completed, all voting machines are quarentined and sent to security
inspection labs where a random selection of them are examined to verify that the memory
chip contains only the validated software.

The hardware manufacturer must post bond before answering the RFP and in case the voting
machine is out of compliance they must pay a large fine.

## 14. Security Discussion

### 14.1. Fake Votes
The **Fake votes** attack takes on a few different forms.

1. Ballots are printed off in a warehouse, filled out, and then dumped into the stream of
ballots to count. This attack fails in three ways:
  * Firstly the ballots are difficult to print off because they are on forgery-resistant
  "security" paper.
  * Secondly, the people printing the ballots will not be able to get the correct ID
  numbers for the polling place where the ballots are to be counted.
  * Third, there will be no evidence of a poll worker having activated the ballots before
  they are counted.
2. Voting multiple times is heavily limited by the use of election ink:
  * Scenario 1 requires collusion of everyone at a polling place:
    * The person checking IDs would have to either allow voters to pass despite having
    election ink on both fingers.
    * The person handing out ballots allows voters to pass despite having election ink
    on both fingers.
    * The person managing the exit allows voters to pass despite having election ink
    on both fingers.
  * Scenario 2 requires collusion of poll workers at 2 stations:
    * The person checking IDs allows voters to pass despire having election ink on one
    finger.
    * The person handing out ballots is unaware.
    * The person managing the exit does not dip the voter's middle finger in election ink.
  * Scenario 3 is the same as Scenario 1, except with no ink rather than ink on 2 fingers.

### 14.2. Switched Votes
Switching votes needs to happen either inside of the voting machine, or at the public
central database.

1. Switching votes in the voting machine is limited by the fact that the voting machine's
software is open source and audited.
2. Switching votes at the public database is made difficult by the fact that each ballot
comes with a photographic scan which means switching requires large scale forgery.

Furthermore, there is no knowing which voters have photographed their ballot's serial
number and will go on to verify the vote later, so indiscriminently switching votes is
highly risky because any of these people may raise a legal challenge which will cause the
original ballot to be unearthed from the storage warehouse, re-scanned, and republished
with a criminal investigation of any wrongdoing.

### 14.3. Bribery & Intimidation
This is perhaps the most challenging issue to account for. There have been cases of local
mafias using write-in fields to pressure local community members to "sign their vote" so
it can be linked to them when the (corrupt) city official is counting ballots.

Generally speaking, write in fields should be strenuously avoided because they create too
much risk of linkability.

As long as voters are permitted to bring their phone into the voting booth, there is no
realistic way to prevent mafias from demanding that they provide photos of their ballots.
As there is no direct link between the names of voters and their ballots, this is the
most realistic attack model for **Bribery & Intimidation**, and since it is already
present in current voting schemes, it is considered "not worse".

### 15. Failure modes
.... TODO