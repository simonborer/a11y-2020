---
title: "Week 7... Plus Week 8?"
date: 2020-06-30T08:47:11+01:00
publishdate: 2020-06-30T08:47:11+01:00
featured_image: groundhog.jpg
summary: "This week I've combined last year's week seven and eight"
---
<section>
    <h3>The internet is open</h3>
    <p>We work on an open platform. The beautiful thing about the internet is that it is a (nearly) global public space built on open access (e.g. Net Neutrality), standards and specifications. This comes with the responsibility, though, that you create services that are meant to be consumed by clients that haven't even been invented yet.</p>
    <p>You will work with (and by with, I mean for) people who do not understand the difference between accessing a pdf and opening a webpage.</p>
    <p>Having an open spec markup language is the backbone of the information age.</p>
</section>
<section>
    <h3>Firefox gets most of their money from...</h3>
    <p class="fragment">Google</p>
    <h3 class="fragment">Wait, why?</h3>
    <p class="fragment">Google's business model depends on the open web. It has made a multi-billion dollar bet that the best place to be is not in a "walled garden", but as the concierge to the innovations afforded by a democratized space.</p>
</section>
<section>
    <h3>You will need to advocate for answering hard questions</h3>
    <p>For those people who do not understand HTML vs PDF, you will need to impress on them that the internet is a place with a multitude of users, and that's not changing anytime soon. You will need to advocate for creating a service rather than an interactive paper flyer.</p>
    <p>This distinction is important because it acknowledges your many types of end user - from the dev/content/QA team, to Google's web crawler, to hackers, to archive.org, to Pocket and Instapaper, to screen readers, to everybody.</p>
</section>
<section>
    <h3>Users at cross-purposes</h3>
    <blockquote>I’m dyslexic, and one of the recommendations for reducing visual stress that I’ve found tremendously helpful is low contrast between text and background color. This, though, often means failing to meet accessibility requirements for people who are visually impaired... Consider:
        <ul>
            <li>Designing for one-handed mobile use raises problems because right-handedness is the default—but 10 percent of the population is left handed.</li>
            <li>Giving users a magnified detailed view on hover can create a mobile hover trap that obscures other content.</li>
            <li>Links must use something other than color to denote their “linkyness.” Underlines are used most often and are easily understood, but they can interfere with descenders and make it harder for people to recognize word shapes.</li>
        </ul>
        <br>
        <cite>Eleanor Ratliff, <a href="http://alistapart.com/article/accessibility-whack-a-mole" target="_blank">http://alistapart.com/article/accessibility-whack-a-mole</a></cite>
    </blockquote>
</section>
<section>
    <h3>Your job is not to write code - it is to solve problems</h3>
    <p>All the easy code has been written already. Don't worry, there are (for the time being), still plenty of jobs writing boring code. But that is less true than it was ten years ago, and will be less true in another ten. You need to think of yourself as someone who can solve the problem of 'How can we best make this work for everyone who needs it?'</p>
    <p>Last week we contrasted accessibility with usability by saying that usability is accessibility for a set audience, but accessibility legislation still limits that audience by defining it. You should always be open to expanding your definition of the end user.</p>
</section>
<section>
    <h3>Youtube stumbled on an audience</h3>
    <p>A few years ago, the Youtube dev team gave themselves a page-weight budget of 800kb. They optimized every conceivable aspect of the site. They predicted that they could get the average load time below 1s. When they released their new, lightning fast code, their average load times tripled.</p>
    <p>There were millions of users in the global south who suddenly were able to watch videos without the page timing out. The team had stumbled onto a massive audience they didn't know they had simply by taking best practices seriously.</p>
    <p>Do what you can for those you're aware of, and keep looking for those you aren't.</p>
</section>
<section>
    <h3>Ok, so who is the user?</h3>
    <p>You are in the strange position of making things that strangers will use. Some of these strangers may take it apart and put it back together. Some of these strangers will be malicious, some will be children, some will be clueless. Some of these strangers won't be human.</p>
    <p>SEO is just usability for bots. Design patterns, OOP and code comments are usability for other programmers (or yourself, later).</p>
</section>
<section class="slide-only">
    <h2>Here's what we're going today</h2>
    <ol>
        <li>Attendance</li>
        <li>OCAS is coming</li>
        <li>Theory
            <ol>
                <li>WAI-ARIA</li>
                <li>Accessibility in JS Frameworks</li>
                <li>Analyzing test results</li>
            </ol>
        </li>
    </ol>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3></h3>
            <p>Please <a href="http://etc.ch/Kpep" target='_blank'>mark your attendance down</a>.</p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>OCAS</h3>
            <p>Tudor Whiteley will be coming in at noon today to meet you and address any questions you have in regards to the desktop+mouse testing.</p>
</section>



<section class="slide-only">
        <h2>Here's what we're going today</h2>
        <ol>
            <li>Attendance</li>
            <li>All your reading assignments are due by Friday</li>
            <li>Good luck today (or tomorrow)!</li>
            <li>Bonus points</li>
            <li>Reviewing the readings</li>
            <li>Theory
                <ol>
                    <li>Review</li>
                    <li>Snaps is the name of the game</li>
                </ol>
            </li>
            <li>Praxis
                <ol>
                    <li>Usability assessment... of this course</li>
                </ol>
            </li>
        </ol>
    </section>
    <section class="slide-only">
        <h3></h3>
        <p>Please <a href="http://etc.ch/Kpep" target='_blank'>mark your attendance down</a>.</p>
    </section>
    <section class="slide-only">
        <h3>Reading assignments</h3>
        <p>Have all your reading assignments in to me by EOD Friday. I'm going to try to have all your final marks in by early next week.</p>
    </section>
    <section class="slide-only">
        <h3>Final project - good luck!</h3>
        <p>You're going to do great. Let's take a look at the rubric to remember our priorities going in to this...</p>
    </section>
    <section>
        <table>
            <caption>Final rubric</caption>
            <thead>
                <tr>
                    <th>Criteria</th>
                    <th>Presentation</th>
                    <th>Written</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Speaking to the goals</td>
                    <td>5</td>
                    <td>10</td>
                </tr>
                <tr>
                    <td>Talking about the methods</td>
                    <td>5</td>
                    <td>10</td>
                </tr>
                <tr>
                    <td>Walking through the results</td>
                    <td>10</td>
                    <td>5</td>
                </tr>
                <tr>
                    <td>Strong conclusions</td>
                    <td>5</td>
                    <td>10</td>
                </tr>
                <tr>
                    <td>Reasonable recommendations</td>
                    <td>10</td>
                    <td>5</td>
                </tr>
                <tr>
                    <td>Documentation</td>
                    <td>N/A</td>
                    <td>20</td>
                </tr>
                <tr>
                    <td>Responding to questions</td>
                    <td>10</td>
                    <td>N/A</td>
                </tr>
            </tbody>
            <tfoot>
                <tr>
                    <td><strong>Total</strong></td>
                    <td><strong>40%</strong></td>
                    <td><strong>60%</strong></td>
            </tfoot>
        </table>
    </section>
    <section class="slide-only">
        <h3>Bonus points</h3>
        <p>I will be awarding up to 3 bonus points per person. These will be added to your final assignment mark. They will be awarded based on the questions you ask to your classmates about their assignments.</p>
        <p>Ask these questions from a client's point of view.</p>
        <p>Make sure they are <strong>questions</strong>. You won't get bonus points by being mean.</p>
        <p>The point of these questions is to give your classmates the opportunity to address any potential weaknesses in their methodology or recommendations.</p>
    </section>
    <section class="slide-only">
        <p>If you're being asked a question, don't get defensive - take it as an opportunity to explain why you made your choices, and to explain how any weaknesses could be addressed going forward, either with further testing, or by doing things differently next time.</p>
    </section>
    <section class="slide-only">
        <h3>Office culture</h3>
        <p>Office culture is different from most other workplaces and it's definitely different from school.</p>
        <p>Offices have their own dialect, customs, style of dress, form of humour, and expectations around behaviour and communication.</p>
    </section>
    <section class="slide-only">
        <p>Every office is a little different. One question I like to ask when being interviewed is "What can you tell me about the culture here?</p>
        <p>This is a question about how to dress, how to talk to your co-workers, how supported you'll be in your work, and how aggressively you'll be expected to self-manage.</p>
    </section>
    <section class="slide-only">
        <p>Office culture in Canada is undergoing a generational shift.</p>
        <p>Older customs tend to be more formal in language and dress, more strict about job definitions and parameters (including work hours), and with more deference to authority.</p>
        <p>"Younger" offices tend to place more of an emphasis on 'likeability', blurring the lines between work and recreation, and have higher expectations about taking on responsibility.</p>
        <p>Expect to find an older office culture in larger institutions like universities, banks, and government.</p>
        <p>If the company you're working for has ever described itself as a 'startup', expect to have your work interrupted by grown men playing with children's toys.</p>
    </section>
    <section class="slide-only">
        <p>Particular attention needs to be paid to language. Some offices have a culture where, in some contexts, swearing or using <span role="img" aria-label="beaming face with smiling eyes">😁</span> is the norm. What's important is that you communicate using the same norms as the rest of your team/office.</p>
        <p>Despite the generational differences, offices everywhere tend to be much gentler when communicating differences of opinion than, say, a restaurant or a construction site.</p>
        <p>However, there is an expectation that you will communicate your needs. Otherwise people will keep being polite with you - until they politely fire you.</p>
    </section>
    <section class="slide-only">
        <p>Jessica's going to tell us a story about people being polite to her - in a bad way.</p>
    </section>
    <section class="slide-only">
        <h3>Why am I telling you this?</h3>
        <p>Modern office culture has certain expectations around 'respectfulness'. When addressing other people's ideas, <em>even when they're dumb ideas that make you angry</em>, you'll be expected to smile, say something positive, and then address your concerns by asking a gentle question.</p>
        <p>When you are asking questions today, your challenge is to ask questions that will get the answers you need, while still maintaining a good relationship with everyone in the room.</p>
    </section>
    <section>
        <h3>Let&#39;s review!</h3>
        <p>But first - something I was reminded of.</p>
        <p>I was reading some writings by people with disabilities, and a point that kept coming up was this - no one is disabled.</p>
        <p>Which is to say, there is nothing about any one person that creates disability. Disability is created when society makes an assumption, and then hardcodes that into design.</p>
        <p>It's in the way we design our buildings and our cities, our school system, our language, et al.</p>
        <p>I think this is important, because you need to understand that when you make something, you are at risk of manufacturing disability.</p>
    </section>
    <section>
        <h3>Let&#39;s review - the readings!</h3>
        <p>You responded more than I thought you would to the reading assignments. More than one of you said you would've liked it if there was more in-class discussion.</p>
        <ol>
            <li class="fragment">Get into small groups.</li>
            <li class="fragment">Choose a reading you&#39;d like to talk about.</li>
            <li class="fragment">What do you remember about it?</li>
            <li class="fragment">Is this a topic you&#39;d thought about before?</li>
            <li class="fragment">Did it change your mind about anything?</li>
            <li class="fragment">Does it change how you think about web development?</li>
            <li class="fragment">Choose someone to present your ideas to the class.</li>
        </ol>
    </section>
    <section>
        <h3>Usability review</h3>
        <p>Usability is not UAT, UX, UI, CX, HCI, IxD, or HCD (although they may overlap).</p>
        <p>Usability is <q>the extent to which specified users can find, understand and use information and services</q>.</p>
        <p>To start with a solid foundation of usability, we develop personas and scenarios.</p>
        <p>To assess usability, we test.</p>
    </section>
    <section>
        <p>In testing, we use a variety of methods, designed to reduce our biases, to collect data on how real people perceive and interact with the design and function of the products we make.</p>
        <p>We do this iteratively throughout the design and production process (including after our product has launched), testing our ideas and improvements, and comparing solutions.</p>
    </section>
    <section>
        <p>During the initial design phase, we develop <strong>personas</strong>, composite identities of our audience, in order to design our product <em>for people to use</em>.</p>
        <p>Based on those personas, since websites tend to be non-linear tools, we develop <strong>scenarios</strong>. Scenarios help us keep track of the different journeys that people in our audience may take in using our product.</p>
        <p>Personas and scenarios are tools for guiding design and implementation discussions, particularly with less technical team members.</p>
    </section>
    <section>
        <p>Once we begin to test our design and development, we use tests to produce both <strong>qualitative</strong> and <strong>quantitative</strong> data.</p>
        <p>Depending on what kind of data we are generating, there are industry standard sample sizes for each test. Qualitative testing, being more exploratory, tends to have smaller sample sizes.</p>
    </section>
    <section>
        <p>To facilitate discussion and decision-making, we can apply quantitative metrics to qualitative data. One example of this is the PURE rubric, for assigning values to the ease with which a task is accomplished.</p>
        <p>This should not overshadow the fact that the most valuable information gained in qualitative testing is usually individual, and best reported in the words of the participant or observer.</p>
    </section>
    <section>
        <p>Before we test, we plan. After we test, we report.</p>
        <p>A good test plan can be a <strong>proposal</strong> (when seeking approval) that provides a clear picture of the time and costs, and makes a case for the efficacy of data that is being generated.</p>
        <p>A good test plan might also be, assuming that approvals and funding are secured, <strong>simple documentation</strong> for your team, in order to keep sight of the scope, definitions, and goals.</p>
    </section>
    <section>
        <p>A good report is readable, credible, and makes clear recommendations for how to action the findings.</p>
    </section>
    <section>
        <p>A friend of mine who does usability testing says that their team has a library of possible tests. They get hired to choose the right test.</p>
    </section>
    <section>
        <p>Usability tests include, but are not limited to:</p>
        <ol>
            <li class="fragment">problem discovery</li>
            <li class="fragment">heuristic evaluation</li>
            <li class="fragment">system usability surveys</li>
            <li class="fragment">moderated/unmoderated</li>
            <li class="fragment">in-person/remote</li>
            <li class="fragment">benchmarks</li>
            <li class="fragment">eye-tracking</li>
        </ol>
    </section>
    <section>
        <p>When performing a test, we try to capture data that is clean and unbiased. We can do this by using careful language, so as not to influence our test participants.</p>
        <p>We also do this by having strong sample sizes, and reducing the number of variables between our tests, i.e. maintaining a consistent hardware and software environment.</p>
    </section>
    <section>
        <p>Once our test data is collected, we format it, and discuss it within our team.</p>
        <p>Collaborating on our recommendations reduces individual bias.</p>
        <p>We then weigh our recommendations based on issue severity and the resources required to implement.</p>
        <p>Whenever possible, we try to provide more than one option for each issue, so the client can decide what is best for them - without putting them in the position of rejecting our work.</p>
    </section>
    <section>
        <p>A report should be easy to read and understand. Choosing the right format for presenting data is essential to interpreting it.</p>
        <p>If you have been rigourous in your testing, then your report can be presented in very plain language.</p>
        <p>Reporting these results is often done in-person. It's important that you understand everything that went into the test and the recommendations, and anticipate questions that the client may raise.</p>
    </section>
    <section class="slide-only">
        <h3>Snaps is the name of the game</h3>
    </section>
    <section class="slide-only">
        <h3>Mild, medium, or spicy?</h3>
    </section>
    <section class="slide-only">
        <h3>heuristic course evaluation</h3>
        <p>
            <ol>
                <li>Get into groups of 4</li>
                <li>Pull up the Nielson Norman Group's <a href='https://www.nngroup.com/articles/ten-usability-heuristics/' target='_blank'>10 Usability Heuristics for User Interface Design</a></li>
                <li>In your group evaluate this course, the content, the lessons, the labs, the lab, the assignments, schedule, syllabus, blackboard, et. al.</li>
                <li>Take note of what worked well and what the pain points were.</li>
                <li>Generate recommendations</li>
                <li>Present your findings</li>
            </ol>
        </p>
    </section>