---
title: "Step 2: Collecting data"
date: 2020-05-23T08:47:11+01:00
publishdate: 2020-05-23T08:47:11+01:00
summary: "In which we learn what goes into a test plan, how to control the browser with your keyboard, what dark patterns are, and how to use a test script."
featured_image: hold-me-closer.jpg
---
<section>
    <h2>Here's what we're going to talk about today:</h2>
    <ol role="directory">
        <li class="fragment"><a href="#theBrief">What is <strong>The Brief</strong></a></li>
        <li class="fragment"><a href="#testPlan">What goes into a test plan</a></li>
        <li class="fragment"><a href="#keyboardControl">How to control the browser with your keyboard</a></li>
        <li class="fragment"><a href="#whosTheBoss">Who's the Boss</a></li>
        <li class="fragment"><a href="#testScript">Test script</a></li>
        <li class="fragment"><a href="#componentOfTheWeek">Component of the Week: Links</a></li>
    </ol>
</section>
<section id="lastWeek" class="slide-only">
    <h3>Last Week</h3>
    <ol>
        <li class="fragment">Usability is not the same as a bunch of other stuff</li>
        <li class="fragment">Accessibility is a good idea, and also it&#39;s the law.</li>
        <li class="fragment">&#39;Heuristic evaluation&#39; is just a fancy way of saying &#39;checklist of good ideas&#39;</li>
        <li class="fragment">Personas and Scenarios are tools for usability design and evaluation</li>
        <li class="fragment">Two kinds of data: quantitative and qualitative</li>
    </ol>
</section>
<section class="slide-only">
    <h3>What did you think of the reading?</h3>
</section>
<section id="theBrief">
    <h2>The Brief</h2>
    <p>This week you are being assigned <strong>The Brief</strong>, a.k.a a test plan.</p>
    <img src="/images/tremors.jpg" alt="Screenshot from the excellent Kevin Bacon movie 'Tremors', wherein Fred Ward is assuring us that there is a plan.">
</section>
<section>
    <p>This is your 2nd major assignment, due June 10th (2 weeks from now).</p>
    <p>Your final assignment will be to do usability testing and report your findings. This assignment is your plan for that testing.</p>
    <p>Today we'll learn what goes in that plan, and why.</p>
</section>
<section>
    <h3>The thing you're testing</h3>
    <p>The <em>thing</em> you are testing is up to you.</p> 
    <p class="callout"><strong>However</strong> I strongly recommend you test something <em>you are building/have built</em>, as you will gain insights into your own assumptions about the user.</p>
</section>
<section>
    <h3>What <em>about</em> the thing is being tested? What are you not testing?</h3>
    <p>The <em>scope</em> of what you are testing is going to be partly pre-defined, and partially negotiable.</p>
</section>
<section>
    <h3 class="slide-only">Things I decide about your scope</h3>
    <ul>
        <li>You must test 5 people; either 5 classmates or 5 people outside the class, <strong>not a mix of the two</strong>.</li>
        <li>If testing your classmates, they must use a screenreader.</li>
        <li>If testing people outside the class, they must only use a keyboard (no mouse).</li>
        <li>As part of feedback on your brief, I will discuss with you whether your scope is too large (you're testing too many things).</li>
    </ul>
</section>
<section id="testPlan">
    <h2>What goes into a test plan?</h2>
    <p>The goal of a test plan is to <strong>convince people it's a good plan</strong>.</p>
    <img src="/images/ghostbusters.jpg" alt="The scene from Ghostbusters where Bill Murray is excited about the plan.">
</section>
<section>
    <p>In the workplace, a test plan is what you submit to get approval for the plan and/or buy-in from your team. You can always make adjustments to go above and beyond!</p>
    <p><strong>Everything that you write in your test plan needs to have a 'why' explained.</strong></p>
</section>
<section>
    <p class="callout">If you want to see a test plan with <em>all</em> the bells and whistles, a comprehensive template is available at <a href='https://www.usability.gov/how-to-and-tools/resources/templates/usability-test-plan-template.html' target='_blank'>Usability.gov</a></p>
</section>
<section>
    <h2>Here are the things you need in your test plan.</h2>
    <h3>The Basics</h3>
    <ol>
        <li class="fragment"><strong><a href="#objective">Objective/Scope/Questions</a></strong>: what are you going to accomplish? What are you NOT going to accomplish? What are you trying to find out in order to accomplish your objective?</li>
        <li class="fragment"><strong><a href="#participants">Participants</a></strong>: who is going to take the test (and why have you selected them)?</li>
        <li class="fragment"><strong><a href="#methods">Methods</a></strong>: how are you going to generate data to answer your questions?</li>
        <li class="fragment"><strong><a href="#metrics">Metrics</a></strong>: how are you going to measure your data?</li>
    </ol>
</section>
<section>
    <h3>A step beyond the basics</h3>
    <ol>
        <li class="fragment"><strong>Executive summary</strong>: the whole plan, summarized in a couple paragraphs.</li>
        <li class="fragment"><strong>Schedule and location</strong></li>
        <li class="fragment"><strong>Equipment</strong></li>
        <li class="fragment"><strong>Scenarios</strong></li>
    </ol>
</section>
<section class="slide-only">
    <h3>Let's break some of these down</h3>
</section>
<section id="objective">
    <h3>Objective/Scope</h3>
    <p>You're probably not going to do a full, comprehensive usability test on a large website. You can test a set of features, or you can test for a set of issues. Define what these are and why you're investigating them.</p>
</section>
<section>
    <h3>Questions</h3>
    <p>Can users find <em>X</em>? Does <em>A</em> work better than <em>B</em>? Do users learn the interface in under <em>Y</em> amount of time?</p>
    <p>You need to explain what questions you're trying to answer, and <strong>why they matter</strong>.</p>
    <p class="post-only">A common analytics metric is the amount of time a user spends on a page. Why does this matter? <strong>It depends on the objectives of the site.</strong> Google wants users to spend a minimal amount of time on Google - it means the user has probably quickly found what they were looking for. The New York Times, on the other hand, wants users to spend a lot of time on their site, reading their content.</p>
    <p>When you define your questions, you must also explain why they are relevant to the product owner's interests.</p>
</section>
<section id="participants">
    <h3>Participants: Some magic numbers</h3>
    <p>What are the demographics of people you're testing? How many people are you testing?</p>
    <p>Jakob Nielsen reports the ROI thresholds in different usability testing methods:</p>
    <table>
        <tr>
            <td>Quantitative</td>
            <td>>20</td>
        </tr>
        <tr>
            <td>Card sorting</td>
            <td>>15</td>
        </tr>
        <tr>
            <td>Eyetracking</td>
            <td>39</td>
        </tr>
        <tr>
            <td>Heuristics</td>
            <td>4 experts</td>
        </tr>
        <tr>
            <td><strong>Qualitative</strong></td>
            <td><strong>5</strong></td>
        </tr>
    </table>
    <p class="post-only">Again, remember the <strong>purpose of the test plan</strong> - to make the argument that <em>your</em> tests will yield results that matter. So why are you testing the people you're testing?</p>
</section>
<section id="methods">
    <h3>Methods</h3>
    <p>Define your procedure, testing type, tools, and tasks.</p>
    <p>Make sure to include browser, screen-recording software, hardware and operating system details! These matter when trying to get good data.</p>
</section>
<section>
    <p>Testing types and tools include:</p>
    <ul>
        <li>heuristics (don't forget to say which heuristics - as we learned, there are many different heuristic checklists),</li>
        <li>eyetracking (not recommended - I haven't found a webcam-based eyetracking solution that wasn't super janky, and, as we'll see shortly, you need <strong>a lot</strong> of users for your data to hold up),</li>
        <li>discovery (finding problems by observing users pursue loosely defined goals),</li>
        <li>benchmark (testing out how well solutions perform),</li>
        <li>moderated/unmoderated (are you talking the user through the test? or just leaving them alone and recording?)</li>
        <li>remote/on-site</li>
        <li class="post-only"><a href="https://fivesecondtest.com/" target="_blank">5-second<span class="show-for-sr"> Opens in a new window</span></a></li>
        <li class="post-only"><a href="https://usabilityhub.com/guides/first-click-testing" target="_blank">First-click testing<span class="show-for-sr"> Opens in a new window</span></a></li>
        <li>etc., etc., etc.</li>
    </ul>
</section>
<section>
    <p class="callout">There are <em>so many</em> different kinds of tests out there <span class="slide-only">(including some in the notes I left out of the slides because I ran out of room!)</span>. Don't start planning with the test. Start by deciding <strong>what question you want answered</strong>, and then figure out how to answer it.</p>
</section>
<section id="metrics">
    <h3>Metrics</h3>
    <p>What is the data you'll be collecting? How should it be measured? How can you be sure it fully answers your questions?</p>
    <p>This is probably the <strong>most important part of your plan</strong>.</p>
</section>
<section class="post-only">
    <h3>Metrics - examples</h3>
    <p>
        <ul>
            <li><strong>Successful Task Completion</strong></li>
            <li><strong>Critical Errors</strong></li>
            <li><strong>Non-Critical Errors</strong></li>
            <li><strong>Error-Free Rate</strong> Error-free rate is the percentage of test participants who complete the task without any errors (critical or non-critical errors).</li>
            <li><strong>Time On Task</strong></li>
            <li><strong>Subjective Measures</strong> These evaluations are self-reported participant ratings for satisfaction, ease of use, ease of finding information, etc where participants rate the measure on a 5 to 7-point <a href='https://en.wikipedia.org/wiki/Likert_scale' target='_blank'>Likert scale</a>. A good, focussed example of this is the <a href="https://www.usabilitest.com/system-usability-scale" target="_blank">system usability scale<span class="show-for-sr"> Opens in a new window</span></a></li>
            <li><strong>Likes, Dislikes and Recommendations</strong> Participants provide what they liked most about the site, what they liked least about the site, and recommendations for improving the site.</li>
        </ul>
    </p>
</section>
<section class="slide-only">
    <h3>Metrics - examples</h3>
    <p>
        <ul>
            <li><strong>Successful Task Completion</strong></li>
            <li><strong>Critical Errors</strong></li>
            <li><strong>Non-Critical Errors</strong></li>
            <li><strong>Error-Free Rate</strong> Error-free rate is the percentage of test participants who complete the task without any errors (critical or non-critical errors).</li>
            <li><strong>Time On Task</strong></li>
        </ul>
    </p>
</section>
<section class="slide-only">
    <h3>Metrics - examples (continued)</h3>
    <p>
        <ul>
            <li><strong>Subjective Measures</strong> These evaluations are self-reported participant ratings for satisfaction, ease of use, ease of finding information, etc where participants rate the measure on a 5 to 7-point <a href='https://en.wikipedia.org/wiki/Likert_scale' target='_blank'>Likert scale</a>. A good, focussed example of this is the <a href="https://www.usabilitest.com/system-usability-scale" target="_blank">system usability scale<span class="show-for-sr"> Opens in a new window</span></a></li>
            <li><strong>Likes, Dislikes and Recommendations</strong> Participants provide what they liked most about the site, what they liked least about the site, and recommendations for improving the site.</li>
        </ul>
    </p>
</section>
<section class="post-only">
    <h3>Sections you may want to include:</h3>
    <ol>
        <li><strong>Executive summary</strong>: the whole plan, summarized in a couple paragraphs. This should be the last thing you write. If you can provide an effective, accurate summary, you've probably done a good job overall.</li>
        <li><strong>Schedule and location</strong>: Since you'll likely be doing this testing remotely, this probably isn't super important to have documented, <em>but</em> you'll need to figure this out at some point anyway.</li>
        <li><strong>Equipment</strong>: If you're using anything more elaborate than the items listed in the 'methods' section, you'll likely want to make note of it.</li>
        <li><strong>Scenarios</strong>: I only listed this as 'may want to include' (rather than 'must-have'), because not all testing types require scenarios. That being said <strong>I'm pretty darn sure you'll all want to write out your scenarios.</strong><p>As I'm sure you'll remember from last week, scenarios are the tasks & goals that your users will try to complete.</p></li>
    </ol>
</section>
<section class="slide-only">
    <h3>Sections you may want to include:</h3>
    <ol>
        <li><strong>Executive summary</strong>: the whole plan, summarized in a couple paragraphs. This should be the last thing you write. If you can provide an effective, accurate summary, you've probably done a good job overall.</li>
        <li><strong>Schedule and location</strong>: Since you'll likely be doing this testing remotely, this probably isn't super important to have documented, <em>but</em> you'll need to figure this out at some point anyway.</li>
    </ol>
</section>
<section class="slide-only">
    <h3>Sections you may want to include: (cont'd)</h3>
    <ol start="3">
        <li class="fragment"><strong>Equipment</strong>: If you're using anything more elaborate than the items listed in the 'methods' section, you'll likely want to make note of it.</li>
        <li class="fragment"><strong>Scenarios</strong>: I only listed this as 'may want to include' (rather than 'must-have'), because not all testing types require scenarios. That being said <strong>I'm pretty darn sure you'll all want to write out your scenarios.</strong><p>As I'm sure you'll remember from last week, scenarios are the tasks & goals that your users will try to complete.</p></li>
    </ol>
</section>
<section>
    <h3>Examples of test plans</h3>
    <ul>
        <li class="fragment"><a href="http://danielleklein.ca/wp-content/uploads/2016/08/Usability-test-plan-CSI.pdf" target="_blank">Centre for Social Innovation website<span class="show-for-sr"> Opens in a new window</span></a></li>
        <li class="fragment"><a href="https://gonzalesnick.com/wp-content/uploads/2019/08/lmb_usability_test_plan.pdf" target="_blank">Mobile app test plan<span class="show-for-sr"> Opens in a new window</span></a></li>
        <li class="fragment"><a href="http://booksite.mkp.com/barnum/testingessentials/pdfs/BWB_test_plan.pdf" target="_blank">Better World Books website<span class="show-for-sr"> Opens in a new window</span></a></li>
        <li class="fragment">Bonus: <a href="https://medium.com/@userfocus/the-1-page-usability-test-plan-dbc8c3d7fb54" target="_blank">Cheat Sheet<span class="show-for-sr"> Opens in a new window</span></a></li>
    </ul>
</section>
<hr>
<section id="keyboardControl">
    <h2>Learning to use the keyboard</h2>
    <table class="text-center"><thead><tr>
            <th>Command</th>
            <th>Mac Shortcut</th>
            <th>Windows Shortcut</th>
        </tr></thead>
        <tbody><tr>
            <td>Scroll up/down</td>
            <td colspan="2"><code>⇧ / ⇩</code></td>
        </tr>
        <tr>
            <td>Previous page</td>
            <td><code>Cmd+⇦</code></td>
            <td><code>Alt+⇦</code></td>
        </tr>
        <tr>
            <td>Next page</td>
            <td><code>Cmd+⇨</code></td>
            <td><code>Alt+⇨</code></td>
        </tr>
        <tr>
            <td>Change focus to next focussable element</td>
            <td colspan="2"><code>Tab</code></td>
        </tr>
        <tr>
            <td>Change focus to previous focussable element</td>
            <td colspan="2"><code>Shift + Tab</code></td>
        </tr>
        <tr>
            <td>Click on focussed element (i.e. link, submit)</td>
            <td><code>Return</code></td>
            <td><code>Enter</code></td>
        </tr>
        <tr>
            <td>Change the value of a form element (i.e. dropdown)</td>
            <td colspan="2"><code>⇧ / ⇩</code></td>
        </tr>
</tbody>
</table>
</section>
<section>
    <h3>An activity</h3>
    <ol>
        <li>Go to <a href="https://toronto.ca" target="_blank">toronto.ca<span class="show-for-sr"> Opens in a new window</span></a></li>
        <li>Get to the section with the breadcrumbs "City of Toronto / Business & Economy/ Industry Sector Support / Film / Plan Your Shoot / Letters of Notification"</li>
        <li>Find the phone number for the Toronto Film, Television & Digital Media Office.</li>
    </ol>
 </section>
 <section><p class="callout">If you like using the browser with the keyboard, you may enjoy what is probably <a href="https://github.com/philc/vimium" target="_blank">my favourite browser extension<span class="show-for-sr"> Opens in a new window</span></a>.</p></section>
 <hr>
<section id="whosTheBoss">
    <h2 class="post-only">Who's the boss?</h2>
    <img src="/images/whos-the-boss.jpg" alt="Who's the Boss? Angela. The answer is Angela." style="width:100%;">
    <hr class="post-only">
</section>
<section>
    <p>When creating a test plan, we must ask the right questions. The right questions can tell us how to improve things. In order to ask the right questions, you must first know <strong>who are you trying to improve things for.</strong></p>
</section>
<section>
    <img src="/images/modal.png" alt="A terrible pop-up" style="max-height: 40vh;">    
    <p class="post-only">In the above image, someone has asked the question <em>"How do we increase our newsletter subscriptions?"</em></p>
    <p class="post-only">And the answer is <em>"A pop-up will increase our newsletter subscriptions by 5%".</em></p>
    <p class="post-only">No one asked the question <em>"Will 95% of our users hate their experience?"</em></p>
    <p class="post-only">Just to take this one step further, I want to talk about something called 'dark patterns'.</p>
</section>
<section>
    <h3>Dark Patterns</h3>
    <p>Dark patterns are design patterns that are meant to manipulate the user.</p>
    <p>Dark patterns are not bad design - they are good design for bad reasons.</p>
</section>
<section>
    <table cellspacing="0" style="font-size:1.25rem">
        <tbody>
            <tr>
                <td>Psychological Insight</td>
                <td>Applied Honestly (benefits users)</td>
                <td>Applied Deceptively (benefits business)</td>
            </tr>
            <tr>
                <td>“We don’t read pages. We scan them” —Steve Krug</td>
                <td><strong>Aid rapid comprehension:</strong> ensure key content is shown in headings, subheadings (etc), using a strong visual hierarchy.</td>
                <td><strong>Hide key information:</strong>
                    Bury facts within paragraphs of text, so some users will proceed without fully understanding the transaction.</td>
            </tr>
            <tr>
                <td>“People tend to stick to the defaults” —Jakob Nielsen</td>
                <td><strong>Prevent mistakes:</strong>
                    Default to the option that’s safest for the user. In important contexts, don’t use defaults and require the user to make an explicit choice.</td>
                <td><strong>Benefit from mistakes:</strong>
                    Ensure default options benefit the business, even if this means some users convert without meaning to.</td>
            </tr>
            <tr>
                <td>“People will do things that they see other people are doing” —Robert Cialdini</td>
                <td><strong>Show unedited feedback:</strong>
                    Allow real customers to share their experiences, so they can make accurate pre-purchase evaluations.</td>
                <td><strong>Bury negative feedback:</strong>
                    Hand-pick positive feedback and display it prominently. Bury negative feedback so it is hard to find.</td>
            </tr>
        </tbody>
    </table>
    <blockquote><cite><a href="https://alistapart.com/article/dark-patterns-deception-vs.-honesty-in-ui-design" target="_blank">A List Apart: Honesty in UI Design<span class="show-for-sr"> Opens in a new window</span></a></cite></blockquote>
</section>
<section>
    <p>Dark patterns test <em>really</em> well.</p>
    <p>Dark patterns could be in legacy code, they could be given to you to develop, or they could even come from you.</p>
    <p>This type of design happens because decisions are being made based on metrics, not a focus on the end user. Whether the company is malicious, or just lazy, doesn't really matter to the end user. But if you see this type of design happening regularly at your work, it might be time to look for a new job.</p>
</section>
<section>
    <p>You need to write your usability plan so that you <strong>justify all your choices to the product owner</strong>.</p>
    <p>On rare occasions, the product owner will have interests that won't be apparent to the user (for example, <em>Do customers notice if we move to cheaper hosting?</em>). If your product owner has interests that conflict with the user, you should run the other way.</p>
</section>
<section><h2>Helping one another</h2></section>
<section>
    <h3>You are biased (don&#39;t worry, everybody is)</h3>
    <p>This is an individual assignment. You will write your test plan alone. You will present your test results alone.</p>
    <p>I want you to consider <em>performing</em> the tests with a helper.</p>
    <p>You are not aware of everyone, and worse yet, you are not aware of yourself. You are not objective. That's ok.</p>
</section>
<section>
    <p>In “<a href='https://vtechworks.lib.vt.edu/handle/10919/26477' target='_blank'>Usability Problem Description and the Evaluator Effect in Usability Testing</a>” a study by Miranda G. Capra at Virginia Tech, she found that 44 usability practitioners’ evaluations reported problems that overlapped by only 22 percent.</p>
    <p>Confirmation bias is likely going to be your biggest issue to watch out for, in yourself and other members of your team. It can occur in planning (how you phrase your questions), testing (how you interact with a subject), and analysis (how you interpret the data).</p>
</section>
<section>
    <h3>You are less biased when you work together</h3>
    <p>Capra found that '[a]dding a second evaluator results in a 30-43% increase in problem detection'.</p>
    <p><span class='slide-only fragment'>Your assignments are not group work, but your results will be better if you trade responsibilities.</span></p>
</section>
<section>
    <h3>You are less biased when you stick to the script</h3>
    <p>A key reason we write our test plan is for transparency. We need to make our work reviewable so that our unconscious biases can be recognized. The more we can script, the better.</p>
    <p>Steve Krug is one of the big names in usability, and he has given us a wonderful sample script to work from. Let`s take a look <a href='/supplemental/test-script.html' target='_blank'>Steve Krug's sample script<span class="show-for-sr"> Opens in a new window</span></a>.</p>
</section>
<section>
    <h2>An activity</h2>
    <p>Get together in pairs, and read the script to one another.</p>
    <p>Answer the following questions:</p>
    <ul>
        <li>How will this script need to be adapted for remote testing?</li>
        <li>What is the purpose of questions like "what’s the split between email and browsing [in your weekly internet usage]"?</li>
        <li>Why do we need to assure the user "we’re testing the <em>site</em>, not you"?</li>
        <li>What type of data is being collected here? Quantitative? Qualitative?</li>
        <li>Find four examples of the types of data that could be collected in this user test.</li>
        <li>What would you change in this script? Why?</li>
    </ul>
</section>
 
 <section id="componentOfTheWeek">
     <h2>Component of the Week: Links</h2>
     <p>Ah, the hyperlink: the core concept of the <a href="https://en.wikipedia.org/wiki/Hypertext">World Wide Web</a>.</p>
     <pre><code class="language-html">&lt;a href="the internet">You're welcome.&lt;/a></code></pre>
     <p>Simple and straightforward, but so ubiquitous and flexible as to invite abuse, and therefore, inaccessibility.</p>
     <p>As I'm sure you've heard, one of the cornerstones of accessibility is <strong>semantic markup</strong>. In other words, <em>use elements for their intended use</em>. We'll better understand the purpose of an anchor tag shortly.</p>
</section>
<section>
     <p>There are only a couple of accessibility mistakes you can make with an anchor tag, while still using it semantically.</p>
     <p>One mistake I made for years: <strong>the text of a link should not be a URL</strong>. Many popular screenreaders <em>will not allow the user to skip while it reads the text of a link</em>.</p>
     <pre><code class="language-html">&lt;a href="guesswhat.co.uk">
https://www.guesswhat.co.uk/I/sound/super/
annoying.php?so=don-t&do=this&to=your&user=ok&lt;/a></code></pre>
<pre class="post-only"><code class="language-html">&lt;a href="guesswhat.co.uk">
You know what? Large volumes of text inside 
links are also not a great idea. We can't put long, 
rambling text in our links like we used to, 
but we have our ways. One trick is to tell 'em stories 
that don't go anywhere - like the time I caught the 
ferry over to Shelbyville. I needed a new heel for my 
shoe, so, I decided to go to Morganville, which is 
what they called Shelbyville in those days. So I tied 
an onion to my belt, which was the style at the time. 
Now, to take the ferry cost a nickel, and in those 
days, nickels had pictures of bumblebees on 'em. Give 
me five bees for a quarter, you'd say. Now where were 
we? Oh yeah: the important thing was I had an onion on 
my belt, which was the style at the time. They didn't 
have white onions because of the war. The only thing 
you could get was those big yellow ones...&lt;/a></code></pre>
</section>
<section>
      <p>Another thing to keep in mind is that links are an in-page navigational tool. When using the keyboard to navigate a page, the user can hit the tab button to go to each interactive element in sequence. This means that if the context for a link comes before that link, people using screenreaders will have not context for that link. Stuff like this is really unhelpful:</p>
      <pre><code class="language-html">&lt;a href="/somewhere-else">Read more&lt;/a></code></pre>
</section>
<section>
      <p>That being said, just like with images, screenreaders will inform the user that what they're focussed on is a link, so it's redundant to tell them:</p>
      <pre><code class="language-html">&lt;a href="https://en.wikipedia.org/wiki/Redundancy">
Link to Read More about Redundancy&lt;/a></code></pre>
</section>
<section>
      <p>And finally, shifting a user into a new window or tab can be disorienting if you don't give them a heads-up.</p>
      <pre><code class="language-html">&lt;a 
href="https://en.wikipedia.org/wiki/Tab_(interface)" 
target="_blank">Read about Tabs on Wikipedia
&lt;span style="font-size: 0"> Opens in a new tab&lt;/span>
&lt;/a></code></pre>
</section>
<section>
    <p>Let's see what happens when we start to get "creative" with links:</p>
    <pre><code class="language-html">// Links must be recognizable
&lt;a style="text-decoration:none;">
I need a non-colour visual indicator&lt;/a></code></pre>
</section>
<section>
<pre><code class="language-html">// There is a temptation to use links as buttons.
// That's bad, because the user is told it's a link.
&lt;a onclick="tooLazyToStyleAButton()">
Why can't buttons be buttons?&lt;/a></code></pre>
</section>
<section>
<pre><code class="language-html">// But I want my image to be linked!
&lt;a href="/image-destination">
    &lt;img src="this-totally-works.jpg"
        alt="The user will be read the alt text 
        as the link text!" />
&lt;/a></code></pre>
</section>
<section>
<pre><code class="language-html" style="font-size: 1rem;line-height: 1.2">// If you have something that behaves like a link
// but for some very good, very important reason 
// cannot be an anchor, you can use the 'role' 
// attribute
// 
// 'role' is an ARIA attribute, which we'll dive
// much deeper into in the second half of the term
// but notice what it does here - 
// when HTML isn't semantic, it provides the 
// information that WOULD have come from the 
// semantic element.
// 
&lt;style>
[role="link"] { color: blue; text-decoration: underline; cursor: pointer; }
[role="link"]:focus { outline: 1px dotted black;}
&lt;/style>
&lt;div role="link" onclick="window.open('https://google.com')">Link
&lt;/div></code></pre>
 </section>
