---
title: "Week 5 - Database Design / Midterm Prep"
date: 2020-06-14T08:47:11+01:00
publishdate: 2020-06-14T08:47:11+01:00
featured_image: arch.jpg
summary: "This week we'll cover the basic steps to design a database; relationships between tables; identify tables and assign columns; identify primary and foreign keys; primary key constraints; foreign key constraints; midterm review."
today:
  -
    title: Steps to designing a database
    id: design
  -
    title: Midterm prep
    id: midterm
  -
    title: Assignment
    id: lab
---
<section class="slide-only">
    <h2>Here's what we're going today</h2>
    <ol>
        <li>Great news!</li>
        <li>Midterms</li>
        <li>Theory
            <ol>
                <li>How to write a usability report</li>
                <li>A game :)</li>
                <li>Evangelism</li>
                <li>Workflow</li>
            </ol>
        </li>
        <li>Praxis
            <ol>
                <li>OCAS</li>
                <li>Your weekly reading</li>
            </ol>
        </li>
    </ol>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>Great news!</h3>
            <p><img src="https://cdn.insidetimmies.com/wp-content/uploads/2014/06/image.jpg" alt="Timbits" style="max-height: 20rem"><br>We're getting paid (in food) to do that test we talked about last week.</p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>Midterm stuff people struggled with</h3>
            <ol>
                <li class="fragment">On any project, there are client requirements, and there are team standards. In the case of the midterm, the client requirements were my instructions. The team standards are Humber&#39;s rules against plagiarism (among other things).</li>
                <li class="fragment">The entire first paragraph of the assignment.</li>
                <li class="fragment">Scope: don&#39;t just factor in all the cool stuff that &lt;em&gt;might&lt;/em&gt; be useful - take a look at the resources you have available and scope for what you can deliver. There&#39;s nothing wrong with a narrow scope that provides really crisp data.</li>
                <li class="fragment">Some people will probably want to change their scope. Or maybe you&#39;re just not happy with your grade. You&#39;ve got a week to resubmit.</li>
            </ol>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <p>Also, please have all your first-term reading assignments in by this time next week. That's the cut-off.</p>
</section>

<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>A game :)</h3>
            <ol>
                <li class="fragment">In an even number of groups of 3-4...</li>
                <li class="fragment">...you are paired with another group.</li>
                <li class="fragment">Create a scorecard for your group with 4 columns - month, price, profit, and total profit.</li>
                <li class="fragment">Subdivide the latter 3 columns into subcolumns, each labelled alternately &#39;us&#39; and &#39;them&#39;</li>
            </ol>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <p>You are competing businesses. Each month you set the price on your product. Your costs are absolutely fixed. Bankruptcy is impossible. Your profits are driven entirely by market competition.</p>
            <p>Each month, you must write down 6 figures: what price you chose, what price your competitor chose, what profit you made, what profit they made, what total profit you made, and what total profit they made.</p>
            <p>The goal of the game is to maximize your company's profit.</p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <h3>Price/Profit</h3>
            <p>
                <table>
                    <thead>
                        <tr>
                            <th>Your price</th>
                            <th>Their price</th>
                            <th>Your profit</th>
                            <th>Their profit</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>$30</td>
                            <td>$30</td>
                            <td>110</td>
                            <td>110</td>
                        </tr>
                        <tr>
                            <td>$30</td>
                            <td>$20</td>
                            <td>20</td>
                            <td>180</td>
                        </tr>
                        <tr>
                            <td>$30</td>
                            <td>$10</td>
                            <td>20</td>
                            <td>150</td>
                        </tr>
                        <tr>
                            <td>$20</td>
                            <td>$30</td>
                            <td>180</td>
                            <td>20</td>
                        </tr>
                        <tr>
                            <td>$20</td>
                            <td>$20</td>
                            <td>80</td>
                            <td>80</td>
                        </tr>
                        <tr>
                            <td>$20</td>
                            <td>$10</td>
                            <td>30</td>
                            <td>150</td>
                        </tr>
                        <tr>
                            <td>$10</td>
                            <td>$30</td>
                            <td>150</td>
                            <td>20</td>
                        </tr>
                        <tr>
                            <td>$10</td>
                            <td>$20</td>
                            <td>150</td>
                            <td>30</td>
                        </tr>
                        <tr>
                            <td>$10</td>
                            <td>$10</td>
                            <td>50</td>
                            <td>50</td>
                        </tr>
                    </tbody>
                </table>
            </p>
</section>
<section class="slide-only">
    <div class="grid-x">
        <div class="cell large-6 large-offset-3 medium-10 medium-offset-1">
            <ol>
                <li class="fragment">Who won?</li>
                <li class="fragment">What was your strategy?</li>
                <li class="fragment">Assumptions did you make?</li>
                <li class="fragment">What would you do differently?</li>
            </ol>
</section>
<section>
    <h3>Evangelism</h3>
    <p>You know a lot already. It won't be long until you're working with someone who knows less than you. They will probably be your boss.</p>
    <p>You'll learn that when you're in a room full of developers, you'll argue differently.</p>
    <p>You will know how to solve problems. You will know the cutting edge of technology. You will feel the inefficiencies start to weigh on you.</p>
</section>
<section>
    <p>What will you do when you're the only person who knows how to make a website accessible?</p>
    <p>What will you do when you're the only person who cares about responsive design? Or load times? Or security?</p>
    <p>You need to make it so your team understands</p>
    <p>You need to make it so your boss doesn't need to understand.</p>
</section>
<section>
    <h3>When your team can improve</h3>
    <p>If there are improvements you can make within your team without additional resources, present it as an opportunity to make your lives easier, and/or grow your skillset.</p>
    <p>But remember, anything that starts with 'If everyone would just...' isn't a solution.</p>
    <p>Peer review, linting, automation. You need to get your team to agree to be held accountable.</p>
</section>
<section>
    <h3>When you need resources</h3>
    <ol>
        <li class="fragment">Get team buy-in</li>
        <li class="fragment">Explain the cost of the issue</li>
        <li class="fragment">Explain the cost of 2 options, both of which you are ready and willing to implement</li>
    </ol>
</section>
<section>
    <h3>OCAS</h3>
    <p>Time to start! ... or is it?</p>
</section>
<section>
    <h3>Praxis: Listening to your reading</h3>
    <p>Your reading this week is <a href='https://webaim.org/projects/screenreadersurvey7/'>https://webaim.org/projects/screenreadersurvey7/</a></p>
    <p>If you have headphones with you, please read it with either <a href='https://www.nvaccess.org/' target='_blank'>NVDA</a> or <a href='https://help.apple.com/voiceover/info/guide/10.12/' target='_blank'>>VoiceOver</a>. Or choose another!</p>
</section>