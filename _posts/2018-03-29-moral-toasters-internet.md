---
layout: post
title: 'Moral Toasters and an Internet of Ethical Things'
bibtex: true
img: holy-toaster.png
comments: true
---

_After reading a [new paper](https://link.springer.com/article/10.1007/s11948-018-0030-8) arguing that the development of morally competent artificial agents isn't justified, I started thinking about ethical reasoning capabilities for various physical objects, including the mighty toaster._

I recently read an interesting article, titled ["Critiquing the Reasons for Making Artificial Moral Agents"](https://link.springer.com/article/10.1007/s11948-018-0030-8), by Aimee van Wynsberghe and Scott Robbins, in which they argue that the reasons used by people like me (people who propose explicitly designing robots/artificially intelligent agents to behave ethically) to justify our endeavor fall apart on further analysis.  It's an interesting argument, and you should read it. I disagree with a lot of their points; maybe some other time I'll try to write a thorough rebuttal.  Anyway, that's not what I'm hoping to accomplish in this post.

One thing van Wynsberghe and Robbins are arguing against is a notion of inevitability.  We artificial moral agent (AMA) designers tend to argue that robots will surely be placed in contexts in which they'll need to make moral decisions, and that we must therefore prepare them to make these decisions.  van Wynsberghe and Robbins cite my advisor, Matthias Scheutz, who says the following:

> Any ordinary decision-making situation from daily life can be turned into a morally charged decision-making situation, where the artificial agent finds itself presented with a moral dilemma where any choice of action (or inaction) can potentially cause harm to other agents. (Scheutz, 2016)

van Wynsberghe and Robbins accuse Matthias of implying that things like the robotic arms in factories and vacuum-cleaning robots should be turned into AMAs, and those robots are doing just fine without explicit ethical algorithms, thank you very much.  If it sounds like they're exaggerating Matthias's position... not really.  While I don't speak for Matthias (so there's always the possibility that I'm wrong here), I can confirm that in [one of my papers](https://hrilab.tufts.edu/publications/kasenbergscheutz18aaai.pdf) we demonstrate our norm conflict resolution algorithm on a set of simple dilemmas _that a vacuum cleaner might conceivably face if you gave it norms for self-preservation and not harming a human in addition to the usual "you should clean stuff" objective_.  I've joked that our goal is to give as much inner turmoil as possible to simple robots.

According to van Wynsberghe and Robbins, this is a slippery slope leading to the logical conclusion of Matthias's position: "that _any technology_ that one interacts with and for which there is a potential for harm (physical or otherwise) must be developed as an AMA and this is untenable" (van Wynsberghe and Robbins, 2018; emphasis mine).  This accusation is extreme, and we shouldn't explore it any further.

Let's explore it anyway.

The sort of argument van Wynsberghe and Robbins seem to be making here is a _reductio ad absurdum_ ("reduction to absurdity"), in which you try to disprove a statement by showing that it leads to absurd consequences.  The absurd consequence here is the idea that every device should be turned into an AMA, including "your tv, phone, fridge, alarm clock, kettle, etc" (van Wynsberghe and Robbins, 2018)- but is this really that absurd?

## Types of ethical agents

In a [frequently-cited 2006 paper](http://ieeexplore.ieee.org/document/1667948/), philosopher James H. Moor outlined four different levels of artificial moral agent:
* **Ethical impact agents**: systems that can have some sort of ethically-relevant effects on the world.  This is a pretty broad category, as we'll see.
* **Implicit ethical agents**: (more or less) systems where the designers/programmers were thinking about ethics, and so they put in some mechanisms to prevent the system from doing certain bad things. An obvious example would be a car that automatically brakes instead of hitting a pedestrian.  The car isn't *thinking* about ethics, but nevertheless some ethical behavior is designed in.
* **Explicit ethical agents**: systems that can reason about and make decisions using moral and social norms/principles/virtues/utilities/whatever.  They "think about" ethics explicitly.  Usually when we talk about AMAs, this is what we're referring to.
* **Full ethical agents**: systems that have consciousness, free will, intentionality, all that good stuff.  This category is limited to humans for the foreseeable future.

Moor designed this hierarchy primarily to think about AI-ish systems, but the analysis isn't limited to computers.  For starters, we note that *almost every thing has an ethical impact*.  Your TV certainly does: it can show you things that influence your worldview and future actions, suck up time which you could be using to do good or evil, etc etc.  Likewise, try thinking about how your phone, fridge, alarm clock, or kettle might affect the world in morally-relevant ways: I bet you could find some.  Even boring old non-electrical objects, like pencils and cups and even rocks, are not without *some* ethical impact. (Ever had a stone thrown at you? You'd then have a pretty strong opinion on the ethical impacts of stones.)

A lot of physical objects, particularly appliances/devices, can even be considered *implicit* ethical agents.  Engineers who are designing things generally have to think about safety and incorporate it into their designs, at least because nobody likes to be sued.  Cars have seatbelts and airbags, pill bottles have 'child-proof' caps, and coffee cups have visible warnings that coffee may be hot.

Right now, not a lot of objects can really be considered *explicit* ethical agents, if any can at all.  Because explicit ethical agents have to be able to do some sort of reasoning, really it's only AI systems that qualify.  Further, since it's an area of active research, whether any AI systems actually *are* explicit ethical agents is open to debate (lots of researchers will tell you that their system qualifies, but other contenders don't). 

Nevertheless, as we keep developing AI algorithms for ethical reasoning, the possibility opens up that we can install these systems in more and more places.  Currently we're mostly thinking about robots and software bots - places where AI is already on the table.  It's certainly not impossible, however, to put ethical AI algorithms into TVs, fridges, kettles, and so forth.

## The toaster of your dreams (or nightmares?)

What might that look like in practice? Consider the humble toaster.  Mine has a pretty simple set of features: two slots for items-to-be-toasted, a lever you push down to begin toasting (which pops up, along with the toast, when it's done), and a little dial to adjust just how toasted you want your item.  Nothing fancy.  A quick web search indicates that modern toasters have a few more features - LED screens that indicate toast progress, as well as safety features to ensure that the toaster shuts down if it detects burning (implicit ethical agent, anyone?).  The LED screens imply that some toasters might have microchips in them, and these, combined with sensors, could allow the toast to do fancy things like checking on toast temperature while dethawing.  That is, there's probably at least some computer power in at least some toasters already.

But we're just getting warmed up (pun intended).  Let's suppose that your toaster had a few extra sensors and a little more computer power.  Maybe the toaster could detect exactly what was being toasted in it, and estimate its nutritional value and calorie count.  It could forward this information to a health app on your phone, helping you keep better track of your diet.  Maybe that health app could then warn you that maybe you shouldn't eat that fourth Pop-Tart&reg;.  More radically, maybe your toaster (or the health app) could determine that it shouldn't toast that junk for you at all, and could simply [refuse to do so](https://gifrific.com/ronald-mcdonald-food-slap/).

Probably all this nutritional data is also going to the toaster company, who are thinking of selling it to advertisers so that they can better target ads to you as toaster-user.  Arguably the fact that this is happening at all is problematic, but let's make the (maybe unreasonable) assumption that it's sometimes okay.  There are nevertheless places where that data shouldn't be allowed to go (maybe the Kellogg's corporation, because you definitely *don't* need them to sell you any more Pop-Tarts&reg;, thank you very much; or maybe the political campaign of the *fascist du jour*).  It might not be that far-fetched for the toaster to use its computer power to reason about the sorts of data it should/shouldn't share, or at least to send that information to some other computer that *does* reason about that rather than just passing it off willy-nilly to advertisers.

Maybe the toaster should also have algorithms that help it optimize power consumption to minimize its environmental impact.  This might be easily handled implicitly (as they currently are in most systems with "Power saver" modes), but it's not inconceivable that the toaster might explicitly reason about how it can minimize its environmental impact. The point is that there are a lot of directions we can take this simple toaster if we give it a few more capabilities (a microchip, a few sensors, maybe an internet connection), and the toaster can, in its own small way, work to make the world a better place.

## An Internet of Ethical Things

In our toaster example, many of the capabilities that I've discussed only need *domain-specific* capabilities: the toaster can have specific algorithms related to its environmental impact and its user's diet and privacy.  Nevertheless, if we really want our toaster to do all these things (more on that later), maybe giving it general ethical algorithms isn't such a bad idea!

The second point made from the toaster example is that it *doesn't need to be the toaster itself that does the reasoning*.  In AI, for something to qualify as an agent, it needs to have *sensors* (things it uses to perceive the world) and *actuators* (things that it can use to make a difference in the world).  A toaster has both:
* My toaster can "sense" whether the bread lever is down, how much it's supposed to toast it, and (presumably) how much time remains.  The hypothetical toaster might also have temperature sensors and maybe even little cameras or composition sensors that can detect what's being toasted.
* The most important actuators for a toaster are the heaters (as well as the bread lever and trays, which are "popped up" when complete), but there may be others (such as the LED screen on which it can display things).

It's probably excessive to give a toaster general-purpose ethical reasoning capabilities - after all, these will probably require a lot of CPU power and memory, which would probably not be economical.  If the toaster instead has connections to a network, then these calculations can be performed on some other computer and sent back to the toaster.  This raises the possibility that a single ethical agent (the computer program) could read information from and act using *many* devices, and thus take much more information into account when doing ethical reasoning.  The health app I mentioned is sort of an example of this: presumably it's using info from the toaster as well as maybe other appliances, your FitBit, etc., to help you better manage your health.

We could think of this as an "[Internet of Ethical Things](https://en.wikipedia.org/wiki/Internet_of_things)", a *distributed* intelligent agent (one that exists across multiple devices) that receives sensory information from, and can control the actuators of, a whole bunch of different devices, and which has general-purpose ethical reasoning capabilities.  It exists to always do the "right thing" (to make the world a better place/to obey universal rules/to contribute to "the good life"), and is constantly "thinking" about how it can use the physical objects at its disposal to do so.

Some people are interested in having "smart homes" which automate your house to fulfill your preferences with the push of a button.  This idea could function like that, with individuals having "ethically smart homes" that can reason in sophisticated ways about how to do the right thing.  The obvious extreme (both infeasible and probably undesireable) would be one agent that controls all such objects across the world, balancing the good of all people who interact with its devices.  Probably not a good idea to give a single agent that much power, no matter how ethical it purports to be.

To the point van Wynsberghe and Robbins are trying to make about the absurdity of appliances and simple robots having morality: I don't think it's that absurd.  Sure, it's an extreme position, but I don't think it's inconceivable that an engineer might feel that because the capabilities are beginning to become available, it's their obligation to try to make the world a better place by converting as many objects as possible into explicit ethical agents (or into parts of a larger distributed ethical agent).

To be fair to van Wynsberghe and Robbins, I want to point out that I might be dead wrong about what they mean by "untenable".  If they mean that making all objects into AMAs would be "infeasible" or "impractical", then I agree (more on that below).  If they mean that there are reasons we should not go all the way in that direction, again I agree, though I'm not convinced those reasons are insurmountable (again, more below).  It's also worth questioning what they mean by the word "must"- if they mean that we should be killing ourselves trying to make every little thing an AMA no matter the cost, then I agree that that's silly.  But if they mean by "must" that we have a moral obligation to make agents into AMAs that should be considered alongside other obligations and concerns, and which is stronger for agents that have more impact on the world (e.g., robots), then I don't think that's untenable (though I'm still agnostic on whether it's *true*).  The world might just be a better place with moral toasters in it.

## Yeah, maybe not...

Let's be clear: I am not advocating that we go full speed ahead on this "Internet of Ethical Things" idea.  I can't say I'm fully decided yet on whether the "Internet of Ethical Things" or the explicit moralization of physical objects is a good idea - again, I'm primarily arguing that it's not incoherent or absurd.  There are a lot of legitimate reasons why it might be misguided.  Here are a few:

1. Certainly converting *all*, or even *most*, objects into explicit ethical agents is overkill.  It'd take a lot of time, money, and environmental resources to give all these things ethical reasoning abilities, and those resources would very likely do more good elsewhere.  This is why even people who might want as many objects as possible to have ethical reasoning capabilities will probably focus most of their attention on robots, which tend to have more powerful actuators, and also will likely be used in social situations making general-purpose reasoning more important.

2. Security would be a *huge* issue.  Current Internet of Things (IoT) technologies (those appliances, etc that are already connected to the internet) tend to be notoriously insecure, allowing hackers to manipulate them in all sorts of terrifying ways.  Putting more objects on the network in order to leverage ethical reasoning capabilities could make the problem much, much worse.

3. People have argued that giving robots and other physical objects ethical reasoning capabilities could undermine humans' moral agency ([Verbeek, 2011](https://books.google.com/books?hl=en&lr=&id=Falkge0XaxoC)) or lead to a moral de-skilling ([Vallor, 2015](https://doi.org/10.1007/s13347-014-0156-9)).  When our objects prevent us from doing anything other than the right thing, where is our freedom? Can we truly live a good life when we're forced to be ethical?  What if we lose our ability to make ethical choices for ourselves?  This is a valid concern, but I'd argue that it underestimates the ethical reasoning ability of future agents.  If the freedom to choose right or wrong is really an important ethical concern (I'd argue that it is), then explicit ethical agents ought to take it into account in decision-making.  This doesn't completely answer all the questions (how should ethical agents weigh human moral freedom relative to other concerns?  Wouldn't it be a waste to give your toaster moral reasoning if it ultimately just decides never to intervene or share data?), but it's a start.

4. Ultimately, the brick wall we run into when creating ethical algorithms is: whose ethics/morality?  We certainly don't know of a universally-agreed-upon set of general moral rules or principles that we can put on a robot uncontroversially.  People can mostly get along when it comes to basic safety concerns, but once we start getting into moral dilemmas and larger-scale questions, it's not clear just whose ethics should count.  The user's? The designer's? Both seem problematic.  One simple step towards a solution is proposed by Verbeek (2011) who proposes that designers employ democratic processes, including anyone who could be affected by a technology to hammer down which moral principles should be employed.  This may get us somewhere, but we're not all the way there (what do we do about *learning* moral norms?  How do we make sure everyone's input matters in this case?).

While I disagree with a lot of the arguments van Wynsberghe and Robbins make, I *do* agree with their proposal: a moratorium on commercialization of robots (and distributed ethical agents, etc) claiming to have ethical capabilities.  AI ethics is an ongoing area of research, and likely to remain that way for a while.  We haven't solved all the problems yet (I don't know if we have even completely solved *any* of the problems yet, or even if we know what all the problems are yet), and it would be irresponsible for any product to hit the market claiming that it has.  While I believe that we should absolutely keep researching and striving for ethical AI, we shouldn't fool people into thinking it'll be here anytime soon.  In the meantime, we should keep having these sorts of conversations and involve as many people as possible in the process of figuring out what ethical AI should look like.

Thanks for getting all the way through my silly ramblings!  Kudos to you! You deserve a Pop-Tart&reg; (if that's what you like, and your toaster will let you have it).

<textarea id="bibtex_input" style="display:none;">
@article{vanwynsberghe,
title={Critiquing the Reasons for Making Artificial Intelligence},
author={van Wynsberghe, Aimee and Robbins, Scott},
year={2018},
journal={Science and Engineering Ethics},
url={https://link.springer.com/article/10.1007/s11948-018-0030-8}
}

@Inbook{Scheutz2016,
author="Scheutz, Matthias",
editor="M{\"u}ller, Vincent C.",
title="The Need for Moral Competency in Autonomous Agent Architectures",
bookTitle="Fundamental Issues of Artificial Intelligence",
year="2016",
publisher="Springer International Publishing",
address="Cham",
pages="517--527",
abstract="Autonomous robots will have to have the capability to make decisions on their own to varying degrees. In this chapter, I will make the plea for developing moral capabilities deeply integrated into the control architectures of such autonomous agents, for I shall argue that any ordinary decision-making situation from daily life can be turned into a morally charged decision-making situation.",
isbn="978-3-319-26485-1",
doi="10.1007/978-3-319-26485-1_30",
url="https://doi.org/10.1007/978-3-319-26485-1_30"
}

@Article{Vallor2015,
author="Vallor, Shannon",
title="Moral Deskilling and Upskilling in a New Machine Age: Reflections on the Ambiguous Future of Character",
journal="Philosophy {\&} Technology",
year="2015",
month="Mar",
day="01",
volume="28",
number="1",
pages="107--124",
abstract="This paper explores the ambiguous impact of new information and communications technologies (ICTs) on the cultivation of moral skills in human beings. Just as twentieth century advances in machine automation resulted in the economic devaluation of practical knowledge and skillsets historically cultivated by machinists, artisans, and other highly trained workers (Braverman 1974), while also driving the cultivation of new skills in a variety of engineering and white collar occupations, ICTs are also recognized as potential causes of a complex pattern of economic deskilling, reskilling, and upskilling. In this paper, I adapt the conceptual apparatus of sociological debates over economic deskilling to illuminate a different potential for technological deskilling/upskilling, namely the ability of ICTs to contribute to the moral deskilling of human users, a potential that exists alongside rich but currently underrealized possibilities for moral reskilling and/or upskilling. I flesh out this general hypothesis by means of examples involving automated weapons technology, new media practices, and social robotics. I conclude that since moral skills are essential prerequisites for the effective development of practical wisdom and virtuous character, and since market and cultural forces are not presently aligned to bring about the more salutary of the ambiguous potentials presented here, the future shape of these developments warrants our close attention---and perhaps active intervention.",
issn="2210-5441",
doi="10.1007/s13347-014-0156-9",
url="https://doi.org/10.1007/s13347-014-0156-9"
}

@book{verbeek2011moralizing,
  title={Moralizing technology: Understanding and designing the morality of things},
  author={Verbeek, Peter-Paul},
  year={2011},
  publisher={University of Chicago Press},
  url={https://books.google.com/books?hl=en&lr=&id=Falkge0XaxoC}
}

@article{moor2006nature,
  title={The nature, importance, and difficulty of machine ethics},
  author={Moor, James H},
  journal={IEEE intelligent systems},
  volume={21},
  number={4},
  pages={18--21},
  year={2006},
  publisher={IEEE},
  url={http://ieeexplore.ieee.org/abstract/document/1667948/}
}

@INPROCEEDINGS {aaai18,
  author="Kasenberg, Daniel and Scheutz, Matthias",
  title="Norm Conflict Resolution in Stochastic Domains",
  booktitle="Proceedings of the Thirty-Second AAAI Conference on Artificial Intelligence",
  year="2018",
  url="https://hrilab.tufts.edu/publications/kasenbergscheutz18aaai.pdf"
}
</textarea>

## References
<div id="bibtex_display" class="bottomspace"></div>