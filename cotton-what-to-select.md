## What to select when you're connecting
Ben Cotton

Communication is key to any project's success. 
Recent discussions in open communities where I participate have made that clear to me. 
By and large, most of these discussions are about the merits of one communication tool over another.
Should Discourse replace mailing lists?
Should Telegram replace IRC?
This chapter is not going to answer those questions.

That's because picking the right communication tool won't automatically make your distributed work successful.
In fact, *there is no single "right" tool for your open team or organization*—just a set of considerations to think about in selecting communications tooling.
The merit of any tool isn't intrinsic to the tool itself.
It's a product of how well it solves a problem for your team.

Without a doubt, the tools you use to communicate will influence the effectiveness of your team's communication.
But every open organization needs to arrive at a consensus about which tools works best for its workflow and culture, bearing in mind that the decision may attract some participants while driving others away.
While some tools naturally favor certain kinds of interaction, your organization's culture matters more.

So let's review some considerations you might make as you select the tools for connecting your distributed team.
 
### Categories of communication

In this chapter, I lump tools into two broad categories based on the kind of communication they facilitate: *synchronous* and *asynchronous*.
Synchronous tools are designed for real-time interaction when participants are active at the same time.
This includes various chat platforms, as well as voice and video call platforms.
Asynchronous tools do not rely on participants being active at the same time.
Email is perhaps the quintessential asynchronous platform, but forum tools, Kanban boards, and social media platforms are also good examples. 

Of course, the categories blur a bit; you can reply to an email immediately and you can let a chat message sit until tomorrow.
But most pretty obviously fall into one category or the other. 
Because you can bend a communication tool to cover both synchronous and asynchronous categories, you may be tempted to fit all of your communication into one tool.
Picking "one tool to rule them all" is a valid option, but be aware that it immediately favors one category of communication over the other.
Plus, the more a tool does, the less likely it is to do those things *well*.

### Pick one

Let me introduce you to something I call "Cotton's Law of Communication": the number of communication platforms you use only increases.

Years ago, I worked for a company that used consumer Skype for both chat and voice-over-IP.
It wasn't great for the purpose, but it worked well enough.
Then someone discovered Slack, and we moved to that.
Well, the engineering teams did.
Marketing, sales, and administrative teams stayed on Skype.
Then we started using Screenhero (later purchased by Slack) for screen sharing.
Then Microsoft bought our company and we switched to Skype For Business and Microsoft Teams.
But we also kept using Slack for a while.

Similarly, the Fedora Project has used IRC since the beginning.
More recently, some contributors have started using Telegram, often bridged to the IRC server.
And other contributors use Element, which *also* has an IRC bridge for many channels.

Twenty years ago, I chatted with my friends on AOL Instant Messenger.
Now I chat with them on Signal, Google Chat, Telegram, Whatsapp, Facebook Messenger, Twitter, Snapchat, Slack, and probably more that I can't even remember.

You get the picture.

Don't let this happen to your team.
Pick no more than one tool for a given purpose.
Otherwise, confusion reigns.
And make those boundaries clear.
Maybe it's an organization-wide decision.
Maybe different teams *within* an organization are using different tools (fine, so long as everyone who wants to participate knows where to look).
Just note that in the latter scenario any communication across teams will require every to manage multiple platforms—and there you go, increasing the number of tools you use.

Cotton's Law.

Do your best to keep entropy in check by intentionally choosing one platform and sticking with it.

### What to select

In what remains of this chapter, I review some considerations you might make when your team is searching for a new communication tool.
Generally, I'll present them as a series of tradeoffs with "X or Y?" framing and in no particular order.
Your priorities are your own and you will have to weight each consideration appropriately.

The first section covers considerations that apply to both synchronous and asynchronous tools while the sections following that look at each of those categories in turn.

#### Considerations for all tools

**Safety.**
Contrary to what I said above, I present this consideration first because you should indeed consider it first.
You may want to think that everyone in your organization is great and will always behave themselves.
The entirety of human history begs to differ.

At some point, you will need to deal with organizational safety issues via your communication tool.
This is particularly true if you use publicly-available tools (see below).
The worst time to learn about your platform's safety features is after they're needed.

To ensure your tools promote organizational safety, I suggest reviewing Ben Balter's [list of seven safety features](https://ben.balter.com/2020/08/31/trust-and-safety-features-to-build-into-your-product-before-someone-gets-hurt/) in which a reliably safe tool should have: 

* blocking/muting
* reporting
* hiding content
* preventing new content
* community guidelines
* auditability
* user consent

While Balter approaches these issues from the perspective of tool *developers*, his list is also instructive for tool *selectors*, too.
If the tool you're looking at does not include these seven features, you may want to reconsider whether it will meet your needs.

**Self-hosted or externally-hosted.**
Do you have the resources—both human and financial—to maintain the tool yourself?
If you do, then that's one way to maintain control over your tooling.
But remember that time spent administering and troubleshooting communication tools is also time your team or organization can't spend working on whatever it is you do.
Externally-hosted tooling (either free or paid) might provide less flexibility, but it's also isolated from internal infrastructure outages.

**Open source or proprietary.**
This is entirely a value judgement for your organization.
For some communities, anything that's not open source is a non-starter while others might not care at all.
Most will fall somewhere on the spectrum between.
Will your team or organization wish to modify, improve, or extend the tool it's using?
If so, it'll need access to the tool's source code or design details, and an open source option might suit it.

**Federated or centralized.**
Email is a federated system; that is, people using it in different domains (@gmail.com, @hotmail.com, @fastmail.com, etc.) can still communicate with one another.
Conversely, centralized platforms *don't* allow that kind of cross-system communication.
(Consider many contemporary social media platforms.
Communication between Twitter and Facebook, for example, isn't possible.)
Will your team, organization, or community need to connect with others using their own instances or implementations of the same tool?
If so, a federated system might be desirable.
But as communication tools today seem to be trending toward centralized models, you may need to work harder to find a federated system that meets your needs.

**Public or private.**
Can outsiders see what you're saying?
Should they?
For many open organizations, public visibility is important.
But even in those organizations, some conversations may need to take place privately (or semi-privately).
Your open and distributed team will need to decide if (and how) to publicize certain aspects of its communication.

**Archived or ephemeral.**
Do you want to be able to go back and see someone said last month, last year, or last decade?
Do you want to maintain an easily referenced record of those conversations?
Some conversations aren't worth keeping, but records of important decisions probably are.
Your tool should allow you to meet your archival needs.

**Third-party clients.**
Does the platform allow for third-party clients, or do you have to use an officially supported client from the tool's developer?
People may want to use different clients to get a particular function the official tool doesn't offer.
This can be an important consideration for people with certain accessibility needs.

#### Considerations for synchronous tools

Sometimes you just really need to talk to people in real-time.

**Mobile experience.**
People do a lot on their phones, especially if they travel frequently or if their Internet service provider experiences an outage.
What is the mobile experience like for the tools you're evaluating?
(It's not just a matter of whether a tool exists, but whether it offers a desirable experience.)
If the user disconnects while on an airplane, do they lose all the messages sent in their absence?

**Status and alerting.**
What happens if someone stays logged in and walks away for a little bit?
Do they have the ability to suppress notifications?
Is there any way to let others know "I'm away or busy, don't expect an immediate reply"?

**Audio, video, and screen sharing.**
Sometimes you need the high-bandwidth modes of communication in order to get your point across (or just shortcut a lot of back-and-forth).
Does the tool you're looking at provide this?
Is it usable by those who can't participate due to bandwidth or other constraints?

**Integrations.**
Can you display animated GIFs?
The ability to speak entirely in images can be either a feature or a bug, depending on the organization's culture.
But if it's important one way or another, you'll want to make sure your tool matches your needs.
Of course, there are other integrations that might matter too.
Can your software build system automatically post alerts to your communication tool, for example?
Does the tool automatically recognize certain links and display them in a particular manner?

#### Considerations for asynchronous tools

Of course, not everyone on your distributed team will be sitting at their desks at the same time.
People go on vacation.
They live in different time zones.
They step away for 10 minutes to get a cup of coffee.
Whatever the reason, you'll occasionally need to communicate asynchronously.

**Push or pull.**
Email is a push mechanism.
Your message arrives in my inbox whether I've asked it to or not.
Web fora are a pull mechanism.
I have to go check them (yes, some forum tools provide an email interface).
Which works better for your workflow and community?
Pull mechanisms are easier to ignore when you want to step away for a little while, but they also mean you might forget to check when you do want to pay attention.

**Is it a ticket system?**
I haven't really talked about ticket systems/issue trackers because I don't consider them a general communication tool.
But for some projects, nearly all discussion essential to the project and team success happens in a ticket tracker (like GitHub issues).
If that works for you, there's no point in adding a new tool to the mix.
