---
title: "Week 7... Plus Week 8?"
date: 2020-06-30T08:47:11+01:00
publishdate: 2020-06-30T08:47:11+01:00
featured_image: groundhog.jpg
summary: "This week I've combined last year's week seven and eight"
---
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

<section>
    <h3>Accessibility in Front-end JS Frameworks</h3>
    <p>Today we're going to look at <a href='https://stateofjs.com/2017/front-end/results' target='_blank'>the big three</a>.</p>
    <p>Let's keep in mind that >4% of users in the WebAIM survey were using IE 6, 7 or 8.</p>
    <p>
        <table>
            <caption>Browser support of javascript frameworks</caption>
            <tbody>
                <tr>
                    <td>Vue</td>
                    <td>ES5-compliant browsers - IE9+</td>
                </tr>
                <tr>
                    <td>React</td>
                    <td>ES5-compliant browsers - IE9 and IE10 require polyfills</td>
                </tr>
                <tr>
                    <td>Angular</td>
                    <td>Modern browsers. Safari 7 & 8, IE9, 10 & 11, Android 4.1+ require polyfills.</td>
                </tr>
            </tbody>
        </table>
    </p>
</section>
<section>
    <h3>Progressive enhancement</h3>
    <p>Within the last year, we've seen companies like Airbnb and Groupon tell Firefox and Safari users that they are 'optimized for Chrome' when their sites failed.</p>
    <p>What if your website, to borrow a phrase, just worked?</p>
    <p>Consider delivering your content in plain HTML, and then 'mustard-cutting' to deliver your CSS and Javascript.</p>
</section>
<section>
    <h3>Internet Explorer refuses to die.</h3>
    <p><a href='https://netmarketshare.com/browser-market-share.aspx' target='_blank'>Internet Explorer market share is >12%.</a> That's more than Firefox. That's more than Edge, Safari and Opera combined.</p>
    <p>Internet Explorer fails to support <em>hundreds</em> of features that Chrome has implemented.</p>
    <p>Progressive enhancement is how we build for an internet that is increasingly fractured.</p>
    <p>Polyfills, autoprefixer, caniuse, modernizr; these are great things. Consider, though, simply delivering content that any client can access as a Minimum Viable Product.</p>
    <p>A List Apart has <a href='http://alistapart.com/article/the-slow-death-of-internet-explorer-and-future-of-progressive-enhancement' target='_blank'>a wonderful article</a> with some recommendations on how to mustard cut for both CSS and Javascript.</p>
</section>
<section>
    <h3>What are you using your framework for?</h3>
    <p>Is it as a static site generator? Cool. Render on the server. Serving static HTML is waaaay faster.</p>
</section>
<section>
    <h3>Let&#39;s assume...</h3>
    <p>Let's assume you've got your fallbacks and polyfills in place. Let's assume SSR isn't an option. How do we make Vue, React and Angular accessible?</p>
</section>
<section>
    <h3>Accessibility in Angular</h3>
    <p>AngularJS 1.7 shipped with a module called ngAria which created hooks for some aria roles. Angular 2+ seems to not have anything similar. You're on your own!</p>
</section>
<section>
    <h3>Accessibility in React</h3>
    <p>React seems to be a lot more on top of accessibility. They even bother to mention it in <a href='https://reactjs.org/docs/accessibility.html' target='_blank'>their docs</a>!</p>
    <p>Aria attributes are supported in JSX (but note that they're lowercased instead of camelcased like most other attributes).</p>
</section>
<section>
    <h3>A few gotchas with React</h3>
    <p>JSX has a tendency to break semantics though, especially with lists and tables, so get familiar with <Fragment>s and <></> syntax.</p>
    <p>The `for` attribute, used with labels, is written as `htmlFor` in JSX</p>
</section>
<section>
    <h3>React A11y</h3>
    <p><a href='https://github.com/reactjs/react-a11y' target='_blank'>react-a11y</a> is a promising looking tool for warning about potential accessibility issues in your React components.</p>
</section>
<section>
    <h3>Accessibility in Vue</h3>
    <p>Vue doesn't have any <a href='https://github.com/vuejs/vuejs.org/issues/974' target='_blank'>accessibility documentation... yet</a>.</p>
    <p>Emily Mears has written <a href='https://medium.com/@emilymears/getting-started-with-web-accessibility-in-vue-17e2c4ea0842' target='_blank'>a pretty great article</a> about accessibility in Vue. The main challenges are held in common with React - updating meta, handling focus and implementing aria.</p>
    <p>Vue is pretty great as a framework - it's easier to pick up and understand than other frameworks, it scales much more gracefully than React, and only updates the components that need re-rendering.</p>
</section>
<section>
    <h3>Controlling focus in client-side frameworks</h3>
    <p>All three frameworks aggressively re-render the DOM - that's kind of the point.</p>
    <p>Be aware that changes to the URL, and rendering of the virtual DOM can wreak havoc on focus. Each framework has methods for mitigating this with programmatic focus control: <a href='https://simplyaccessible.com/article/react-a11y/' target='_blank'>refs in React</a>; <a href='https://www.npmjs.com/package/vue-focus' target='_blank'>vue-focus in Vue</a>; <a href='https://docs.angularjs.org/api/ng/directive/ngFocus' target='_blank'>ngFocus in Angular</a>. Make sure you're familiar with the appropriate technique.</p>
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