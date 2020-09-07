# What to select when you're connecting

Communication is key to the success of any project.
Picking the right tool won't automatically make your distributed work successful, but the tools you use to communicate play a part in how effective your communication is.
Recent discussions in projects where I participate have made me consider what tool selection looks like.
Should Discourse replace mailing lists?
Should Telegram replace IRC?
This chapter is not going to answer those questions.

There's no one right tool, just a set of considerations to think about in selecting communications tooling.
Each organization needs to arrive at a consensus about what works best for its workflow and culture, bearing in mind that the decision may attract some participants while driving others away.
While some tools naturally favor certain kinds of interaction, your organization's culture matters more.

## Categories of communication

In this chapter, I broadly lump tools into two categories: *synchronous* and *asynchronous*.
Synchronous tools are designed for real-time interaction when participants are active at the same time.
This includes various chat platforms, as well as voice and video call platforms.
Asynchronous tools do not rely on participants being active at the same time.
Email is perhaps the quintessential asynchronous platform, but forum tools, Kanban boards, and social media platforms are also good examples.

Of course, you can reply to an email immediately and you can let a chat message sit until tomorrow.
Many tools can be used for both to a decent approximation, but most will pretty obviously fall into one category or the other.
Because you can bend a communication tool to cover both categories of communication, you may be tempted to fit all of your communication into one tool.
Picking one tool to rule them all is a valid option, but be aware that it immediately favors one category of communication over the other.
Plus, the more a tool does, the less likely it is to do those things *well*.

## Pick one

You should pick no more than one tool for a given purpose.
Otherwise, confusion reigns.
Years ago, I worked for a company that used consumer Skype for chat and voice-over-IP.
It wasn't great for the purpose, but it worked well enough.
Then someone discovered Slack, and we moved to that.
Well, the engineering teams did.
Marketing, sales, and administrative teams stayed on Skype.
Then we started using Screenhero (later purchased by Slack) for screen sharing.
Then Microsoft bought our company and we switched to Skype For Business and Microsoft Teams.
But we kept using Slack for a while.

Similarly, the Fedora Project has used IRC for chat from the beginning.
Recently, some contributors have started using Telegram, often bridged to the IRC server.
Some people also use Element, also has an IRC bridge for many channels.

Twenty years ago, I chatted with my friends on AOL Instant Messenger.
Now I chat on SMS, Signal, Google Chat, Telegram, Whatsapp, Facebook Messenger, Twitter DMs, Snapchat, Slack, and probably more that I can't remember.
I tell you all of this to provide evidence for what I call "Cotton's Law of Communication": the number of communication platforms you use only increases.
Do your best to keep entropy in check by intentionally choosing one platform and sticking with it.

The boundaries should be made clear.
If it's an organization-wide decision, that's fine.
It's also okay to have different teams within an organization using different tools, so long as people who want to participate know where to look.
The gotcha here is that any communication across teams will require being on multiple platforms, and there you go increasing the number of tools you use.

## What to select

The remainder of this chapter provides some considerations for tool selection.
These are generally offered as tradeoffs with X or Y framing.
They are not presented in a particular order.
Your priorities are your own and you will have to weight each consideration appropriately.

The first section covers considerations that apply to both synchronous and asynchronous tools.
The next two sections look at those categories in turn.

### Considerations for all tools

**Safety.**
Unlike what I said above, this first consideration is presented in a particular order.
I include it first because you should consider it first.
You may want to think that everyone in your organization is great and would always behave.
The entirety of human history begs to differ.

At some point, you will need to deal with safety issues.
This is particularly true if you use publicly-available tools (see below).
The worst time to learn about your platform's safety features is after they're needed.

Ben Balter wrote a [blog post describing seven safety features](https://ben.balter.com/2020/08/31/trust-and-safety-features-to-build-into-your-product-before-someone-gets-hurt/): blocking/muting, reporting, hiding content, preventing new content, community guidelines, auditability, user consent.
while he approached it from the perspective of tool developers, it's instructive for tool selection, too.
If the tool you're looking at does not include the seven features, you may want to reconsider if it will meet your needs.

**Self-hosted or externally-hosted.**
Do you have the resources to maintain the tool—both human and monetary?
If you do, that's a way to maintain control, but it's also time that your organization can't spend working on whatever it is you do.
Externally-hosted tooling (either free or paid) might give you less flexibility, but it can also be more isolated from internal infrastructure outages.

**Open source or proprietary.**
This is entirely a value judgement for your organization.
For some communities, anything that's not open source is a non-starter.
Others might not care at all one way or another.
Most will fall somewhere on the spectrum between.

**Federated or centralized.**
Can the community connect their own tools together (e.g. like with email) or is it a centralized system (like most social media platforms)?
The trend is definitely toward centralized systems these days, so you may have to work harder to find a federated system that meets your needs.

**Public or private.**
Can outsiders see what you're saying?
For many open organizations, public visibility is important.
But even in those organizations, some conversations may need to take place in private or semi-private.

**Archived or ephemeral.**
Do you want to be able to go back and see what was said last month, last year, or last decade?
Some conversations aren't worth keeping, but records of important decisions probably are.
Does your tool allow you to meet your archival needs?

**Third-party clients.**
Does the platform allow for third-party clients, or do you have to use the official client?
People may want to use different clients to get a particular behavior not offered in the official tool.
This can be an important consideration for people with accessibility needs.

### Considerations for synchronous tools

Sometimes you really need to talk to people in real time.

**Mobile experience.**
People do a lot on their phones, if they travel frequently or if their ISP has an outage.
What is the mobile experience like for the tools you're evaluating?
It's not just a matter of if clients exist, but the whole experience.
If the user disconnects while on an airplane, do they lose all the messages that were sent in their absence?

**Status and alerting.**
What happens if someone stays logged in and goes away for a little bit?
Do they have the ability to suppress notifications?
Is there any way to let others know "I'm away or busy, don't expect an immediate reply"?

**Audio, video, and screen sharing.**
Sometimes you need the high-bandwidth modes of communication in order to get your full message across (or just shortcut a lot of back-and-forth).
Does the tool you're looking at provide this?
Is it usable for those who can't participate due to bandwidth or other constraints?

**Integrations.**
Can you display GIFs?
The ability to speak entirely in animated images can be either a feature or a bug, depending on the organization's culture.
But if it's important one way or another, you'll want to make sure your tool matches your needs.
Of course, there are other integrations that might matter too.
Can your build system post alerts?
Does the tool automatically recognize certain links and display them in an particular manner?

### Considerations for asynchronous tools

Of course, you're not all going to be sitting at your computer at the same time.
People go on vacation.
They live in different time zones.
They step away for 10 minutes to get a cup of coffee.
Whatever the reason, you'll need to communicate asynchronously sometimes.

**Push or pull.**
Email is a push mechanism.
Your message arrives in my inbox whether I've asked it to or not.
Web fora are a pull mechanism.
I have to go check them (yes, some forum tools provide an email interface).
Which works better for your workflow and community?
Pull mechanisms are easier to ignore when you want to step away for a little while, but they also mean you might forget to check when you do want to pay attention.

**Is it a ticket system?**
I haven't really talked about ticket systems/issue trackers because I don't consider them a general communication tool.
But for some projects, all the discussion that needs to happen happens in GitHub issues or another ticket tracker.
If that works for you, there's no point in adding a new tool to the mix.
