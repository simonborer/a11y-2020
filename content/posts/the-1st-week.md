---
title: "Step 1: What are we talking about?"
date: 2019-09-02T08:47:11+01:00
featured_image: card-catalogue.jpg
summary: "Today we're going to look at an overview of the course, define our terms, and start a heuristic evaluation."
---
<section class="slide-only">
    <h2>Here's what we're going today</h2>
    <ol>
        <li class="fragment">Go over the syllabus</li>
        <li class="fragment">Define our terms</li>
        <li class="fragment">Learn about heuristics</li>
        <li class="fragment">
            Component of the week: &lt;picture&gt;
        </li>
    </ol>
</section>
<section class="slide-only">
    <h2>Syllabus</h2>
    <a href="/files/http5301-accessibility-and-usability-syllabus.pdf" target="_blank" class="button primary">Let's take a look at the syllabus =></a>
</section>
<section>
    <h2 class="post-only">Resources</h2>
    <hr class="post-only">
    <a class="button primary" href="/files/http5301-accessibility-and-usability-syllabus.pdf" target="_blank">Download the syllabus</a>
    <hr>
</section>
<section>
    <h2>This course (in chart form)</h2>
    <table>
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
    <h3>Why does it matter?</h3>
    <p>As with most of what you're learning in this program, it matters because <strong>it will make you good at making things</strong>. In most of your courses, you learn how to make things. In this course, you will learn how to make things <strong>for real people, better.</strong></p>
    <img src="/images/people.png" alt="Vectors of faces">
    <h3>How will we learn it?</h3>
    <p>In this course, we will:
        <ul>
            <li>Read materials related to usability, and reflect on them in the context of our work. <br>These are the <strong>reading assignments</strong>.</li>
            <li>Work in a team of 4-5 with fellow experts to evaluate a website based on an industry-standard checklist (a.k.a. a 'heuristic evaluation'). <br>This is your <strong>group assignment</strong>.</li>
            <li>Design a usability test for collecting good information about the website, application or component of your choice. <br>This is <strong>the brief</strong>.</li>
            <li>Carry out that test with 5 users, observing them using the website (or application, component, etc.) <em>while they are using only a screenreader or keyboard</em> (you'll pick one for all your users), and reporting to the class your findings. <br>This is <strong>the final report/presentation</strong>.</li>
        </ul>
    </p>
</section>
<section>
    <h2>Hi! Let's talk about things.</h2>
    <figure>
        <img src="/images/women.jpg" alt="Socially distanced people talking">
        <figcaption>...from a safe distance.</figcaption>
    </figure>
    <p>What better place to start in any discipline than knowing the jargon. It makes googling your problems so much easier! Let's jump into accessibility and usability by going over some of the common terms for the fields' general concepts.</p>
</section>
<section>
    <h3>In this lesson, we'll...</h3>
    <ol>
        <li class="fragment"><a href="#terms">Define general terms and concepts for both usability and accessibility.</a></li>
        <li class="fragment"><a href="#heuristicEvaluation">Learn how to perform a heuristic evaluation.</a></li>
    </ol>
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
</section>
<section>
    <p>Let's differentiate usability from some similar (and sometimes overlapping) terms.</p>
</section>
<section>
    <p><strong>Usability</strong>, as we said, is how quantitatively useful a product is.</p>
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
    <p>So, if we were to apply these terms to, and I'm dating myself here, an ipod...
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
    </p>
</section>
<section>
    <h3>Okay, so now that we know what usability is (and isn't), let's talk about some terms associated with <strong>how we test it</strong>.</h3>
</section>
<section id="heuristics">
    <img src="/images/lightbulb.jpg" alt="This is a decorative image, which doesn't need alt text, but I'm trying to set a good example.">
    <h3>Heuristics</h3>
    <p>For whatever reason, 'heuristic' is one of those words I have to look up every six months, I always forget the definition, probably because it's a little hard to define.</p>
    <p>An heuristic is a good-enough solution, an approximation, a rule of thumb. In usability, <strong>heuristic analysis</strong> is basically a checklist of good usability principles. You don't need to watch a live test subject to know that you need good error messages, or system feedback.</p>
</section>
<section><p>Heuristics aren't just something to test, they're rules to internalize when making things.</p><hr><p>The next term, <em>personas</em>, describes a tool that is typically used when designing (and adding to) a user workflow, but also come into play during usability testing.</p></section>
<section id="personas">
    <h3>Personas</h3>
    <p>Personas are a tool for creating a design. A persona is a fake person you use to represent a major user group for your product. Let's say you're a library, and you're creating a form to get people to sign up for an online account. You would create personas based on your current users, and any group that you want to target as a user (maybe you've got an ad campaign to drive new users to the website, for example).</p>
    <p>Based on the information you have, you might create personas for an elderly person, a parent with children, and a student. </p>
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
    <p>The purpose of making up a fake person, rather than simply pointing to your analytics data, is to facilitate design discussions (particularly with people who don't deal with analytics on the regular).</p>
    <p>The next term, <em>scenarios</em>, is also used during the design phase, but is a crucial element of usability testing.</p>
</section>
<section id="scenarios">
    <h3>Scenarios</h3>
    <p>Now that you've got an idea of who is using your site, you can go a step further and write down WHAT they're using the site for - these are called Scenarios. A Scenario is a set of tasks required to accomplish a user's goal.</p>
    <p class="post-only">Further reading: <a href="https://www.nngroup.com/articles/task-scenarios-usability-testing/" target="_blank">https://www.nngroup.com/articles/task-scenarios-usability-testing/</a></p>
    <p class="post-only"><hr>So, with your personas to guide you, you've developed a prototype application. Time to see if your fake people translate to real people - it's time for usability testing! In usability tests, you take your scenarios, and you ask people to try and accomplish the goal of that scenario. Then, you spy on them like a total creep! But it's fine because you have their consent and you're probably giving them $5 and some donuts. When you run your scenario, there are a number of ways that you can get data from the test.</p>
</section>
<section id="qualQuant">
    <h3>Qualitative and quantitative data</h3>
    <figure><img src="/images/data.jpg" alt="Data that doesn't mean anything. So, I guess, qualitative?"></figure>
    <p>Before we get into methods, let's define the two categories of data that we report. Quantitative and Qualitative, aka quant and qual.</p>
    <p><strong>Quantitative data</strong> is, naturally, data you can quantify. How long does it take to complete the task? How many errors does a user generate, etc. </p>
    <p><strong>Qualitative data</strong> is observational, and, generally, subjective. Is the user struggling to find a UI element? Is there a part of the interface that they seem to enjoy fiddling with? </p>
</section>
<section>
    <p>Quantitative research requires different conditions than qual, for a few reasons. First of all, <strong>to get good quantitative data, you need a large data set</strong>. You'll be running a lot of people through a well-defined and tightly controlled task set. Qualitative data, on the other hand, is gathered in a much looser and more adaptable way. Quantitative research is less common, but provides a business with some all-important numbers. <strong>Qualitative research is more subjective, as it's meant to be exploratory</strong>. Of course, when you're dealing with an organization, they'll still want numbers to supplement all your lovely written summaries and reports.</p>
</section>
<section id="qualQuant">
    <p>That's where PURE comes in - <strong>Pragmatic Usability Rating by Experts</strong>. This is just a rubric for putting your subjective findings into, so that your hunches and intuition get turned into numbers. You split your scenario into tasks, and your tasks into steps, and give each step a score out of three for how difficult the user found the task, 1 being easy, 3 being difficult.</p>
    <img src="https://media.nngroup.com/media/editor/2017/04/11/pure-product.png" alt="Examples of PURE evaluations.">
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
<section id="aoda">
    <h3>AODA</h3>
    <p>These guidelines are codified in the <a target="_blank" href="https://www.ontario.ca/laws/regulation/110191#BK14">AODA (Access for Ontarians with Disabilities Act) <span class="show-for-sr">Link opens in a new tab</span></a> specs.</p>
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

<section id="heuristicEvaluation">
    <ol>
        <li>Walk through the NN list</li>
        <li>assign the group project</li>
        <li>assign the reading (99%)</li></ol>
    Get into groups, and evaluate a site based on <a href="https://www.nngroup.com/articles/ten-usability-heuristics/" target="_blank">https://www.nngroup.com/articles/ten-usability-heuristics/</a>
</section>
<!-- <section id="scenarioWriting">
    <p>Review <a href="https://www.nngroup.com/articles/task-scenarios-usability-testing/" target="_blank">https://www.nngroup.com/articles/task-scenarios-usability-testing/</a> and Brainstorm task scenarios for a website, i.e. amazon</p>
</section> -->
<!-- <section id="page">
    <h3>Accessibility basics</h3>
    <p>See also: <a href="https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML" target="_blank">https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML</a></p>
    <ul>
        <li class="fragment">Semantics: Can you use a <code>button</code>?</li>
        <li class="fragment">Content: Can the <code>button</code> describe its function?</li>
        <li class="fragment">Focus: If it's not a button, can you trigger it anyway?</li>
        <li class="fragment">Tables: <code>scope</code> and <code>colspan</code></li>
        <li class="fragment">Inputs: <code>label</code> for id.</li>
        <li class="fragment">Images: <code>alt</code> text</li>
        <li class="fragment">Source order: Javascript, but also CSS (i.e. <code>flex-order</code>)</li>
    </ul>
</section> -->
<section class="slide-only">
    <h3>Thank you!</h3>
</section>