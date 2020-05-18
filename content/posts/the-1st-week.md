---
title: "Step 1: What are we talking about?"
date: 2019-09-02T08:47:11+01:00
featured_image: card-catalogue.jpg
summary: "Today we're going to look at an overview of the course, define our terms, and start a heuristic evaluation."
---
<section class="slide-only">
    <h2>Here's what we're going today</h2>
    <ol>
        <li class="fragment">Course overview</li>
        <li class="fragment">Define our terms</li>
        <li class="fragment">
            Component of the week: &lt;img&gt;
        </li>
        <li class="fragment">Two assigments</li>
    </ol>
</section>
<section class="slide-only">
    <h2>Syllabus</h2>
    <a href="/files/http5301-accessibility-and-usability-syllabus.pdf" target="_blank" class="button primary">Let's take a look at the syllabus →</a>
</section>
<section class="post-only">
    <h2>Resources</h2>
    <hr>
    <a class="button primary" href="/files/http5301-accessibility-and-usability-syllabus.pdf" target="_blank">Download the syllabus</a>
    <hr>
</section>
<section>
    <h2>This course (in chart form)</h2>
    <table style="font-size:1.1rem">
    <tr>
        <th><small>Week&nbsp;#</small></th>
        <th>Topic</th>
        <th>Task</th>
        <th>Due</th>
    </tr>
    <tr>
        <td>May 19th,&nbsp;21st</td>
        <td>Definitions, Heuristics</td>
        <td>Reading 1 assigned;<br>Group project assigned.</td>
        <td></td>
    </tr>
    <tr>
        <td>May 26th,&nbsp;28th</td>
        <td>Collecting data</td>
        <td>Brief assigned.</td>
        <td>Reading 1 (2.5%)</td>
    </tr>
    <tr>
        <td>June 2nd,&nbsp;4th</td>
        <td>Analyzing & reporting</td>
        <td>Report assigned.</td>
        <td>Group&nbsp;project&nbsp;(30%)</td>
    </tr>
    <tr>
        <td>June 9th,&nbsp;11th</td>
        <td>The DOM and assistive devices</td>
        <td></td>
        <td>Brief (25%)</td>
    </tr>
    <tr>
        <td>June 16th,&nbsp;18th</td>
        <td>Content & inputs</td>
        <td>Reading 2 assigned.</td>
        <td></td>
    </tr>
    <tr>
        <td>June 23rd,&nbsp;25th</td>
        <td>Navigation</td>
        <td></td>
        <td>Reading 2 (2.5%)</td>
    </tr>
    <tr>
        <td>June&nbsp;30th,&nbsp;July&nbsp;2nd</td>
        <td>Presentations</td>
        <td></td>
        <td>Report (40%)</td>
    </tr></table>
</section>
<section>
    <h2>This course (in detail)</h2>
    <hr>
    <h3>What are we learning about?</h3>
    <p>This course is about usability (which includes accessibility).</p>
    <p>Usability is <strong>how useful something is</strong>. In order to find out how useful something is, we need to:
        <ul>
            <li>figure out who's going to use it,</li>
            <li>get data about how well it works for them,</li>
            <li>interpret that data based on our expert knowledge of how things are made more useful, and</li>
            <li>make recommendations about how to improve the thing.</li>
        </ul> 
    </p>
</section>
<section>
    <h3>Why does it matter?</h3>
    <p>As with most of what you're learning in this program, it matters because <strong>it will make you good at making things</strong>. In most of your courses, you learn how to make things. In this course, you will learn how to make things <strong>for real people, better.</strong></p>
    <img class="post-only" src="/images/people.png" alt="Vectors of faces">
</section>
<section>
    <h3>How will we learn it?</h3>
</section>
<section>
    <p>In this course, we will:
        <ul>
            <li>Read materials related to usability, and reflect on them in the context of our work. <em>(These are the <strong>reading assignments</strong>.)</em></li>
            <li>Work in a team of 4-5 with fellow experts to evaluate a website based on an industry-standard checklist (a.k.a. a 'heuristic evaluation'). <em>(This is your <strong>group assignment</strong>.)</em></li>
            <li>Design a usability test for collecting good information about the website, application or component of your choice. <em>(This is <strong>the brief</strong>.)</em></li>
            <li>Carry out that test with 5 users, observing them using the website (or application, component, etc.) <em>while they are using only a screenreader or keyboard</em> (you'll pick one for all your users), and reporting to the class your findings. <em>(This is <strong>the final report/presentation</strong>.)</em></li>
        </ul>
    </p>
</section>
<section>
    <h3>In this lesson, we'll...</h3>
    <ol>
        <li class="fragment"><a href="#terms">Define general terms and concepts for both usability and accessibility.</a></li>
        <li class="fragment"><a href="#heuristicEvaluation">Learn how to perform a heuristic evaluation.</a></li>
    </ol>
</section>
<section>
    <h2>Hi! Let's talk about things.</h2>
    <figure>
        <img src="/images/women.jpg" alt="Socially distanced people talking">
        <figcaption>...from a safe distance.</figcaption>
    </figure>
    <p class="post-only">What better place to start in any discipline than knowing the jargon. It makes googling your problems so much easier! Let's jump into accessibility and usability by going over some of the common terms for the fields' general concepts.</p>
</section>

<div id="terms" class="post-only">
    <h3>Here are the terms we're going to define:</h3>
    <ol>
        <li class="fragment"><a href="#usability">Usability</a></li>
        <li class="fragment">Things that aren't Usability <ol>        <li class="fragment"><a href="#ux">UX</a></li>
        <li class="fragment"><a href="#cx">CX</a></li>
        <li class="fragment"><a href="#ui">UI</a></li>
        <li class="fragment"><a href="#hci">HCI</a></li>
        <li class="fragment"><a href="#ixd">IxD</a></li>
        <li class="fragment"><a href="#hcd">HCD</a></li></ol></li>
        <li class="fragment">Usability Tools
            <ol> 
        <li class="fragment"><a href="#heuristics">heuristics</a></li>
        <li class="fragment"><a href="#personas">personas</a></li>
        <li class="fragment"><a href="#scenarios">scenarios</a></li>
        <li class="fragment"><a href="#qualQuant">quantitative & qualitative data</a></li></ol></li>
        <li><a href="#access">Accessibility</a>
            <ol>
                <li class="fragment"><a href="#lowercase">accessibility (the idea)</a></li>
                <li class="fragment"><a href="#uppercase">Accessibility (the law)</a></li>
                <li class="fragment"><a href="#aoda">AODA</a></li>
                <li class="fragment"><a href="#wcag">WCAG</a></li>
                <li class="fragment"><a href="#wai-aria">WAI-ARIA</a></li>
            </ol>
        </li>
    </ol>
</div>
<section id="usability">
    <h2>Usability</h2>
    <blockquote><strong>Web usability</strong> The extent to which specified users can find, understand and use information and services online. Web usability can be measured through the effectiveness and efficiency with which users can complete defined tasks online.
        <footer><cite><a href="https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=24227&section=glossary" target="_blank">Government of Canada, Standard on Web Usability</a></cite></footer></blockquote>
    <p class="post-only">Let's differentiate usability from some similar (and sometimes overlapping) terms.</p>
</section>
<section>
    <p><strong>Usability</strong> is, as we said, how quantitatively useful a product is.</p>
    <p class="fragment" id="ux"><strong>User experience (UX)</strong> is how people felt about their experience of using the product. </p>
    <p class="fragment" id="cx"><strong>Customer experience (CX)</strong> is how people felt about the company that the product represents.</p>
    <p class="fragment" id="ui">The <strong>user interface (UI)</strong> is the mechanism by which the person uses the product.</p>
</section>
<section>
    <p id="hci"><strong>Human-Computer Interaction (HCI)</strong> is the study of the usability of user interface(s). It is an old (<a href="https://www.cs.cmu.edu/~amulet/papers/uihistory.tr.html" target="_blank">50+ years!<span class="show-for-sr"> Link opens in a new tab</span></a>), and primarily academic discipline that talks about cognitive science, ergonomics, and all kinds of wonderful stuff.</p>
    <p class="fragment" id="ixd"><strong>Interaction design (IxD)</strong> is the functional design of the interface, while UI design is the appearance of the interface. We're really starting to split hairs here. If you're a UI designer, this is not a "not my job" type of thing.</p>
    <p class="fragment" id="hcd"><strong>Human-centred design</strong> and <strong>user-centred design</strong> are often used interchangeably, BUT, (and, again, we're splitting hairs), human centred design is a design process that takes into consideration the end user (i.e. humanity) at each stage of design, whereas UCD takes into consideration <em>a specific audience</em>.</p>
</section>
<section>
    <figure>
        <footer>
            <img src="/images/ipod.jpg" alt="">
            <figcaption>I couldn't find an image of a Zune, so here is an iPod.</figcaption>
        </footer>
    </figure>
</section>
<section>
    <p class="post-only">So, if we were to apply these terms to, and I'm dating myself here, an iPod...</p>
        <ul>
            <li>Usability === average number of steps to listen to a song.</li>
            <li>UX === people like using the ipod.</li>
            <li>CX === people like Apple.</li>
            <li>UI is both the hardware and software<span class="post-only"> that provides the user with input or output (as opposed to, say, the internal database retrieval software, or internal hardware)</span>.</li>
            <li>HCI studies the totality of the interactions, including the charging port.</li>
            <li>IxD === how the wheel affects the display.</li>
            <li>UI design === what the wheel looks like, what font the display uses.</li>
            <li>HCD means<span class="post-only">, from the beginning of the design process,</span> someone was thinking about what it would be like to hold in your hand.</li>
            <li>UCD means<span class="post-only">, from the beginning of the design process,</span> someone was thinking about the hands of people who would spend $399 on a portable music player.</li>
        </ul>
    <p class="post-only">Okay, so now that we know what usability is (and isn't), let's talk about some terms associated with...</p>
</section>
<section>
    <h3><strong>How We Test It</strong></h3>
</section>
<section id="heuristics">
    <img class="post-only" src="/images/lightbulb.jpg" alt="This is a decorative image, which doesn't need alt text, but I'm trying to set a good example.">
    <h3>Heuristics</h3>
    <p class="post-only">For whatever reason, 'heuristic' is one of those words I have to look up every six months, I always forget the definition, probably because it's a little hard to define.</p>
    <p>An heuristic is a good-enough solution, an approximation, a rule of thumb. In usability, <strong>heuristic analysis</strong> is basically a checklist of good usability principles. You don't need to watch a live test subject to know that you need good error messages, or system feedback.</p>
</section>
<section>
    <p class="callout">Let's take a look at the most popular checklist for doing heuristic evaluations: Jakob Nielsen's <a href="https://www.nngroup.com/articles/ten-usability-heuristics/" target="_blank">10 Usability Heuristics for User Interface Design<span class="show-for-sr"> Opens in a new window</span></a></p>
    <p class="post-only">Heuristics aren't just something to test, they're rules to internalize when making things.</p><hr class="post-only"><p class="post-only">The next term, <em>personas</em>, describes a tool that is typically used when designing (and adding to) a user workflow, but also come into play during usability testing.</p>
</section>
<section id="personas">
    <h3>Personas</h3>
    <p>Personas are a tool for creating a design. A persona is <strong>a fake person you use to represent a major user group</strong> for your product.</p><p class="post-only">Let's say you're a library, and you're creating a form to get people to sign up for an online account. You would create personas based on your current users, and any group that you want to target as a user (maybe you've got an ad campaign to drive new users to the website, for example).</p>
    <p class="post-only">Based on the information you have, you might create personas for an elderly person, a parent with children, and a student. </p>
</section>
<section>
    <blockquote>
        <p>Personas generally include the following key pieces of information:</p>
        <ul>
            <li>Persona Group (i.e. web manager) </li>
            <li>Fictional name</li>
            <li>Job titles and major responsibilities</li>
            <li>Demographics such as age, education, ethnicity, and family status</li>
            <li>The goals and tasks they are trying to complete using the site</li>
            <li>Their physical, social, and technological environment</li>
            <li>A quote that sums up what matters most to the persona as it relates to your site </li>
            <li>Casual pictures representing that user group</li>
        </ul>
        <footer><cite><a href="https://www.usability.gov/how-to-and-tools/methods/personas.html" target="_blank">https://www.usability.gov/how-to-and-tools/methods/personas.html</a></cite></footer>
    </blockquote>
</section>
<section>
    <p>The purpose of making up a fake person, rather than simply pointing to your analytics data, is to <strong>facilitate design discussions</strong> (particularly with people who don't deal with analytics on the regular).</p>
    <hr>
    <p>The next term, <em>scenarios</em>, is also used during the design phase, but is a crucial element of usability testing.</p>
</section>
<section id="scenarios">
    <h3>Scenarios</h3>
    <p><span class="post-only">Now that you've got an idea of who is using your site, you can go a step further and write down WHAT they're using the site for - these are called Scenarios. </span>A Scenario is <strong>a set of tasks required to accomplish a user's goal</strong>.</p>
    <p class="post-only">Further reading: <a href="https://www.nngroup.com/articles/task-scenarios-usability-testing/" target="_blank">https://www.nngroup.com/articles/task-scenarios-usability-testing/</a></p>
    <p class="post-only"><hr>So, with your personas to guide you, you've developed a prototype application. Time to see if your fake people translate to real people - it's time for usability testing! In usability tests, you take your scenarios, and you ask people to try and accomplish the goal of that scenario. Then, you spy on them like a total creep! But it's fine because you have their consent and you're probably giving them $5 and some donuts. When you run your scenario, there are a number of ways that you can get data from the test.</p>
</section>
<section id="qualQuant">
    <h3>Qualitative and quantitative data</h3>
    <figure class="post-only"><img src="/images/data.jpg" alt="Data that doesn't mean anything. So, I guess, qualitative?"></figure>
    <p class="post-only">Before we get into methods, let's define the two categories of data that we report. Quantitative and Qualitative, aka quant and qual.</p>
    <p><strong>Quantitative data</strong> is, naturally, data you can quantify. How long does it take to complete the task? How many errors does a user generate, etc. </p>
    <p><strong>Qualitative data</strong> is observational, and, generally, subjective. Is the user struggling to find a UI element? Is there a part of the interface that they seem to enjoy fiddling with? </p>
</section>
<section>
    <p>Quantitative research requires different conditions than qual, for a few reasons. First of all, <strong>to get good quantitative data, you need a large data set</strong>. <span class="post-only">You'll be running a lot of people through a well-defined and tightly controlled task set. Qualitative data, on the other hand, is gathered in a much looser and more adaptable way. Quantitative research is less common, but provides a business with some all-important numbers.</span> <strong>Qualitative research is more subjective, as it's meant to be exploratory</strong>. Of course, when you're dealing with an organization, they'll still want numbers to supplement all your lovely written summaries and reports.</p>
</section>
<section id="qualQuant">
    <img src="https://media.nngroup.com/media/editor/2017/04/11/pure-product.png" alt="Examples of PURE evaluations." style="float:right;"><p>That's where PURE comes in - <strong>Pragmatic Usability Rating by Experts</strong>.</p><p>This is just a rubric for putting your subjective findings into, so that your hunches and intuition get turned into numbers. You <strong>split your scenario into tasks, and your tasks into steps, and give each step a score out of three</strong> for how difficult the user found the task, 1 being easy, 3 being difficult.</p>
</section>
<section>
    <p>Now, there's a whole variety of types of user tests you can do, and if you're a usability expert or UX researcher, part of your job is having your own catalog of tests and deciding which ones are appropriate. </p>
    <hr>
</section>
<section id="access">
    <h2>Accessibility</h2>
    <img src="/images/braille.jpg" alt="Well, it's braille. No idea what it says. Or how to find out, even. Not really very accessible if you ask me.">
</section>
<section id="lowercase">
    <h3>accessibility (the idea)</h3>
    <p class="post-only">Lowercase 'a'. Accessibility as a broad term means recognizing what kind of barriers people might have to using your product or service and doing what you can to remove those barriers where possible, or, if it's not possible, providing equivalent alternatives.</p>
    <p class="post-only">I want to emphasize that accessibility is not something that you should expect to 'finish'. It's not that kind of thing. It is a way of thinking, it is a set of questions you should always be asking. There are 7 billion people out there, it is not possible to make something perfectly accessible. That's not your responsibility. What <em>is</em> your responsibility, I think, is to always look for opportunities to make things better, to be humble and recognize that people might have barriers that you've never thought of, and to be open to criticism and willing to take that as an opportunity to improve. That's not an easy thing to do - to accept that the things you make will always be imperfect, and that you won't always have the resources to do right by everyone. But try your best, and, odds are, this means you are a good person.</p>
    <ul class="slide-only">
        <li class="fragment">What kind of barriers does your product or service have?</li>
        <li class="fragment">Can you remove them?</li>
        <li class="fragment">Failing that, can you provide ways around them?</li>
    </ul>
</section>
<section id="uppercase">
    <h3>Accessibility (the law)</h3>
    <p class="post-only">...with a capital 'A' takes all of the guesswork out of it. Capital A accessibility means complying with the legal guidelines set out by the goverment for making your product or service usable by people with broadly defined physical challenges. So, we often talk about visual impairments, because we're working in a primarily visual medium. Hopefully your website doesn't have a lot of audio cues, but it's common to work with video that has an audio component, so we also talk about people with hearing issues. And, of course, our products and services generally have some kind of physical interface, so we talk about mobility issues. These are the big three categories of barrier that are addressed by capital 'A' accessibility.</p>
    <ul class="slide-only">
        <li class="fragment">This is the law.</li>
        <li class="fragment">(This is also what gets you hired!)</li>
        <li class="fragment">Primarily addresses visual, hearing and mobility impairments.</li>
    </ul>
</section>
<section id="a11y">
    <h3>a11y</h3>
    <blockquote>
        <p>"a11y" is an abbreviation for "accessibility" that is more compact for the character limits on social media. The “11” in the middle stems from conventions in software engineering and Information and Communication Technology that shortens long words by substituting middle letters with the number of middle letters instead. There are 11 letters between the "a" and the "y," so accessibility becomes a11y. For another example, “l10n” refers to "localization," because 10 letters come between the “l” and the “n.”</p>
        <p>Coincidentally, a11y looks like it would read phonetically as <em>ally</em>... Many technologists see a11y as a movement, and not just the simple act of making websites more accessible.</p>
        <footer><cite><a href="https://www.boia.org/blog/what-is-a11y">Bureau of Internet Accessibility - What is a11y?</a></cite></footer>
    </blockquote>
</section>
<section id="aoda">
    <h3>AODA</h3>
    <p>These guidelines are codified in the <a target="_blank" href="https://www.ontario.ca/laws/regulation/110191#BK14">AODA (Access for Ontarians with Disabilities Act)<span class="show-for-sr"> Link opens in a new tab</span></a> specs.</p>
    <blockquote>
        (4) Designated public sector organizations and large organizations for their internet websites shall meet the requirements of this section <br><br>2. By January 1, 2021, all internet websites and web content must conform with WCAG 2.0 Level AA, other than, <br><br>i. success criteria 1.2.4 Captions (Live), and <br><br>ii. success criteria 1.2.5 Audio Descriptions (Pre-recorded). O. Reg. 191/11, s. 14 (4).</blockquote>
</section>
<section id="wcag">
    <h3>WCAG</h3>
    <p>Which brings us to WCAG - Web Content Accessibility Guidelines. These are the recommendations written by the World Wide Web Consortium, which is the organization that creates standards around things like HTML and CSS. The vast majority of capital A accessibility regulations (like the AODA) defer to these specifications and the different tiers (levels).</p>
</section>
<section id="wai-aria">
    <h3>WAI-ARIA</h3>
    <p>is also produced by the W3C. It is a set of specifications for techniques to make dynamic content accessible (which helps it <a href="https://www.w3.org/TR/WCAG20-TECHS/aria" target="_blank">comply with the WCAG</a>). It's pretty simple - it's essentially just a specification for a set of attributes in your markup language. The purpose is to fill in a visibility gap created when a scripting language turns static markup into dynamic content. </p>
</section>
<section>
    <h3>That's all the definitions!</h3>
    <p>Now for the fun stuff.</p>
</section>
<section>
    <h2>Component of the week</h2>
    <p class="post-only">The first half of this course is mostly going to be looking at usability testing and best practices, with the second half focussed more on accessibility best practices. But I didn't want to save all the good stuff for last, so each week we'll look at how to make one component or design pattern fully accessible.</p>
    <p>This week, we turn our spotlight on the <code>&lt;img&gt;</code> element!</p>
</section>
<section>
    <p>Our story <a href="https://thehistoryoftheweb.com/the-origin-of-the-img-tag/" target="_blank">begins in 1995<span class="show-for-sr"> Opens in a new tab</span></a>, with the introduction of the humble <code>&lt;img></code> element.</p>
    <p>Along with it came the <code>alt</code> attribute, for specifying alternative text.</p>
    <p>If people know anything about accessibility on the web, it's probably the <code>alt</code> attribute.</p>
</section>
<section>
    <p>It's a deceptively simple concept - you have an image, and you provide an alternative to that image in text form.</p>
    <img src="/images/alternative.jpg" alt="What should the alternative text be?">
    <hr class="post-">
</section>
<section>
    <p>If you've got an image with text in it - just put the text in the alt attribute.</p>
    <p>If you've got an image that you can click to <em>do</em> something, describe what happens.</p>
    <img style="height:5rem" class="float-center" src="/images/play.svg" alt="Play this song (example)">
    <pre><code class="language-html">&lt;img src="/images/play.svg" 
    alt="Play the song 'Misty'"></code></pre>
</section>
    <hr>
<section>
    <h3>"A picture is worth a thousand words... Oh no."</h3>
    <p>It's our<a href="#team">*</a> responsibility to provide the same information in an alternative format, and that can be a challenge.</p>
</section>
<section>
    <figure><img src="/images/testing.jpg" alt="A graph showing COVID-19 testing in Ontario, having exceeded the April 29 goal of 14,000 per day." class="float-center" style="max-height: 30vh"></figure>
    <p class="post-only">We need to consider what the primary message of the image is. Graphs and charts are a great example of this. They have a huge volume of information, but to try and capture each data point would result in a volume of text that most users not only don't need, but would negatively affect their experience.</p>
    <p class="post-only">Instead, we think about what the 'message' of the data is.</p>
    <pre><code class="language-html">&lt;img src="/images/testing.jpg" 
        alt="A graph showing COVID-19 testing 
        in Ontario, having exceeded 
        the April 29 goal of 14,000 per day." ></code></pre>
</section>
    <hr>
<section>
    <p><h3>Things people get wrong about the <code>alt</code> attribute:</h3></p>
    <ul>
        <li><em>It's an attribute, not a tag</em> (tags are the opening and closing of an element, but the term 'tag' is often used to refer to elements).</li>
        <li><em>It is not interchangeable with the <code>title</code> attribute.</em> Title attributes are rudimentary tooltips that the HTML spec <a href="https://www.w3.org/TR/html51/dom.html#the-title-attribute">actually discourages you from using<span class="show-for-sr">&nbsp;Opens in a new tab</span></a> <strong>specifically because it's not accessible</strong>. A lot of people are under the mistaken impression that it is an accessibility requirement. It's <strong>the opposite of that</strong>.</li>
        <li>All images should have alternative text.</li>
        <li>Not all images need alt attributes.</li>
    </ul>
</section>
<section>
    <h3>No alternative</h3>
    <p>Let's talk about those last two points. 
        <ol><li>All images should have an alt tag. This is so everyone (i.e. the user, your team, Google's web crawler) knows if it's empty, that's <em>on purpose</em>.</li>
            <li>Some images should have empty alt attributes because the image has no meaning.</li></ol></p>
</section>
<section>
    <img style="height:10rem; transform: rotate(90deg);" src="/images/round-box.png" alt="An example of a decorative image, a transparent box with rounded corners." class="float-center">
    <p class="post-only">When I was a young web developer, we used images for pretty much <em>any</em> kind of decorative layout. Things like <code>border-radius</code> weren't supported in older browsers, so we rounded corners using images.</p>
    <p>This image, if used for decoration, <strong>should have an alt attribute, and it should be empty.</strong></p>
    <pre><code class="language-html">&lt;img src="rounded-box.png" alt=""></code></pre>
</section>
<section>
    <p>The goal of accessibility is to provide all people with the same information. If an image provides no (or redundant) information, then there doesn't need to be a text alternative to that image.</p>
    <p>What do I mean by redundant? The World Wide Web Consortium provides us with a <a href="https://www.w3.org/WAI/tutorials/images/decision-tree/" target="_blank">very handy decision-tree about what to include in your alt text<span class="show-for-sr"> Opens in a new window</span></a>.</p><p class="post-only">If you read through this (and it's a great thing to bookmark), you'll notice that most images don't need alternative text, <em>provided that the meaning is conveyed in real text nearby</em>.</p>
</section>
<section>
    <hr class="post-only"><p>To sum up, <strong>accessibility is making meaning available</strong>.</p>
    <p>If your meaning is only available in one form, and that form excludes some people, then create an alternative.</p>
</section>
<section>
    <hr class="post-only">
    <p>Depending on how much time we have today, I might pop into this pen I made and show you how to provide people with a good experience even when your images aren't loading.</p><p class="codepen" data-height="265" data-theme-id="dark" data-default-tab="result" data-user="simonborer" data-slug-hash="rNOqJJM" data-preview="true" style="height: 465px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Usability &amp;amp; Accessibility in the &amp;lt;picture&amp;gt; element">
  <span>See the Pen <a href="https://codepen.io/simonborer/pen/rNOqJJM">
  Usability &amp; Accessibility in the &lt;picture&gt; element</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script></section>
<section>
    <h2>Assignments</h2>
    <p>You're being assigned two things today.</p>
    <ol>
        <li><a href="#theReading">The Reading</a></li>
        <li><a href="#theGroupProject">The Group Project</a></li>
    </ol>
</section>
<section>
    <hr class="post-only">
    <h3 id="theReading">The Reading (or listening!)</h3>
    <p><strong>Step 1:</strong> Please read or listen to <a href="https://99percentinvisible.org/episode/on-average/">On Average</a> (or both, for the full experience).</p>
    <p><strong>Step 2:</strong> In Blackboard, please submit to me 250-500 words on the following topic: <em>How this article/podcast relates to the work of web development</em>.</p>
    <p>This is due <strong>one week from today</strong>.</p>
</section>
<section>
    <h3 id="theGroupProject">The Group Project</h3>
    <p><strong>Step 1:</strong> Individually, go to <a href="https://humber.ca" target="_blank">humber.ca<span class="show-for-sr"> Opens in a new window</span></a>.</p>
    <p><strong>Step 2:</strong> Individually, using the use case <strong>"Get directions to the Usability Lab"</strong>, evaluate the website based Jakob Nielsen's <a href="https://www.nngroup.com/articles/ten-usability-heuristics/" target="_blank">10 Usability Heuristics for User Interface Design<span class="show-for-sr"> Opens in a new window</span>.</a> Create a spreadsheet. For each heuristic, provide examples of where this was done well, or needs improvement.</p>
    <p><strong>Step 3</strong>: Get into groups, and compare notes. Create a spreadsheet of your evaluation <em>based on consensus</em>. What do you all agree was done well, or needs improvement, for each heuristic, with examples.</p>
    <p><strong>Step 4</strong>: Submit your individual and group spreadsheets via blackboard within the next two weeks.</p>
</section>
<footer class="post-only">
    <section>
        <h2>Footnotes</h2><span id="team">*</span><small>Well, it's the responsibility of whoever is generating the content, so feel free to tell someone else that it's not the job of a web developer to generate content.</small>
    </section>
</footer>
<section class="slide-only">
    <h3>Thank you!</h3>
</section>