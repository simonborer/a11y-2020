---
title: "Step 3: Analyze & Report"
date: 2020-05-28T08:47:11+01:00
publishdate: 2020-05-28T08:47:11+01:00
featured_image: confused.png
summary: "What to do with your data: collecting, compiling, analyzing, reporting and presenting."
---
<section>
    <h2>Here's what we're going to talk about today:</h2>
    <ol>
        <li class="fragment"><a href="#collection">Data collection</a></li>
        <li class="fragment"><a href="#compilation">Data compilation</a></li>
        <li class="fragment"><a href="#analysis">Data analysis</a></li>
        <li class="fragment"><a href="#reporting">Data reporting</a></li>
        <li class="fragment"><a href="#presenting">Data presenting</a></li>
        <li class="fragment"><a href="#componentOfTheWeek">Component of the Week</a></li>
    </ol>
</section>
<section>
    <p>So, last week we looked at how to <strong>ask good questions</strong> that will give us reliable data.</p>
    <p>We talked about how to vet those questions for bias (<strong>peer review</strong>).</p>
    <p>We talked about how to <strong>script those questions</strong> (and/or the language that frames them) in order to keep our data consistent, and avoid leading the subject.</p>
</section>
<section>
    <p>Today we're going to talk about the 5-step process that's going to get you to the finish line (aka your final report):</p>
    <ul>
        <li>collecting our data</li>
        <li>compiling our data</li>
        <li>analyzing our data</li>
        <li>reporting our data</li>
        <li>presenting our data</li>
    </ul>
</section>
<section id="collection">
    <h2>Data collection</h2>
    <p>Data collection is the step that takes place <em>during</em> the execution of the test.</p>
    <p>Since you've already defined, in your test plan, the "whys", the "hows" and the "what types" of data you're collecting, the actual process of collecting data should be fairly straightforward.</p>
    <p>Most likely, you'll be doing some combination of the following:</p>
    <ul>
        <li>Taking notes (or having a partner take notes)</li>
        <li>Screen/video recording</li>
        <li>Tracking in Excel/Google Sheets/Airtable/some kind of git-based csv workflow.</li>
    </ul>
    <p>Of course, you're allowed to have an assistant (or heck, as many assistants as you'd like), but it's unlikely that you'll encounter the kind of messiness that comes from working as part of a larger team.</p>
    <p>That being said, you should have a plan for <strong>your data collection workflow</strong>. <em>(Note: this might be a nice thing to include in your test plan)</em></p>
</section>
<section>
    <p>A workflow plan for a small project can be quite simple.</p>
    <h3>For example...</h3>
    <blockquote>
        <ul class="nested-list">
            <li>Screen recordings backed up to Dropbox</li>
            <li>Observations in spreadsheet for each participant:
                <ul>
                    <li>1 tab per goal</li>
                    <li>2 columns per task
                        <ul>
                            <li>1st column / task - errors are entered in rows with colour coding for severity</li>
                            <li>2nd column / task - timestamp</li>
                        </ul>
                    </li>
                </ul>
            </li>
            <li><abbr title="System usability scale">SUS</abbr> as Google Form</li>
        </ul>
    </blockquote>
    <p>...or whatever is appropriate for the type of data <em>you</em> are collecting.</p>
    <p>Point is, it's a really good idea to define where the data's going to go, and how you'll keep it organized, <em>before</em> it's time to compile it.</p>
</section>
<section id="compilation">
    <h2>Data compilation</h2>
    <p>Data compilation is the step whereby you prepare your data for analysis.</p>
    <p>For those of you who are working exclusively quantitative data, this will be sort of a mini-step. You may write some Excel formulae and be done with it.</p>
    <p>When dealing with qualitative data, however, you'll need to decide (preferrably ahead of time), how you're going to compile your data.</p>
    <p>One example of compiling qualitative data is a word cloud. Personally, I happen think word clouds are a stupid way to present data. They look "cool" (do they though?), but don't actually show you word frequency in a way that's easy to parse (as the words are usually fairly close in size), so people's brains will pick up on the words that confirm their biases (which is why people like word clouds, really).</p>
    <figure>
        <img src="/images/word-cloud.png" alt="A word cloud, wherein the largest words are 'think', 'trust', 'smart', and 'communicating'.">
        <figcaption><strong>Input text: </strong>Word clouds aren't a smart way for smart people to control for their biases.
            Frankly when I see a word cloud I think "I can't trust what this person says - they're either communicating that they're not smart, or they're communicating that they think I'm not smart".
            Are they worthy of your trust? Of course not. Don't trust them. There's no good reason to think they're good at communicating. Individual words don't communicate meaning. What do words mean? Nothing, at least not when they're in a word cloud.</figcaption>
    </figure>
</section>
<section>
    <p>Since you're dealing with a small sample size, you could simply present individual answers, and that <em>can</em> be valuable, but only when that single data point is significant.</p>
    <p>Single data points are significant when that individual teaches us something about a larger issue.</p>
    <p>For example: "One participant took 20 seconds longer than others to fill out this form. When we asked them why, they said their cat walked across their keyboard." <strong>Not significant.</strong></p>
    <p>A different example: "One participant was confused by the error message. They recently immigrated from China, where the colour red does not signify an error, and the content of the error message didn't actually <em>explicitly say</em> it was an error message." While this participant might be the only one of the 5 participants that was confused by this, the <em>reason</em> they were confused raises a potential <strong>significant usability problem</strong> for a lot of people.</p>
    <p>The inverse is true as well - aggregate data is only as important as the lessons we take away from it.</p>
    <p>When compiling your data, <strong>don't pass judgement</strong> by ignoring potentially significant data (individual or aggregate) until you've analyzed and determined its validity.</p>
</section>
<section id="analysis">
    <h2>Data Analysis</h2>
    <p>Data analysis is the step where you find out the answers to your questions (and make new discoveries!)</p>
    <p>Just like in the compilation stage, the complexity of this step is defined by the kind of data you're dealing with, and the kinds of questions you asked.</p>
    <p>If you already have a tightly-defined hypothesis (i.e. "If users can complete the 'checkout' task in <120 seconds with no critical errors, the 'checkout' task does not require a redesign"), and you're dealing with quantitive data, analyzing those results will be fairly simple.</p> <p class="callout"><u>Are users regularly able to complete the 'checkout' task in under 120 seconds?</u><br>
            Users averaged completion of the 'checkout' task in 96 seconds. The minimum completion time was 88 seconds. The maximum time was 104 seconds. No critical errors were observed. <strong>We can conclude that the 'checkout' task does not require a redesign.</strong></p>
    <p>If you have a more loosely-defined hypothesis (i.e. "Users may find alternate ways of completing the checkout process"), this step may be more labourious. <strong>The amount of work you have to do in this stage isn't a sign of success or failure, it's a function of your methods and data types.</strong></p>
</section>
<section>
    <h3>Facts vs. Conclusions vs. Speculation</h3>
    <p>In the compilation phase, you are able to generate <strong>facts</strong>.</p>
    <p>Facts are not valuable in and of themselves. In the analysis phase, you must turn facts into answers.</p>
    <figure>
        <img src="/images/margarine-chart.jpg" alt="A chart showing a strong correlation between divorce rates in Maine and per capita margarine consumption.">
        <figcaption>Source: <a href="https://www.tylervigen.com/spurious-correlations" target="_blank">Spurious Correlations<span class="show-for-sr"> Opens in a new window</span></a></figcaption>
    </figure>
    <p>Again, this is not a group project, but I <strong>strongly encourage you</strong> to have a partner challenge your conclusions.</p>
    <p>A fact that doesn't answer a question is not important.</p>
    <p>A conclusion supported by facts is important.</p>
    <p>Speculation is also important, so long as it is presented as a line of further inquiry, and not a conclusion!</p>
    <p>Consider the following facts (via <a href="https://www.nature.com/news/the-myopia-boom-1.17120" target="_blank">Nature.com<span class="show-for-sr"> Opens in a new window</span></a>):</p>
    <p><strong>Fact:</strong> Sixty years ago, 10–20% of the Chinese population was short-sighted.</p>
    <p>Without a relevant question, this fact doesn't matter much.</p>
    <p>Let's add context (more facts) to raise a question.</p>
    <p><strong>Fact:</strong> Today, up to 90% of teenagers and young adults in China are short-sighted.</p>
    <p>Ok, now things are getting interesting. We see a change over time, which leads us to believe that something is having an impact. We can <strong>speculate</strong> - higher rates of diagnosis? More reading/detail-oriented work?</p>
    <p><strong>Fact:</strong> At a school in southern Taiwan, teachers were asked to send children outside for 80 minutes of their daily break time instead of giving them the choice to stay inside. After one year, doctors had diagnosed myopia in 8% of the children, compared with 18% at a nearby school.</p>
    <p>Those of you with a scientific background will know that this isn't a large or well-controlled enough of a study to draw strong scientific conclusions from, and doesn't rule out other factors contributing to myopia, but it does suggest a statistically-significant connection.</p>
    <p>For the purposes of usability testing, we are looking for <strong>strong connections</strong> (not necessarily conclusive evidence).</p>
</section>
<section>
    <p>As a little aside, let's look at a common pattern of abusing statistical significance: 'p-hacking'.</p>
    <figure>
        <img src="https://imgs.xkcd.com/comics/significant.png" alt="XKCD comic about p-hacking">
        <figcaption>via <a href="https://xkcd.com/882/" target="_blank">XKCD<span class="show-for-sr"> Opens in a new window</span></a></figcaption>
    </figure>
    <p>P-hacking is the manipulation of data's 'p-value', a.k.a. the likelihood of data being coincidental.</p>
    <p>Let's take a look at 538's wonderful <a href="https://projects.fivethirtyeight.com/p-hacking/" target="_blank">p-hacking interactive tutorial<span class="show-for-sr"> Opens in a new window</span></a>.</p>
</section>
<section>
    <p>As we said, some of your data analysis will be simply testing a hypothesis - taking your assumptions and seeing if they are correct.</p>
    <p>There is also analysis that discovers new ideas - answering questions you didn't think to ask in the first place, but are valuable nonetheless.</p>
    <p>One type of "post hoc" (after the fact) analysis is "task analysis".</p>
</section>
<section>
    <h3>Task analysis</h3>
    <p>When you provide users with scenarios (a.k.a goals), you'll probably want to break down those goals into the steps they would take to accomplish those goals.</p>
    <p>What users actually <em>do</em> is another story. By looking at the tasks users actually perform, you can gain valuable insights into how users use your web site.</p>
</section>
<section>
    <h3>Task analysis topics</h3>
    <ol>
        <li class="fragment">Trigger: What prompts users to start their task?</li>
        <li class="fragment">Desired Outcome: How users will know when the task is complete?</li>
        <li class="fragment">Base Knowledge: What will the users be expected to know when starting the task?</li>
        <li class="fragment">Required Knowledge: What the users actually need to know in order to complete the task?</li>
        <li class="fragment">Artifacts: What tools or information do the users utilize during the course of the task?</li>
    </ol>
</section>
<section>
    <h3>Task analysis topics</h3>
    <p>With a partner, perform a task analysis of their journey to class today. Use your judgement in determining the level of detail that is appropriate to find efficiences in their journey. Was their journey optimal?</p>
</section>
<section>
    <p>Data analysis is a complicated topic, and it depends largely on what questions your trying to answer/topics you're trying to investigate, and what type of data you're working with.</p>
    <p>The best advice I can give you is to <strong>find some people who will challenge you</strong>.</p>
</section>
<section id="reporting">
    <h2>Reporting your data</h2>
</section>
<section>
    <h3>Presenting solutions</h3>
    <p>Now that you've understood your data, it's time to generate some solutions.</p>
    <p>Keep solutions specific and positive - 'don't use hamburger menus' isn't an action, it's a non-action.</p>
    <p>The gold standard is 'elegance', which is just a fancy way of saying 'cheap, fast, easy and effective'.</p>
    <p>Most solutions won't be elegant though. It's up to you to be mindful of how resource-heavy your solutions are - and how certain you are of their efficacy.</p>
</section>
<section>
    <p>The more uncertain you are of a solution, the more you'll need to be prepared to present multiple options, and to speak to the pros and cons of each one.</p>
    <p>Consider laying out your solutions in a chart graded for issue severity and actionability.</p>
</section>
<section>
    <h3>Make it readable</h3>
    <p>A usability report is, at its best, a plan for action. There are two types of 'takeaway's:</p>
    <ul>
        <li>Things to improve, and </li>
        <li>things to investigate further.</li>
    </ul>
    <p>Make the case for your recommendations.</p>
</section>
<section>
    <h3>How to tell people how they can improve</h3>
    <p>Now that you've understood your data, it's time to generate some solutions.</p>
    <p>Keep solutions specific and positive - 'don't use hamburger menus' isn't an action, it's a non-action.</p>
    <p>The gold standard is 'elegance', which is just a fancy way of saying 'cheap, fast, easy and effective'.</p>
    <p>Most solutions won't be elegant though. It's up to you to be mindful of how resource-heavy your solutions are - and how certain you are of their efficacy.</p>
</section>
<section>
    <p>The more uncertain you are of a solution, the more you'll need to be prepared to present multiple options, and to speak to the pros and cons of each one.</p>
    <p>Consider laying out your solutions in a chart graded for issue severity and actionability.</p>
</section>
<section>
    <h3>A basic structure for your report:</h3>
    <ol>
        <li class="fragment">What we did</li>
        <li class="fragment">Why we did it</li>
        <li class="fragment">How we did it</li>
        <li class="fragment">What we learned</li>
        <li class="fragment">What should be done</li>
        <li class="fragment">All the boring data that backs this up</li>
    </ol>
</section>
<section>
    <h3>Be useful</h3>
    <ul>
        <li class="fragment">Be specific</li>
        <li class="fragment">It&#39;s not the user&#39;s fault</li>
        <li class="fragment">Don&#39;t recommend making small changes to a big problem</li>
        <li class="fragment">Don&#39;t redesign for them</li>
        <li class="fragment">Align with the client&#39;s priorities</li>
        <li class="fragment">Help the client prioritize</li>
    </ul>
</section>
<section>
    <h3>Another possible format:</h3>
    <p>Via <a href="https://uxdesigntemplates.com/resource/user-testing-report-template" target="_blank">UX Design Templates<span class="show-for-sr"> Opens in a new window</span></a></p>
    <ol>
        <li class="fragment">Cover sheet</li>
        <li class="fragment">Test outline</li>
        <li class="fragment">Test participant details</li>
        <li class="fragment">Executive summary</li>
        <li class="fragment">Bugs list</li>
        <li class="fragment">Sheets for key findings (including usability problems and positives)</li>
        <li class="fragment">Post-test question responses</li>
        <li class="fragment">Full list of recordings</li>
    </ol>
</section>
<section>
    <p>Being informal doesn't mean being lazy. It's actually more difficult - you need to explain thoroughly, but in simple terms, and in a way that's easy to synthesize.</p>
    <p>You're telling people how best to spend their money. Think about what they care about - what works, quick wins, and big wins.</p>
</section>
<section>
    <p>That said, if you want a jumping-off point for a more formal documentation format, here's a couple:</p>
    <p>
        <ul>
            <li><a href="http://www.sage-research.com/v4/sage_usability_study_report_example.pdf" target="_blank">Sage Research: Usability Study Report<span class="show-for-sr"> Opens in a new window</span></a></li>
            <li><a href="https://www.usability.gov/how-to-and-tools/resources/templates/report-template-usability-test.html" target="_blank">Usability.gov: Usability Test Report Template<span class="show-for-sr"> Opens in a new window</span></a></li>
        </ul>
    </p>
</section>
<section>
    <h2 id="presenting">Presenting data</h2>
    <p>Now that your report is ready, you'll need to give a sort of 'executive summary' as a 5-minute presentation. My advice: start with the conclusions and work backwards.</p>
</section>
<section>
    <h3>Presenting a story</h3>
    <p>The point of all this is to give people something they can use. Data is boring. If your report puts them to sleep, they won't use it. Anecdotes are fun, but lack credibility. People won't use your report if they don't feel they can trust it.</p>
    <p>Use enough data to build a credible story, but focus on appealing to the things that people really pay attention to.</p>
</section>
<section>
    <p>Be funny. Be informal. Think of your report as having <a href='http://channel101.wikia.com/wiki/Story_Structure_101:_Super_Basic_Shit' target='_blank'>a beginning, middle, and end <span class="show-for-sr"> Opens in a new window</span></a>. Tell the story of the website, the testing, the results, and the solutions. And yes, even the data.</p>
    <p>The best way to do this is to focus on people. Talk about yourself, the participants, the website's audience, the client. That's the only real way to help us all figure out why the data matters.</p>
</section>
<section>
    <h2>A Survey</h2>
    <p>In preparation for our lab work, please take the survey entitled 'Test Survey' under Notes & Assignments in Blackboard.</p>
</section>
<section id="componentOfTheWeek">
    <h2>Component of the Week</h2>
    <p class="codepen" data-height="357" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="bd8f4f5f4585af1269f193c6632807f7" style="height: 357px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Accessible toggle">
    </p>
    <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    <p style="margin-top:2rem;">The most complex concept when creating accessible content is communicating a change of state.</p>
    <p>State changes are most often apparent becuase of visual cues.</p>
    <p>In the above example, we have a toggle switch. In some cases, a toggle switch should just be a radio button (which, as a native form element, is inherently accessible). However, a 'toggle' can sometimes better communicate the idea of submitting a default binary value, rather than choosing one from a group of values.</p>
    <p>Toggles are <strong>not</strong> inherently accessible, because they are not native HTML elements - so we have to communicate their purpose, and not just visually.</p>
    <p>Luckily, ARIA recognizes that they are a common feature, so we have a <code>role</code> value available: <pre><code class="language-html">&lt;button role="switch"></code></pre></p>
    <p>With this role, we can pass the <code>aria-checked</code> true and false values to indicate whether it's 'on' or 'off'.</p>
    <p>We change these values with javascript.</p>
    <p>We're also able to tie our styles with the attributes that make this switch accessible - meaning we make accessibility mandatory.</p>
    <p>One more important thing to note is the <code>aria-labelledby</code> attribute - meaning that anyone landing on our toggle will know what it's for, without having to backtrack.</p>
</section>