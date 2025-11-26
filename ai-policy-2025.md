# Artificial Intelligence (AI) Policy for the AQUA Research Group, Quantum Information Processing, and Quantum Internet (Fall 2025)
Rod Van Meter, incorporating and adapting suggested text on rules and examples from Andrew Todd (though I take responsibility for the current draft; Andrew has not endorsed this yet)

[**"AI is a tool to delegate tasks, not understanding"**](https://datatracker.ietf.org/meeting/124/materials/slides-124-rasprg-02-jaime-jimenez-01) Jaime Jiménez, RASPRG at IETF 124, Nov. 2025

This is a set of guidelines for [my research group](https://aqua.sfc.wide.ad.jp/) and the classes I am teaching at [Keio's Shonan Fujisawa Campus](https://www.sfc.keio.ac.jp/). These guidelines supplement the ITC [Guideline for Generative AI Usage at Keio University](https://www.itc.keio.ac.jp/en/software_ai_guideline.html).

First, even before we begin, it is important to note that AI is everywhere, and that everyone is already using it all the time.  Speech recognition, voice synthesis, chess-playing programs, image recognition systems, even route planning for your road trip are all, technically, artificial intelligence. This document is not intended to be a blanket prohibition on its use (otherwise this would be a very short document), although there are plenty of academics [arguing in favor of this position](https://zenodo.org/records/17065099).

Artificial intelligence (AI), in its current instantiation, warrants a great deal of caution as AI achieves widespread use.  It is perhaps the most transformative information technology of our generation, in terms of the impact on society and how humans go about their daily lives, likely even moreso than our own research area of quantum computing and communications. Let me spend some time explaining my opinion and how I arrived at it before laying down some actionable rules.  I hope this will help group members and students to not only understand _what_ to do and not do, but also _why_, and to develop their own mental framework that will stand them in good stead for some time to come.

I am definitely not an anti-technologist (as evidenced by my career choices), but that doesn't mean I always instantly and unquestioningly accept every new thing that comes down the highway.  (In fact, I'm often kind of slow to adopt new technology into my daily workflow.)  As I have gotten older (and more experienced, if not actually wiser), I have come to see that technology is not always an automatic good for society.  (This is one of the driving reasons for the creation of the [Keio Cyber Civilization Research Center](https://www.ccrc.keio.ac.jp/).)

## Prologue: My Own Thoughts and a Little History

I have been reading science fiction for about half a century now, starting with all of the Isaac Asimov I could get my hands on, which involved a lot of stories about robots (i.e., embodied AI).  (Mild spoiler alerts, if you care about such things for half-century old stories.)  Many of those stories worked from the assumption that robots and AI would be beneficial, and simply tried to work out quirks of the technology and the logic robots would follow (notably Asimov's [Three Laws of Robotics](https://en.wikipedia.org/wiki/Three_Laws_of_Robotics)), though the distaste of the human protagonist for his robot partner in the R. Daneel Olivaw novels left an impression on me.  A little more disturbing is Jack Williamson's "With Folded Hands", in which robots "protect" humans from doing almost anything interesting in the name of protecting them from harm.  Following that thread to a different logical conclusion, in the 1980s Asimov retconned a connection between his not-so-far-future robot stories and his Foundation space opera universe (which had no robots), via the interesting plot device of robots collectively deciding that the best thing for Humanity would be for Robots to withdraw from society altogether.  Meantime, in New Wave stories such as Harlan Ellison's "I Have No Mouth and I Must Scream" (which was definitely intended to shock and probably doesn't hold up well today) and others, we got a far more apocalyptic version of what can go wrong with AI.  The New Wave was, of course, followed by cyberpunk, in which AI and ubiquitous technology almost always have far more complicated, ambiguous effects on society.  So pretty much every possible future has been sketched out, from AI becoming the God of Genesis to apocalyptic extermination of humanity, and I have read a lot of it.  I even recently reread _Frankenstein_, which unless you have read it is definitely not what you think it is.  It really should be required reading for everyone in technology -- or even, just everyone.  And for that matter, one of the concerns is that we lose not only our own skills, but even our ability to understand the systems we ourselves built; in H.G. Wells' _The Time Machine_, the Eloi were in exactly that situation.  It is even a common theme in generation starship stories such as Heinlein's ["Universe"](https://en.wikipedia.org/wiki/Orphans_of_the_Sky).

I'm not old enough to remember when computers were called "electronic brains", but I played with a version of Eliza (hand-typed from a book), and I am old enough to remember when chess-playing programs transitioned from signs of incipient intelligence to just something computers do.  Likewise, early image recognition programs (a friend of mine worked on a visual fruit sorter shortly after we gradauted from college, and a company I used to work for built a system for visual inspection of computer chips) and voice recognition systems were considered AI, albeit with limited success.  A couple of friends and I even played with neural networks in a class project back in 1986, when taking Richard Feynman's class "Potentialities and Limitations of Computing Machines".  (Feynman, Carver Mead and John Hopfield co-taught an earlier version of that class.  The chain reaction radiation off of those three in one place probably changed the DNA of the students.)  In those days, neural nets were at best toys, but a lot of energy was invested in expert systems and rule-based, structured knowledge bases like Cyc.  In later years, even the techniques used in unstructured web search were based on techniques from what is called GOFAI, good, old-fashioned artificial intelligence.  And yet, somehow, all of that failed to prepare us for the impact of deep learning-based systems.

In the last few years, I have also spent a fair amount of time reading modern AI-relevant and tech society-relevant nonfiction books such as Bostrom's _Superintelligence_ (which should be read with a grain of salt, but lays out an interesting framework in its early chapters), Olson's _Supremacy: AI, ChatGPT, and the Race that will Change the World_, Ford's _Machines of Loving Grace_, Russell's _Human Compatible_, Mitchell's _Artificial Intelligence: A Guide for Thinking Humans_, the compilation of short essays titled _What to Think about Machines that Think_, and even Kissinger and Schmidt's _Genesis_ (a book I highly disrecommend as derivative and not insightful, even leaving aside my opinion of the men) and some that are only peripherally about AI, such as Becker's _More Everything_, Zakaria's _Age of Revolutions_ (which gets a lot of the history of tech wrong), and Epstein's _Tech Agnostic_.  I also read some very early criticism of whether or not AI would ever really work, _What Computers Still Can't Do: A Critique of Artificial Reason_, by Hubert L. Dreyfus.  Out of all of these books, the single most important one I have read is Merchant's _Blood in the Machine_.

So, I have spent fifty years reading about and thinking about a future (or a Now), both positive and negative, in which AI arrives.  And yet, somehow, it isn't playing out the way I expected, which I suppose was inevitable.  It's also worth pointing out that despite this half century of exposure to the issues, it's also inevitable that I am behind the leading edge in this field, and also that everything is evolving rapidly.  As Dave Farber likes to point out, the principles may stay the same, but the technology, business and societal environments change, so the right answer can also change.

## What is AI?

With all of that prologue, let's look at the state of "AI", and its plusses and minuses.

Fundamentally, a current-generation AI (i.e., LLM) doesn't find a _true_ answer, it synthesizes something that _looks plausible_.  That is its only metric.  A while back, I asked one for a biography of me, and it didn't even get my universities right, although it did report some plausible-looking results.  Current LLMs have no notion of true or false, just plausible or not-plausible as words.

Researchers are, of course, working on improving AIs, including the lab and company (companies?) of Fei-Fei Li at Stanford; a quick search will turn up lots of things, some of them [recent](https://www.forbes.com/sites/geekgirlrising/2025/11/20/fei-fei-li-ushers-in-ais-next-frontier-spatial-intelligence/) about their work in what she calls "spatial intelligence".  Spatial intelligence will require a certain level of ground truth.

(Needs to differentiate among key types of AIs, especially LLMs and generative AIs versus basic image classifiers.)

## The Plusses

There are some obvious reasons that AI is attracting a lot of positive attention.

1. Sometimes, it does a pretty good job of synthesizing a summary of a set of documents or other work.
1. It can help you sketch out code more quickly.
1. Sometimes, when doing either of the above, it brings a new perspective or piece of information you didn't know about or hadn't thought of.
1. Its written English is usually clear and grammatically correct (although with a bland personality unless you instruct it otherwise, and a synthetic one that isn't you in any case).
1. It can turn quickly-written phrases or bullet points into more fleshed-out descriptions (if not always exactly what you wanted).
1. It can bring structure to an otherwise unstructured set of data fairly quickly; note the failure of [Cyc](https://en.wikipedia.org/wiki/Cyc) to organize all of human knowledge.
1. All of us (including me) use online translation tools; the quality of those is increasing rapidly, thanks to LLMs.  (If you are reading this in Japanese or another language, it was probably translated using an LLM, either explicitly or implicitly.)

## Concerns

There are downsides to the use of AI from multiple points of view: the pragmatic concerns for both the user and the instructor, the problems as a researcher and as a manager, and the moral and ethical issues.  We will address those in this section.

### Moral and Ethical Issues

Let's begin with the moral and ethical issues, because they affect as all as individuals and as a society, and therefore underlie all of the other roles discussed below.

1. Excessive consumption of energy.
2. Distortion of semiconductor market https://www.bloomberg.com/news/articles/2025-10-09/why-experts-are-warning-the-ai-boom-could-be-a-bubble
3. Theft of intellectual property (and loss of revenue). https://www.cbc.ca/news/business/anthropic-ai-copyright-settlement-1.7626707 https://futurism.com/artificial-intelligence/openai-danger-authors-internal-slack-messages
4. Undocumented bias (e.g., against Black people when evaluating creditworthiness; Musk's current efforts to get Grok to reflect his own personal political bias)
5. Are we as a society ready to put many people ([including artists](https://www.linkedin.com/posts/amandagautierillustration_ai-is-everywhere-in-general-as-many-other-activity-7399031648539021312-WkJO/), who often already have a marginal economic life) out of work? 
6. Possible suicide ideation and encouragement. https://arstechnica.com/ai/2025/10/openai-data-suggests-1-million-users-discuss-suicide-with-chatgpt-weekly/ https://apnews.com/article/openai-chatgpt-lawsuit-suicide-56e63e5538602ea39116f1904bf7cdc3# https://edition.cnn.com/2025/11/06/us/openai-chatgpt-suicide-lawsuit-invs-vis
7. It may also produce inaccurate renderings and information when such things matter, [like in a medical setting](https://www.linkedin.com/posts/amandagautierillustration_ai-is-everywhere-in-general-as-many-other-activity-7399031648539021312-WkJO/).


On the theft of IP, are you willing to be on _either_ end of that?

[MechaHitler](https://www.npr.org/2025/07/09/nx-s1-5462609/grok-elon-musk-antisemitic-racist-content) may be the garish end point of LLM bias, but _every_ system will have some bias.

### Concerns You Should Have as a Learner

The pragramatic concerns from the user's side, either as a learner:

1. The harder the question, the wronger the answer.
2. Learning & retention are (seem to be?) impaired.
3. Inappropriate dependency develops.
4. It's never (at least currently) localized.
5. It can't read your mind.
6. It can't do math.
7. All AI-generated answers sound the same.
8. There are reports of excessive use of AI exacerbating mental health problems.

Let's look at those in a little more detail.

(1.) **The harder the question, the wronger the answer:** this seems to be inherent in the way public AIs are trained.  They are trained on publicly available data on the Internet, but for hard questions there is a lot of bad information out there.  So, the AIs are learning the wrong things, which they will then teach you.  (This may change as AIs are trained on more carefully curated datasets, but IMO getting them better grounded in reality will require some new innovations.)

Similarly, as you know, present-day systems have a tendency to "hallucinate" (translation: make up wrong answers).  Researchers are working hard to eliminate this, but it won't fully solve the above problems.

(2.) **Learning & retention are (seem to be?) impaired:** When you ask an AI to do something _for_ you, then you don't develop the skills. You also don't remember what you learn.  Having an AI do the work for you is no better than having a friend do it for you.

(3.) **Inappropriate dependency develops:** "I couldn't do my homework, ChatGPT was down!" 'Nuff said.

(4.) **It's never (at least currently) localized:** Many of the tasks we do either in class or as homework involve local information such as e.g. the names of machines we use, which the AI doesn't know.

(5.) **It can't read your mind:** When you ask it to create an outline or a summary of something, or to extend or refine something you are creating, it usually doesn't do what _you_ would do if you did the work yourself, and so your own ideas and opinions get lost.

(6.) **It can't do math:** again, it doesn't generate something true, just something plausible.  There was a lot of humor as early image generation programs created images of people with six fingers and worse, but the problem extended to basic abstract mathematics, as well.  This is one that is being "solved" by special-casing the systems to recognize mathematics questions and send them to a separate engine.  But even as the AIs themselves learn to do math, this will get better, but having an AI do basic math for you will cost millions or maybe billions of times as much energy as a well-tuned program for the specific purpose.  (More on that below.)

(7.) **All AI-generated answers sound the same:** If you're writing an essay or other original material, don't you want it to stand out?  Faculty friends of mine who spend more time with written essays say that all of the essays they receive that are written by or with the help of an AI sound the same.

(8.) **There are reports of excessive use of AI exacerbating mental health problems:** This issue is more of a concern for personal use rather than professional/academic use, but it's worth noting here anyway.  There are reports of mental health issues being exacerbated, including all the way up to chatbots encouraging people to commit suicide.  This issue should not be taken lightly.

For these reasons, you as a user or student should be very cautious about whether the answers you are getting are right, and whether or not you are learning what you need to learn (and are expected to learn).

### Concerns I Have as an Instructor

The pragmatic concerns from the instructor's side:

1. It's hard to evaluate where you are developmentally.
2. It results in unfair _appearance_ of development by those who are using AI v. those who aren't.

The basic assumption in evaluating written work by students is that the work _was done by the student_.  This means we faculty have to reevaluate how we assess student development.

_Of course_ it's okay to use new tools for learning, and if that means that you learn faster or better, that's great! Then everyone should adopt it. However, if it's financially burdensome, then it becomes just another way in which economically privileged students have an advantage over others, which is a concern for us as a university, where we aim to provide the best education for all of our students.

### Concerns We Should All Have as Researchers

As a researcher:

1. Plagiarism.
1. Improper/incorrect text (including citations).
1. Leaking or outright theft of your ideas/data.

**Plagiarism is a very big deal**.  I believe that LLMs are copying substantial blocks of text from other research papers and websites when used in writing research papers, _even when told not to_.  If you submit a research paper that is found to have plagiarized others, whether or not you wrote the offending sections directly, it can have dire consequences for you and even for the university.  Worst case, we could be forced to return research funds to the funding agency and be banned from receiving more, and be banned from submitting papers to a specific journal.  _You are ultimately responsible for what goes out with your name on it._

**Incorrect research.**  Note that this includes [hallucinated citations](https://www.cjr.org/tow_center/we-compared-eight-ai-search-engines-theyre-all-bad-at-citing-news.php)

**Leakage of your original work.** "White hat" hackers have shown that it is possible to [convince a chatbot to reveal data](https://news.uoguelph.ca/2025/08/ai-chatbots-are-giving-away-your-companys-data/) that it has learned through what is supposed a secret conversation.  I haven't checked, but I'm sure that the AI companies' user agreements promise that they won't share your secret info, but confirming this is harder than for ordinary classical systems.

Microsoft has also [recently found](https://www.microsoft.com/en-us/security/blog/2025/11/07/whisper-leak-a-novel-side-channel-cyberattack-on-remote-language-models/) that there are additional side channel attacks, but that seems inevitable; ordinary non-AI systems also have vulnerabilities found on a regular basis.

### Concerns for Managers/Businesspeople

As a manager/businessperson:

1. As of today, one estimate has found that 95% of AI projects result in no benefit to the company.
2. Code developed in large part by AIs is resulting in a lot of "technical debt", especially unanticipated security issues.
3. Loss of control: dependence on tools over which you have limited control.

There have been anecdotal reports, for example, that major companies have forced their employees to use AIs, but the employees are finding them less than helpful.  This situation could change, if the developers can gain feedback that helps them make the AIs better.

The last point represents a serious business risk. What happens when your provider changes the AI in ways that affect output you depend on, or worse, they go out of business?  Can you tolerate that?




## Rules and Recommendations

So in light of the above, what kind of specific policy rules can we put in place?

### Principles

First, this policy recognizes that AI tools can be very helpful. This policy does not forbid the use of AI.
society cannot function without mutual respect for others. 

Misrepresenting AI-generated work as your own demonstrates:

* A lack of respect for yourself: you are not allowing yourself to learn effectively.
* A lack of respect for other students: you are making it difficult to understand what students are actually accomplishing, and how they are struggling.
* A lack of respect for your teachers: your teachers want to understand your challenges and help you develop as a person; they do not want to be fed work generated by an AI.

### Recommendations for All Humans

(Here, I can't really say _rules_; whether you apply these is really up to you.)

1. _Think_.  Be mindful of how you use AI.
1. Read _a lot_ -- news, contemporary nonfiction books, SF.
1. Do not share your personal or private information with an AI.
1. Do not use an AI as a counselor or therapist.
1. Look for classical solutions when the problem is important.

### Recommendations for Instructors & Mentors

One of my most valued colleagues says, paraphrasing, "Just like the Internet thirty years ago, AI is the next generation of tool. We really should give students the experience of using it and working with it; that will make them more valuable on the job market."

https://zenodo.org/records/17065099

### Rules for Learners

1. Disclose _all_ use of AI, in detail.
2. Do not submit anything directly created by an LLM.  Your submissions are to be _your work_.

### Rules for Researchers

1. Disclose _all_ use of AI, in detail.
2. Do not submit anything created by an AI.  Your submissions are to be _your work_.

## Examples

### Making a presentation for AQUA

Situation: You are asked to summarize a new academic paper for the weekly AQUA meeting.

#### Best

You read the paper, create slides, and write a script for your presentation. If you re-use diagrams or text from the original paper, you make sure to give credit to the original authors. You use the paper's citations and Google Scholar to find related work.

You ask other students or faculty members to review your work, or if you have questions.

You ask ChatGPT to look over your slides and script, asking for advice.

In your slides, you thank the students and faculty members who gave you advice, and explain how you used ChatGPT.

You are able to answer some of the questions you are asked after the presentation.

#### Good

You read the paper, and use ChatGPT to help translate parts you don't understand into Japanese. You ask ChatGPT for help finding related work.

You want to make the presentation in English. However, you are not confident in your English abilities, so you write the slides and script in Japanese and ask ChatGPT to help you transform them in to English. You read the output several times and make adjustments.

If you re-use diagrams or text from the original paper, you make sure to give credit to the original authors. In your slides, you explain how you used ChatGPT for translation and research tasks.

You are able to answer some of the questions you are asked after the presentation.

#### Unacceptable

You do not read the paper, or you read the paper but do not try to make slides and a script by yourself.

You give the paper to ChatGPT and ask it to generate a script and slides for your presentation.

During your presentation, you read the script.

After the presentation, you have difficulty answering questions.

You do not explain how you used ChatGPT.

#### Explanation

In the "best" and "good" examples, AI's strengths are used: AI might be good at correcting grammar, doing translation work, or acting as a research assistant. AI might help you do better work and improve your skills.

However, in the "unacceptable" example, you are misrepresenting AI's work as your own. Moreover, you are not using AI effectively. Rather than augmenting your abilities, it is replacing you. The "unacceptable" example could be considered academic misconduct in some circumstances.

## Consequences

Students found to violate these guidelines will be handled on a case-by-case basis. Some cases may fall under the [university academic misconduct policies](https://www.students.keio.ac.jp/en/sfc/pmei/class/fraud/).

## Caveats and Concluding Remarks

As noted at the beginning, I personally am being a little slow to work with the AIs/LLMs, so my opinion is not as fully informed as it could be.  Moreover, _my opinion will likely change as the technology changes and my understanding grows_.  But this is my best effort as of today.

## References and Learning More

See also a couple of recommendations on my [#QuantumNative Engineer's Bookshelf](https://rdvlivefromtokyo.blogspot.com/2020/05/a-quantumnative-engineers-bookshelf.html).

### The Technology

It seems incumbent on all technologists at this point to have at least a basic grasp of deep learning, LLMs and generative AI. It is all moving insanely fast, so this list will become out of date quickly.

1. Grant Sanderson _et al._, [_Neural Networks_](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) YouTube course on the 3 Blue, 1 Brown channel. (9 videos totalling 3 hours)
1. [The moment we stopped understanding AI [AlexNet]](https://youtu.be/UZDiGooFs54?si=OLZjaqaAU0P0Itmq). (The title is misleading, it's much more about understanding how NNs learn to understand images.)
1. Andrew Ng and Kian Katanforoosh, [CS 230](https://cs230.stanford.edu/syllabus/) at Stanford. (10 video lectures, 50-90 minutes each, plus Coursera, plus substantial homework/programming assignments)


### Ethics and Society

I know this is the core of what this document is about, but this aspect is moving even faster than the technology, so this list is inevitably incomplete.  I am reading several articles _a day_ about AI and its uses and misuses in society.  Work to develop a framework rather than a long list of specific rules.

1. Nataliya Kosmyna, Eugene Hauptmann, Ye Tong Yuan, Jessica Situ, Xian-Hao Liao, Ashly Vivian Beresnitzky, Iris Braunstein, Pattie Maes, [Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an AI Assistant for Essay Writing Task](https://arxiv.org/abs/2506.08872)
1. Lucy Osler, [Hallucinating with AI: AI Psychosis as Distributed Delusions
](https://arxiv.org/abs/2508.19588)
1. [Pope Leo: AI must reflect the design of God the Creator](https://www.vaticannews.va/en/pope/news/2025-11/pope-leo-xiv-message-builders-ai-forum-ethical-technology.html) (full message [here](https://www.vatican.va/content/leo-xiv/en/messages/pont-messages/2025/documents/20251103-messaggio-builders-aiforum.html))

### Quantum Machine Learning

Given that our research group focuses in quantum computing and communications, it also seems reasonable to invest some effort in learning about quantum machine learning.

1. Francesc Rodríguez-Díaz, David Gutiérrez-Avilés, Alicia Troncoso, Francisco Martínez-Álvarez, [A Survey of Quantum Machine Learning: Foundations, Algorithms, Frameworks, Data and Applications](https://dl.acm.org/doi/10.1145/3764582)
1. Su Yeon Chang, M. Cerezo, [A Primer on Quantum Machine Learning](https://arxiv.org/abs/2511.15969)


## History

* 2025/10/20: Version 1.
* 2025/10/21: Restructure rules, all AI essays sound the same.
* 2025/11/12: Some progress on reformatting and reorganizing, but update to rules themselves still pending.
* 2025/11/26: Finally got around to bringing in Andrew's examples.
