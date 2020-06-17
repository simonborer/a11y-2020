---
title: "Step 6 - State change & frameworks"
date: 2020-06-21T08:47:11+01:00
publishdate: 2020-06-21T08:47:11+01:00
featured_image: space-time.jpg
summary: "This week we'll look at accessibility when state changes, and accessibility in Javascript application frameworks"
---
<section>
    <h3>Accessible content - form labels, instructions and errors</h3>
    <p>Be very clear about what's expected of a user, and how errors should be resolved. A red asterisk appearing suddenly adjacent to an input isn't helpful to everyone.</p>
</section>
<section>
    <h3>Mobile accessibility</h3>
    <p>The WCAG has <a href='https://www.w3.org/TR/IMPLEMENTING-UAAG20/mobile' target='_blank'>multiple documents</a> on <a href='https://www.w3.org/TR/mobile-accessibility-mapping/'>how accessibility standards translate to mobile</a>.</p>
    <p>It's mostly along the lines of 'don't try to cram your whole desktop site onto mobile', and 'just make sure that you're doing what you do on desktop', but with a few extra cautions.</p>
</section>
<section>
    <ol>
        <li class="fragment">Take special pains to test resizing up to 200%.</li>
        <li class="fragment">You definitely still have to have keyboard-only controls</li>
        <li class="fragment">Touch targets are at least 9mm x 9mm, with adequate space between them (without magnification)</li>
        <li class="fragment">Use mouseup or touchend events so that users can change their minds</li>
    </ol>
</section>
<section>
    <ol>
        <li class="fragment">Gestures should be kept simple, and have alternatives</li>
        <li class="fragment">Support either orientation</li>
        <li class="fragment">Put important elements above the fold</li>
        <li class="fragment">Provide easily discoverable instructions</li>
        <li class="fragment">Set the keyboard to the type of data entry required</li>
        <li class="fragment">No scrolljacking</li>
        <li class="fragment">Show focus</li>
    </ol>
</section>
<section>
    <h3>Accessible tabs are &lt;em&gt;hard&lt;/em&gt;</h3>
    <p>
        <p data-height="265" data-theme-id="0" data-slug-hash="pVBoQx" data-default-tab="js,result" data-user="simonborer" data-embed-version="2" data-pen-title="pVBoQx" class="codepen">See the Pen <a href="https://codepen.io/simonborer/pen/pVBoQx/">pVBoQx</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>) on <a href="https://codepen.io">CodePen</a>.</p>
        <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
    </p>
</section>
<section class="slide-only">
    <h2>Here's what we're going today</h2>
    <ol>
        <li>Attendance</li>
        <li>Final projects</li>
        <li>Unpaid internships</li>
        <li>Being a test subject</li>
        <li>Theory
            <ol>
                <li>UAT vs Usability</li>
                <li>Mobile accessibility</li>
                <li>Accessible content</li>
            </ol>
        </li>
        <li>Praxis
            <ol>
                <li>Being a test participant</li>
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
<section>
    <h3>Your final</h3>
    <p>Your final project is a usability study, presented during the final lab. Your presentation should run 5-8 minutes. You will be required to present the findings of your test in person.</p>
    <p>A slide presentation is acceptable, as is a longform document. Either way though, your report needs to present what you did, why you did it, what the results are, and what your recommendations are based on those results. You must also include all the data that backs up your conclusions (although you don't necessarily need to talk through every single data point, as that would be pretty boring).</p>
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
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>11:30</h3>
            <p>At 11:30 today we'll be helping to test the usability of the Humber Career Outlooks web app. Approach it as a participant, but while you're taking part, reflect on their methodology. We'll get to talk about what we thought about <em>their</em> testing in the lab. Would you have taken the same approach? Does this change how you'll interact with your test participants?</p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>Unpaid internships</h3>
            <p>https://www.labour.gov.on.ca/english/es/pubs/internships.php</p>
            <p>
                <blockquote>
                    <p>The Ministry of Labour is committed to ensuring fairness and protecting young workers. The fact that you are called an “intern” does not determine whether or not you are entitled to the protections of the Employment Standards Act, 2000 (ESA), including the minimum wage.</p>
                    <p>...The ESA does not apply to an individual who performs work <strong>under a program</strong> approved by a college of applied arts and technology or a university.</p>
                    <p>...If someone performing work as an unpaid intern is unsure of whether he or she is excluded from the ESA, he or she should call the Employment Standards Information Centre toll-free at 1-800-531-5551 for further information.</p>
            </p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>Reading without peeking</h3>
            <p>How was it using a screenreader?</p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>Where are you at?</h3>
            <p>How do you feel about the testing so far?</p>
            <p>Are you confident that you'll be able to draw meaningful conclusions about the data?</p>
            <p>Did anything surprise you?</p>
            <p>What would you like to change going forward?</p>
            <p>What's difficult?</p>
            <p>What's easy?</p>
            <p>What's fun?</p>
            <p>What's not?</p>
</section>
<section>
    <h3>Differentiating UAT &amp; Usability testing</h3>
    <p>UAT and usability testing are both kinds of testing. As are regression testing, unit testing and integration testing. Tests have plans, requirements and scenarios.</p>
</section>
<section>
    <p>
        <table>
            <thead>
                <tr>
                    <td>Usability</td>
                    <td>UAT</td>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Meant to determine whether users can learn, understand and use the product efficiently to achieve theirgoals.</td>
                    <td>Meant to determine whether the client is satisfied that the product meets their requirements.</td>
                </tr>
                <tr>
                    <td>Can happen before or during development, before or after launch.</td>
                    <td>Happens after development, but before launch.</td>
                </tr>
                <tr>
                    <td>Tests whether users can achieve the result they want.</td>
                    <td>Tests whether the product produces the expected result.</td>
                </tr>
                <tr>
                    <td>Meant to generate continuous improvements.</td>
                    <td>Meant to achieve final sign-off.</td>
                </tr>
                <tr>
                    <td>Run by the software team.</td>
                    <td>Run by the client.</td>
                </tr>
            </tbody>
        </table>
    </p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>OH NO POP QUIZ</h3>
            <p>Please go to <a href='http://etc.ch/Yfga' target='_blank'>the quiz</a></p>
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