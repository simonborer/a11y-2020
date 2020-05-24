---
date: 2020-06-07 08:47:11 +01:00
featured_image: count.jpg
publishdate: 2020-06-07 08:47:11 +01:00
summary: "This week we'll cover queries that use aggregate functions; queries with MAX, MIN, COUNT, AVG, and SUM group functions; the use of the GROUP BY and HAVING clauses; the differences between HAVING and WHERE clauses. We'll cover subqueries & have a brief introduction to CRUD."
title: "Week 4 - Use of Functions"
today: 

---
<section class="slide-only">
    <h2>Here's what we're going today</h2>
    <ol>
        <li>Another test?</li>
        <li>Moving forward with OCAS</li>
        <li>What would you like to go over from last week?</li>
        <li>Praxis
            <ol>
                <li>Linting!</li>
                <li>An accessible accordion</li>
            </ol>
        </li>
    </ol>
</section>
<section class="slide-only">
    <h3>Would you like to participate in a test?</h3>
    <p>We have been asked to use <a href='https://public.tableau.com/profile/humber.college#!/vizhome/HumberCollege-CareerOutlooks/CareerOutlooks'>this site</a> and fill out <a href='https://goo.gl/gn411u' target='_blank'>this survey</a>.</p>
</section>
<section class="slide-only">
    <h3>OCAS is a great case study in requirements</h3>
</section>
<section class="slide-only">
    <h3>Let`s see what some people missed...</h3>
    <p><a href='/a11y/slides/notes/week-2/' target='_blank'>...last week</a></p>
</section>
<section>
    <h3>Hooray for linting!</h3>
    <p>Clone <a href="https://github.com/simonborer/a11y-linting" target='_blank'>https://github.com/simonborer/a11y-linting</a></p>
</section>
<section>
    <p>We will be looking at both an html linter (<code>htmllint</code>) and a command line auditing tool (<code>lighthouse</code>).</p>
</section>
<section>
    <h3>HTMLLint</h3>
    <ol>
        <li class="fragment">Open the project in your text editor</li>
        <li class="fragment">Look at package.json under &#34;dependencies&#34; and &#34;devDependencies&#34;</li>
        <li class="fragment">Open your command line client</li>
        <li class="fragment">Go to the project folder</li>
        <li class="fragment">Run &lt;code&gt;npm install&lt;/code&gt;</li>
    </ol>
</section>
<section>
    <ol>
        <li class="fragment">Look at package.json under &#34;scripts&#34; - this is where we define the node scripts the will get called by &lt;code&gt;npm run&lt;/code&gt;</li>
        <li class="fragment">&lt;code&gt;npm run build&lt;/code&gt;</li>
        <li class="fragment">htmllint options are defined in .htmllintrc - try getting rid of one of the tag bans to clear an error</li>
        <li class="fragment">Now try fixing the html to clear the rest</li>
        <li class="fragment">Tell me why we put htmllint under the &#34;build&#34; script</li>
    </ol>
</section>
<section>
    <h3>Lighthouse CLI</h3>
    <ol>
        <li class="fragment">Look at package.json under &#34;scripts&#34;, at the &#34;audit&#34; script. Read me this script in non-technical terms.</li>
        <li class="fragment">Run &lt;code&gt;npm run audit&lt;/code&gt; and view the output file.</li>
    </ol>
</section>
<section>
    <h3>Exercise: an accessible accordion</h3>
    <p>Build an accessible accordion and submit it as a pull request. Feel free to pair-program.</p>
</section>
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